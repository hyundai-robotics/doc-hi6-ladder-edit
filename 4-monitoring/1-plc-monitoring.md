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