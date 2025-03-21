# Hi6 Robot Controller Function Manual - Ladder Edit

{% hint style="warning" %} The information provided in this product manual is the property of Hyundai Robotics.

It cannot be reproduced or redistributed in part or whole without written consent from Hyundai Robotics, and it cannot be provided to third parties or used for other purposes.

The manual is subject to change without prior notification.

Copyright ⓒ 2025 by Hyundai Robotics {% endhint %}# 1. OverView

{% hint style="info" %}This feature is supported from version V60.32-00 and later.

{% endhint %}# 1.1 Ladder Edit

The Ladder Edit function of the Hi6 controller is an embedded feature that allows users to directly create and edit ladder programs for the Hi6's built-in PLC.

The editing method is similar to HRLadder, a dedicated ladder editing PC software for Hyundai Robotics. Therefore, users who have experience editing ladder programs using HRLadder will be able to quickly familiarize themselves with the function through this manual.

HRLadder can be downloaded by searching for it on the Hyundai Robotics website (https://www.hd-hyundairobotics.com/main) - Customer Support - Download Center.
For instructions on how to use HRLadder, please refer to the user manual linked in the help menu of HRLadder.

{% hint style="info" %} For information on the Hi6 controller settings, relays, and the built-in PLC, please refer to the [ Hi6 Embedded PLC Manual](https://hrbook-hrc.web.app/#/view/doc-hi6-embedded-plc/korean/README) 를 참조하시기 바랍니다.

{% endhint %}  
# 2. Starting Ladder Edit
This section explains the location and process to execute the Ladder Edit function.# 2.1. Initial Screen
Let’s execute the Ladder Edit function.

1. Touch the [pane layout] button on the right side of the screen, the [split] button at the bottom, and then the [select] button at the lower left in sequence. The panel selection window will appear.<br><br>
    <img src="../_assets/split_window_en.png" width="600">
    <br><br>

2. Select Edit Ladder in the panel selection window.<br><br>
<img src="../_assets/select_panel_en.png" width="600"><br><br>

3. The Ladder Edit function will start.<br><br>
If the bottom button bar is not in the form shown below, press the ESC button.
<br><br>
<img src="../_assets/f_btn_screen_en.png" width="600"><br><br>
You can use various functions through the buttons at the bottom.
<br><br><br>

Here is an explanation of the functions of each button.<br>
<table text-align: center; style="tg">
    <tr>
        <th colspan = 3 style="text-align: center;"> Button</th>
        <th style="text-align: center;">functions </th>
    </tr>
    <tr>
        <td colspan = 3> File</td>
        <td > File-related functions such as loading and saving files. </td>
    </tr>
    <tr>
        <td colspan = 3>Edit</td>
        <td>Editing functions such as undo, copy, paste, find/replace, etc.</td>
    </tr>
    <tr>
        <td colspan = 3>Layout</td>
        <td>Screen-related functions such as full-screen mode, branch spacing, tag format, etc.</td>
    </tr>
    <tr>
        <td colspan = 3>Insert</td>
        <td>All elements that can be inserted.</td>
    </tr>
    <tr>
        <td colspan = 3>Tool</td>
        <td>PLC monitoring-related functions such as syntax checking, comparison, Remote RUN/STOP, etc.</td>
    </tr>
</table>

# 3. Ladder Diagram Editing
This section explains the editing of the ladder diagram.# 3.1 Insert Element
The method of editing the ladder diagram is similar to the editing method of HRLadder, so for more detailed instructions, please refer to the basic editing section in the HRLadder manual.

1. The insertion of all elements can be accessed through the Insert button on the bottom button bar.<br><br>
    <img src="../_assets/f_btn_insert_en.png" width ="355" ><br>
    <img src="../_assets/f_btn_elements.png" width ="500" ><br><br>

2. To check other elements, you can touch the prev/next buttons.<br><br>
    <img src="../_assets/insert_move_next_prev_en.png" width ="500" ><br><br>
# 3.2 Editing Features
Other editing functions are the same as the features in HRLadder.<br>
For more detailed editing instructions, please refer to the Ladder Diagram Editing section in the HRLadder manual.
1. The branch gap option makes it easier to edit branches.<br>
    Press the View button on the bottom button bar, then press the Branch Gap button.<br><br>
    <img src="../_assets/f_btn_layout_en.png" width ="415" ><br>
    <img src="../_assets/f_btn_branch_gap_en.png" width ="250" ><br><br>
2. Cut, copy, paste, undo, and redo functions can be accessed by pressing the Edit button on the bottom button bar.<br><br>
    <img src="../_assets/f_btn_edit_en.png" width ="415"><br>
    <img src="../_assets/f_btn_edit_menu_en.png" width ="500"><br><br>

3. Press the [Del] key to delete the selected instructions, or the selected Rung or branch.
<br><br>
# 3.3 Tag Format
The 1-bit data in the relay index can be entered and displayed in one of four formats: 1-bit, 8-bit, 16-bit, or 32-bit.<br>
{% hint style="info" %}For more details on relay notation, please refer to the [Hi6 Embedded PLC Relay Notation Manual](https://hrbook-hrc.web.app/#/view/doc-hi6-embedded-plc/korean/3-relay/2-relay-expression)

{% endhint %}
<br>
 In the Ladder Edit function, you can choose one of the four formats and display it on the ladder diagram in the same way as HRLadder.<br>

1. Press the Layout button, then press the Tag Format button. <br><br>
<img src="../_assets/f_btn_layout_en.png" width ="415"><br>
<img src="../_assets/f_btn_tag_format_en.png" width ="250"><br>

2. Each time you press the Tag Format button, the display format cycles through 1-bit -> 8-bit -> 16-bit -> 32-bit.
# 3.4 Find and Replace
This function allows you to search the entire ladder file for a specified string or replace the found string with another specified string.<br>

Since this is the same feature as in HRLadder, please refer to the "Find and Replace" section in the HRLadder manual for explanations of each item.<br>

1. Click the Edit button on the bottom button bar, then click the Find and Replace button.<br><Br>
    <img src="../_assets/f_btn_edit_en.png" width ="415" ><br>
    <img src="../_assets/f_btn_find_and_change_en.png" width ="500" ><br>
<br>
2. The Find and Replace dialog will appear.<br><br>
<img src="../_assets/find_and_change_dlg_en.png" width = "" ><br>

{% hint style="info" %} To enter text, press the keyboard button below the Replace All button, and use the soft keyboard.

{% endhint %}  
# 3.5 Syntax Check
This function checks if there are any syntax errors in the created ladder diagram.

1. Click the Tool button on the bottom button bar, then click the Check Syntax button.<br><br>
    <img src="../_assets/f_btn_tool_en.png" width ="400" ><br>
    <img src="../_assets/f_btn_chk_syntax_en.png" width ="320" ><br><br>

2. If there are errors, a message will pop up showing the total number of errors, the location of the first error, and its details.<br><br>
    <img src="../_assets/error_message.png" width ="400" ><br><br>
    If there are no errors, a message with the text "No Error" will pop up.<br><br>
    <img src="../_assets/no_error_message.png" width ="400" ><br>
# 3.6 Ladder File
This section explains how to save and load ladder files.# 3.6.2 File Load
Let's verify if the file has been saved correctly using the File Load function.

1. First, press the File > New File button on the bottom button bar to return to the initial state.<br><Br>
    <img src="../../_assets/f_btn_file_en.png" width ="430" ><br>
    <img src="../../_assets/f_btn_new_file_en.png" width ="430" ><br><br>
    <img src="../../_assets/new_file_result_en.png" width ="500" ><br>
    
2. Clicking the Load button will open the file manager screen.<br><br>
    <img src="../../_assets/f_btn_load_file_en.png" width ="430" ><br><br>
    <img src="../../_assets/file_load_screen_en.png" width ="500" ><br><br>

3. Hover over the saved S00.lad file and press the Enter button. You will see the saved file displayed on the current screen.<br>

    {% hint style="info" %}The file load function only supports loading files with the extension .lad or .LAD.
    
    {% endhint %}# 3.6.3 New File
If you want to create a new ladder file or return to the initial state of the ladder editing function, you can use the New File function.

1. Press the File > New File button on the bottom button bar.<br><br>
    <img src="../../_assets/f_btn_file_en.png" width ="430" ><br>
    <img src="../../_assets/f_btn_new_file_en.png" width ="430" ><br><br>
2. This is the result after executing the New File button.<br><br>
    <img src="../../_assets/new_file_result_en.png" width ="600" ><br>
    
3. If you are editing a ladder file and use the New File function, a pop-up will appear asking if you want to save the changes.<br><br>
    <img src="../../_assets/new_file_pop_up_en.png" width ="300" ><br>
    - If you click Yes, you will be taken to the file save screen. If the file is already saved, the changes will be applied to the file.
    - If you click No, the state will change to a new file.
    - If you click Cancel, the new file function will be canceled.

# 4. Monitoring
This section explains the monitoring functions of the ladder diagram.
# 4.1. PLC Monitoring
This function monitors the current relay value status of the robot controller's built-in PLC.<br>

{% hint style="info" %}  
- The monitoring results are the same as in HRLadder, so please refer to the HRLadder manual for more detailed explanations.<br>
- For more information on the built-in PLC operation mode, please refer to the [Hi6 Embedded PLC ManualHi6](https://hrbook-hrc.web.app/#/view/doc-hi6-embedded-plc/korean/2-rc-setting/1-plc-mode-set)

{% endhint %}

1. You can change the built-in PLC's operation mode to Remote Run or Remote Stop by pressing the R.RUN or R.STOP buttons on the bottom button bar.<br><Br>
    <img src="../_assets/f_btn_tool_en.png" width ="430"><br>
    <img src="../_assets/f_btn_remote_en.png" width ="340"><br>

2. When changing the PLC mode to Remote Run, if the S00.lad file is not present in the main/project/lads directory or if the S00.lad file contains syntax errors, the ladder file will not load, and a message saying "No PLC ladder program" will appear. <br><br>
    <img src="../_assets/remote_run_error_en.png" width ="430"><br>

3. If the S00.lad file exists in the main/project/lads directory and there are no syntax errors, the built-in PLC mode will switch to Remote Run, and you will see an icon appear at the top right of the TP screen.<br><br>
    <img src="../_assets/remote_run_header.png" width ="500"><br><br>

4. When the built-in PLC is in STOP or Remote STOP mode, the operand monitoring values will not be displayed.<br><br>
    <img src="../_assets/remote_stop_header.png" width ="500"><br><br>



# 4.2 Checksum Compare
When the built-in PLC is in RUN or Remote Run mode, a checksum comparison function is provided to compare the currently viewed ladder diagram with the file downloaded to the built-in PLC. <br>

1. If the currently viewed ladder diagram is different from the file downloaded to the built-in PLC, a "difference" indicator (<>) will appear next to the title at the top of the monitoring window.<br>
    <img src="../_assets/chksum_diff_state.png" width ="300"><br>

2. If the ladder diagram is the same as the file downloaded to the built-in PLC, a "same" indicator (=) will appear next to the title at the top of the monitoring window.<br>
    <img src="../_assets/chksum_same_state.png" width ="300"><br>

3. You can also directly perform the checksum comparison by pressing the Compare button in the Tools section of the bottom button bar. <br><br>
    <img src="../_assets/f_btn_tool_en.png" width ="400"><br>
    <img src="../_assets/f_btn_compare_en.png" width ="320"><br>

