
# MacroError Object (Access)

Represents the properties of a run-time error that occurs in a macro.


## Remarks

When an error occurs in a macro, information about the error is stored in the  **MacroError** object. If you have not used the **OnError** action to suppress error messages, the macro stops and the error information is displayed in a standard error message. However, if you have used the **OnError** action to suppress error messages, you may want to use the information stored in the **MacroError** object in a condition or a custom error message.

After an error has been handled, the information in the  **MacroError** object is out of date, so it is a good idea to clear the object using the **ClearMacroError** action. This resets the error number in the **MacroError** object back to zero, and clears any other information about the error that is stored in the object, such as the error description, macro name, action name, condition, and arguments. This way, you can inspect the **MacroError** object again later to see if another error has occurred.

The  **MacroError** object contains information about only one error at a time. If more than one error has occurred in a macro, the **MacroError** object contains information about only the last one.

The  **MacroError** object does not contain information about run-time errors that occur when running Visual Basic for Applications (VBA) code. See[Elements of Run-Time Error Handling](a0e06a1e-2709-aa51-92d0-340788a31a8a.md) for more information about handling run-time errors in VBA.


## See also


#### Concepts


[Access Object Model Reference](2de134a4-6c5c-d2a3-8377-f4dd973ba650.md)
#### Other resources


[MacroError Object Members](43288575-7577-6750-6822-cc4b7ddbb9e7.md)
