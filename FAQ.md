# FAQ

## Contents

* [Batch Scripting](#Batch_Scripting)
   * [How do I split a string?](#How_do_I_split_a_string?)
* [Environment Variables](#Environment_Variables)
  * [Why won't my changes to `%PATH%`/`%PATHEXT%` save properly?](Why_won't_my_changes_to_`%PATH%`/`%PATHEXT%`_save_properly?)

## Batch Scripting

### How do I split a string?

## Environment Variables

### Why won't my changes to `%PATH%`/`%PATHEXT%` save properly?

Because when a console session ends, any changes made to the environment variables are discarded.
In order to retain the changes, they must be made outside of `cmd`.

One option for setting them is:
1. Press <kbd>Win</kbd>+<kbd>R<kbd> to bring up the 'Run' prompt.
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