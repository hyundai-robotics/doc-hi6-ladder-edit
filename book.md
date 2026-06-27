
[__SOURCE](README.md)
# ${cont_model} 控制器功能手册 - 梯形编辑
[__SOURCE](0-about-this-manual/README.md)
# 关于手册
[__SOURCE](0-about-this-manual/precautions.md)
# 注意事项

{% include file="zh/precautions.md" %}
[__SOURCE](0-about-this-manual/safety-notice.md)
# 安全注意事项

{% include file="zh/safety-notice.md" %}
[__SOURCE](1-intro/README.md)
# 1. 介绍

{% hint style="info" %}此功能在版本 V60.32-00及之后的版本中支持。

{% endhint %}
[__SOURCE](1-intro/1-ladder-edit.md)
# 1.1 梯形编辑

${cont_model} 控制器的梯形编辑功能是一个嵌入式特性，允许用户直接创建和编辑 ${cont_model} 内置 PLC 的梯形程序。

编辑方法类似于 HRLadder，这是用于 HD Hyundai Robotics 的专用梯形编辑 PC 软件。因此，具有使用 HRLadder 编辑梯形程序经验的用户将能够通过本手册快速熟悉此功能。

- HRLadder 可以通过在 HD Hyundai Robotics 网站（https://www.hd-hyundairobotics.com/main）上搜索下载 - 客户支持 - 下载中心。
- 有关如何使用 HRLadder 的说明，请参考 HRLadder 帮助菜单中链接的用户手册。

