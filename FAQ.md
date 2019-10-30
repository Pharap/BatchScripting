# FAQ

## Contents

* [Batch Scripting](#batch-scripting)
   * [How do I split a string?](#how-do-i-split-a-string)
* [Environment Variables](#environment-variables)
  * [Why won't my changes to `%PATH%`/`%PATHEXT%` save properly?](#why-wont-my-changes-to-pathpathext-save-properly)

## Batch Scripting

### How do I split a string?

To be added...

## Environment Variables

### Why won't my changes to `%PATH%`/`%PATHEXT%` save properly?

Because when a console session ends, any changes made to the environment variables are discarded.
In order to retain the changes, they must be made outside of `cmd`.

One option for setting them is:
1. Press <kbd>Win</kbd>+<kbd>R</kbd> to bring up the 'Run' prompt.
2. Type `SystemPropertiesAdvanced` or `SystemPropertiesAdvanced.exe` to access the Advanced tab of System Properties
3. Click `Environment Variables...`

Then for `%PATH%`:
1. Locate or create `Path` in the list of `User variables`
  * If creating it, copy the default settings from the value found in the `System variables` list
2. Choose `Edit...` and edit the value
  * I.e. append a `;` followed by a complete path to the chosen directory
3. Click `OK` to confirm any changes and close the `Edit User Variable` dialogue
4. Click `OK` to confirm any changes and close the `Environment Variables` dialogue
5. Click `OK` to confirm any changes and close the `System Properties` dialogue

Or alternatively for `%PATHEXT%`:
1. Locate or create `PATHEXT` in the list of `User variables`
  * If creating it, copy the default settings from the value found in the `System variables` list
2. Choose `Edit...` and edit the value
  * I.e. append a `;` followed by a `.` and the desired extension, preferably in all caps
3. Click `OK` to confirm any changes and close the `Edit User Variable` dialogue
4. Click `OK` to confirm any changes and close the `Environment Variables` dialogue
5. Click `OK` to confirm any changes and close the `System Properties` dialogue