{% hint style="info" %} 有关 ${cont_model} 控制器设置、继电器和内置 PLC 的信息，请参考 [ ${cont_model} 嵌入式 PLC 手册](https://hrbook-hrc.web.app/#/view/doc-hi6-embedded-plc/zh/README?cont_model=${cont_model}) 

{% endhint %}  
[__SOURCE](2-ladder-edit-start/README.md)
# 2. 启动梯形图编辑
本节解释了执行梯形图编辑功能的位置和过程。
[__SOURCE](2-ladder-edit-start/1-initial_screen.md)
# 2.1. 初始屏幕
让我们执行梯形图编辑功能。

1. 点击屏幕右侧的 [pane Layout] 按钮和底部的 [split] 按钮。然后，点击拆分监控窗口，接着点击左下角的 [select] 按钮。面板选择窗口将出现。<br><br>
    <img src="../_assets/split_window_en.png" width="600">
    <img src="../_assets/split_window2_en.png" width="600">
    <br><br>

2. 在面板选择窗口中选择编辑梯形图。<br><br>
<img src="../_assets/select_panel_en.png" width="600"><br><br>

3. 梯形图编辑功能将开始。<br><br>
如果底部按钮条未显示如下所示的形式，请按 ESC 按钮。
<br><br>
<img src="../_assets/f_btn_screen_en.png" width="600"><br><br>
您可以通过底部的按钮使用各种功能。
<br><br><br>

以下是每个按钮功能的说明。<br>
<table text-align: center; style="tg">
    <tr>
        <th colspan = 3 style="text-align: center;"> 按钮</th>
        <th style="text-align: center;"> 功能 </th>
    </tr>
    <tr>
        <td colspan = 3> 文件</td>
        <td > 与文件相关的功能，例如加载和保存文件。 </td>
    </tr>
    <tr>
        <td colspan = 3> 编辑</td>
        <td> 编辑功能，例如撤销、复制、粘贴、查找/替换等。</td>
    </tr>
    <tr>
        <td colspan = 3> 布局</td>
        <td> 与屏幕相关的功能，例如全屏模式、分支间距、标签格式等。</td>
    </tr>
    <tr>
        <td colspan = 3> 插入</td>
        <td> 可以插入的所有元素。</td>
    </tr>
    <tr>
        <td colspan = 3> 工具</td>
        <td> 与 PLC 监控相关的功能，例如语法检查、比较、远程运行/停止等。</td>
    </tr>
</table>
[__SOURCE](3-ladder-diagram-edit/README.md)
# 3. 梯形图编辑
本节解释梯形图的编辑。
[__SOURCE](3-ladder-diagram-edit/1-insert-element.md)
# 3.1 插入元素
编辑梯形图的方法类似于HRLadder的编辑方法，因此有关更详细的说明，请参阅HRLadder手册中的基本编辑部分。

1. 所有元素的插入可以通过底部按钮栏上的插入按钮访问。<br><br>
    <img src="../_assets/f_btn_insert_en.png" width ="355" ><br>
    <img src="../_assets/f_btn_elements.png" width ="500" ><br><br>

2. 要检查其他元素，您可以触摸上一个/下一个按钮。<br><br>
    <img src="../_assets/insert_move_next_prev_en.png" width ="500" ><br><br>
[__SOURCE](3-ladder-diagram-edit/2-editing-features.md)
# 3.2 编辑功能
其他编辑功能与 HRLadder 中的功能相同。<br>
有关更详细的编辑说明，请参阅 HRLadder 手册中的梯形图编辑部分。
1. 分支间隔选项使编辑分支更加容易。<br>
    按下底部按钮栏中的查看按钮，然后按分支间隔按钮。<br><br>
    <img src="../_assets/f_btn_layout_en.png" width ="415" ><br>
    <img src="../_assets/f_btn_branch_gap_en.png" width ="250" ><br><br>
2. 剪切、复制、粘贴、撤消和重做功能可以通过按底部按钮栏中的编辑按钮访问。<br><br>
    <img src="../_assets/f_btn_edit_en.png" width ="415"><br>
    <img src="../_assets/f_btn_edit_menu_en.png" width ="500"><br><br>

3. 按 [SHIFT]+[DEL] 键删除选定的指令，或选定的梯步或分支。
<br><br>
[__SOURCE](3-ladder-diagram-edit/3-tag-format.md)
# 3.3 标签格式
继电器索引中的 1 位数据可以以四种格式之一输入和显示：1 位、8 位、16 位或 32 位。<br>
{% hint style="info" %}有关继电器表示法的更多详细信息，请参阅 [${cont_model} 嵌入式 PLC 继电器表示法手册](https://hrbook-hrc.web.app/#/view/doc-hi6-embedded-plc/zh/3-relay/2-relay-expression?cont_model=${cont_model})

{% endhint %}
<br>
在梯形图编辑功能中，您可以选择四种格式之一，并以与 HRLadder 相同的方式在梯形图上显示。<br>

1. 按下布局按钮，然后按下标签格式按钮。 <br><br>
<img src="../_assets/f_btn_layout_en.png" width ="415"><br>
<img src="../_assets/f_btn_tag_format_en.png" width ="250"><br>

2. 每次按下标签格式按钮时，显示格式循环通过 1 位 -> 8 位 -> 16 位 -> 32 位。
[__SOURCE](3-ladder-diagram-edit/4-find-and-replace.md)
# 3.4 查找和替换
此功能允许您在整个梯形图文件中搜索指定字符串或将找到的字符串替换为另一个指定字符串。<br>

由于此功能与 HRLadder 中的相同，因此请参考 HRLadder 手册中的“查找和替换”部分，以获取每个项目的说明。<br>

1. 点击底部按钮栏上的编辑按钮，然后点击查找和替换按钮。<br><Br>
    <img src="../_assets/f_btn_edit_en.png" width ="415" ><br>
    <img src="../_assets/f_btn_find_and_change_en.png" width ="500" ><br>
<br>
2. 查找和替换对话框将出现。<br><br>
<img src="../_assets/find_and_change_dlg_en.png" width = "" ><br>

{% hint style="info" %} 要输入文本，请按下替换全部按钮下方的键盘按钮，并使用软键盘。

{% endhint %}  
[__SOURCE](3-ladder-diagram-edit/5-syntax-check.md)
# 3.5 语法检查
此功能检查创建的梯形图中是否存在语法错误。

1. 点击底部按钮栏上的工具按钮，然后点击检查语法按钮。<br><br>
    <img src="../_assets/f_btn_tool_en.png" width ="400" ><br>
    <img src="../_assets/f_btn_chk_syntax_en.png" width ="320" ><br><br>

2. 如果有错误，将弹出一条信息，显示错误的总数、第一个错误的位置及其详细信息。<br><br>
    <img src="../_assets/error_message.png" width ="400" ><br><br>
    如果没有错误，将弹出一条文本为"No Error"的信息。<br><br>
    <img src="../_assets/no_error_message.png" width ="400" ><br>
[__SOURCE](3-ladder-diagram-edit/6-file/README.md)
# 3.6 梯形图文件
本节解释如何保存和加载梯形图文件。
[__SOURCE](3-ladder-diagram-edit/6-file/1-file-save.md)
# 3.6.1 文件保存
本节解释如何保存梯形图文件。

1.  按下底部按钮栏上的 文件 > 保存 按钮。<br><br>
    <img src="../../_assets/f_btn_file_en.png" width ="430" ><br>
    <img src="../../_assets/f_btn_save_en.png" width ="430" ><br>
    
2. 如果没有语法错误，将出现一个文件管理器屏幕，提供输入文件名的文本字段。<br><br>
    <img src="../../_assets/file_save_intro_en.png" width ="500" ><br>
    - 项目 1 是文件目录部分，您可以设置将要保存文件的目录
    - 项目 2 是目录中文件的列表。
    - 项目 3 是文件名输入字段，在此您可以输入要保存的文件名。
3. 在文件名输入字段中，以 S00 格式输入梯形图文件名，然后按 Enter 按钮完成保存。<br><br> 
    <img src="../../_assets/file_save_name_edit_en.png" width ="500" ><br><br>
    {% hint style="info" %}
    如果光标集中在目录字段，按 Enter 按钮将不会保存文件。必须在光标集中在项目 2 或项目 3 时按下 Enter 按钮才能保存文件。
    
    {% endhint %}
4. 如果您想用不同的名称保存当前文件，可以使用底部按钮栏上的 文件 > 另存为 按钮，以不同的名称保存当前梯形图文件。<br><br>

5. 按下梯形图编号保存按钮将显示文件管理器屏幕，文件名输入字段中的文件名格式为 S{Ladder Number}{Additional Description}。<br><br>
    <img src="../../_assets/file_save_name_edit_en.png" width ="500" ><br>
    
    (如果梯形图文件名不符合要求的格式，则文件名将设置为 S00。)
[__SOURCE](3-ladder-diagram-edit/6-file/2-file-load.md)
# 3.6.2 文件加载
让我们验证文件是否已通过文件加载功能正确保存。

1. 首先，按下底部按钮栏上的 文件 > 新文件 按钮以返回初始状态。<br><Br>
    <img src="../../_assets/f_btn_file_en.png" width ="430" ><br>
    <img src="../../_assets/f_btn_new_file_en.png" width ="430" ><br><br>
    <img src="../../_assets/new_file_result_en.png" width ="500" ><br>
    
2. 点击加载按钮将打开文件管理器屏幕。<br><br>
    <img src="../../_assets/f_btn_load_file_en.png" width ="430" ><br><br>
    <img src="../../_assets/file_load_screen_en.png" width ="500" ><br><br>

3. 将鼠标悬停在保存的 S00.lad 文件上并按下回车按钮。您将在当前屏幕上看到保存的文件显示。<br>

    {% hint style="info" %}文件加载功能仅支持加载扩展名为 .lad 或 .LAD 的文件
    
    {% endhint %}
[__SOURCE](3-ladder-diagram-edit/6-file/3-new-file.md)
# 3.6.3 新文件
如果您想创建一个新的梯形文件或返回梯形编辑功能的初始状态，可以使用新文件功能。

1. 按下底部按钮栏上的文件 > 新文件按钮。<br><br>
    <img src="../../_assets/f_btn_file_en.png" width ="430" ><br>
    <img src="../../_assets/f_btn_new_file_en.png" width ="430" ><br><br>
2. 这是执行新文件按钮后的结果。<br><br>
    <img src="../../_assets/new_file_result_en.png" width ="600" ><br>
    
3. 如果您正在编辑一个梯形文件并使用新文件功能，将出现一个弹出窗口，询问您是否要保存更改。<br><br>
    <img src="../../_assets/new_file_pop_up_en.png" width ="300" ><br>
    - 如果您点击是，您将进入文件保存屏幕。如果文件已经保存，更改将应用于文件。
    - 如果您点击否，状态将更改为新文件。
    - 如果您点击取消，新文件功能将被取消。
[__SOURCE](4-monitoring/README.md)
# 4. 监控
本节解释梯形图的监控功能。
[__SOURCE](4-monitoring/1-plc-monitoring.md)
# 4.1. PLC 监控
该功能监控机器人控制器内置PLC的当前继电器值状态。<br>

{% hint style="info" %}  
- 监控结果与HRLadder中的结果相同，因此请参考HRLadder手册以获取更详细的解释。<br>
- 有关内置PLC操作模式的更多信息，请参阅[${cont_model} 嵌入式PLC手册](https://hrbook-hrc.web.app/#/view/doc-hi6-embedded-plc/zh/2-rc-setting/1-plc-mode-set?cont_model=${cont_model})

{% endhint %}

1. 您可以通过按下底部按钮栏上的R.RUN或R.STOP按钮，将内置PLC的操作模式更改为远程运行或远程停止。<br><Br>
    <img src="../_assets/f_btn_tool_en.png" width ="430"><br>
    <img src="../_assets/f_btn_remote_en.png" width ="340"><br>

2. 当将PLC模式更改为远程运行时，如果在main/project/lads目录中没有S00.lad文件，或者S00.lad文件包含语法错误，则梯形图文件将无法加载，并将出现“没有PLC梯形图程序”的消息。<br><br>
    <img src="../_assets/remote_run_error_en.png" width ="430"><br>

3. 如果在main/project/lads目录中存在S00.lad文件且没有语法错误，则内置PLC模式将切换到远程运行，您将在TP屏幕的右上角看到一个图标出现。<br><br>
    <img src="../_assets/remote_run_header.png" width ="500"><br><br>

4. 当内置PLC处于STOP或远程STOP模式时，将不会显示操作数监控值。<br><br>
    <img src="../_assets/remote_stop_header.png" width ="500"><br><br>
[__SOURCE](4-monitoring/2-checksum-compare.md)
# 4.2 校验和比较
当内置 PLC 处于运行或远程运行模式时，提供校验和比较功能，以将当前查看的梯形图与下载到内置 PLC 的文件进行比较。 <br>

1. 如果当前查看的梯形图与下载到内置 PLC 的文件不同，则监控窗口顶部标题旁边会出现“差异”指示器 (<>)。<br>
    <img src="../_assets/chksum_diff_state.png" width ="300"><br>

2. 如果梯形图与下载到内置 PLC 的文件相同，则监控窗口顶部标题旁边会出现“相同”指示器 (=)。<br>
    <img src="../_assets/chksum_same_state.png" width ="300"><br>

3. 您还可以通过按下底部按钮栏的工具部分中的比较按钮直接执行校验和比较。 <br><br>
    <img src="../_assets/f_btn_tool_en.png" width ="400"><br>
    <img src="../_assets/f_btn_compare_en.png" width ="320"><br>