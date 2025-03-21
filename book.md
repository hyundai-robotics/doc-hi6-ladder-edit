# Hi6 로봇제어기 기능설명서 - 래더 편집 (Ladder Edit)

{% hint style="warning" %}
본 제품 설명서에서 제공되는 정보는 현대로보틱스의 자산입니다.

현대로보틱스의 서면에 의한 동의 없이 전부 또는 일부를 무단 전재 및 재배포할 수 없으며, 제3자에게 제공되거나 다른 목적에 사용할 수 없습니다.



본 설명서는 사전 예고 없이 변경될 수 있습니다.



**Copyright ⓒ 2025 by Hyundai Robotics**
{% endhint %}
# 1. 개요

{% hint style="info" %}
본 기능은 V60.32-00 및 이후 버전부터 지원됩니다.
{% endhint %}# 1.1 래더 편집(Ladder Edit)

Hi6 제어기의 래더 편집(Ladder Edit) 기능은 Hi6 내장 PLC를 통해 구동할 래더 프로그램을 사용자가 직접 작성 및 편집할 수 있는 Hi6 제어기 내장 기능입니다.

편집 방식은 현대로봇 전용의 래더 편집 PC 소프트웨어인 HRLadder와 유사하므로 이미 HRLadder를 사용하여 래더 프로그램을 편집해 본 경험이 있는 사용자들은 본 설명서를 통해 빠르게 기능을 익힐 수 있을 것 입니다. 

* HRLadder는 현대로보틱스 웹사이트(https://www.hd-hyundairobotics.com/main) - 고객지원 - 다운로드 센터에서 HRLadder를 검색하여 다운로드 하실 수 있습니다.
* HRLadder의 사용법은 HRLadder의 도움말 메뉴에 연결된 기능설명서를 참조하십시오.


{% hint style="info" %} Hi6 제어기 설정, 릴레이, 내장 PLC에 대한 설명은 [Hi6 내장 PLC 설명서](https://hrbook-hrc.web.app/#/view/doc-hi6-embedded-plc/korean/README) 를 참조하시기 바랍니다.

{% endhint %}  
# 2. 래더 편집 시작
래더 편집 기능의 위치 및 실행하기 위한 과정을 설명드립니다.# 2.1. 초기 화면
래더 편집 기능을 실행해보겠습니다.

1. 화면 우측의 [창조정] 버튼과 하단의 [분할] 버튼을 터치한 후 왼쪽 하단의 [선택] 버튼까지 순서대로 터치 하십시오. 패널 선택창이 나타납니다.<br><br>
    <img src="../_assets/split_window.png" width="600">
    <br><br>

2. 패널 선택창에서 래더 편집을 선택합니다.<br><br>
<img src="../_assets/select_panel.png" width="600"><br><br>
3. 래더 편집 기능이 시작됩니다.<br><br>
하단 버튼바가 아래와 같은 형태가 아닌 경우 ESC 버튼을 누르십시오.
<br><br>
<img src="../_assets/f_btn_screen.png" width="600"><br><br>
하단의 버튼을 통해 다양한 기능을 사용할 수 있습니다. 
<br><br><br>

버튼별 기능들에 대한 설명입니다.<br>
<table text-align: center; style="tg">
    <tr>
        <th colspan = 3 style="text-align: center;"> 버튼</th>
        <th style="text-align: center;">기능 </th>
    </tr>
    <tr>
        <td colspan = 3> 파일</td>
        <td > 파일 불러오기, 저장하기 등 파일 관련 기능 </td>
    </tr>
    <tr>
        <td colspan = 3>편집</td>
        <td>실행 취소, 복사, 붙여넣기, 찾기/바꾸기 등 편집 기능</td>
    </tr>
    <tr>
        <td colspan = 3>보기</td>
        <td>전체화면, 브랜치 간격, 태그 형식 등 화면 확인 관련 기능</td>
    </tr>
    <tr>
        <td colspan = 3>삽입</td>
        <td>삽입 가능한 모든 요소들</td>
    </tr>
    <tr>
        <td colspan = 3>도구</td>
        <td>문법검사, 비교, Remote RUN/STOP 등 PLC 모니터링 관련 기능</td>
    </tr>
</table>

# 3. 래더 다이어그램 편집
래더 다이어그램의 편집에 대해서 설명드립니다.# 3.1 요소 삽입
래더 다이어그램을 편집하는 방식은 HRLadder의 편집 방식과 유사하므로 더 자세한 설명은 HRLadder 설명서의 기본 편집 항목을 확인하여 주십시오. 

1. 모든 요소의 삽입은 하단 버튼 바의 삽입 버튼을 통해 확인하실 수 있습니다.<br><br>
    <img src="../_assets/f_btn_insert.png" width ="355" ><br>
    <img src="../_assets/f_btn_elements.png" width ="500" ><br><br>

2. 다른 요소들을 확인하고 싶다면 이전/다음 버튼을 터치하시면 됩니다.<br><br>
    <img src="../_assets/insert_move_next_prev.png" width ="500" ><br><br>
# 3.2 편집 기능
다른 편집 기능들도 HRLadder의 기능과 동일합니다.<br>
더 자세한 편집 방법은 HRLadder 설명서의 래더 다이어그램 편집 항목을 확인해 주십시오.
1. 브랜치 편집을 쉽게 하기 위한 브랜치 간격 옵션입니다.<br>
    하단 버튼 바 보기 버튼을 누른 후 브랜치 간격 버튼을 누르시면 됩니다.<br><br>
    <img src="../_assets/f_btn_layout.png" width ="415" ><br>
    <img src="../_assets/f_btn_branch_gap.png" width ="250" ><br><br>
2. 잘라내기, 복사, 붙여넣기, 실행 취소, 다시 실행 기능은 하단 버튼 바 편집을 누르면 확인하실 수 있습니다.<br><br>
    <img src="../_assets/f_btn_edit.png" width ="415"><br>
    <img src="../_assets/f_btn_edit_menu.png" width ="500"><br><br>

3. [Del]키를 누르면 선택된 명령어들, 혹은 선택된 Rung 이나 브랜치가 삭제됩니다.<br><br>
# 3.3 태그형식
릴레이 인덱스 중 1비트 데이터는 1 비트, 8비트, 16비트, 32비트 4가지 형식 중 하나로 입력하고 표시될 수 있습니다.<br>
{% hint style="info" %}릴레이 표기에 대한 자세한 설명은 
[Hi6 내장 PLC 릴레이의 표기 설명서 ](https://hrbook-hrc.web.app/#/view/doc-hi6-embedded-plc/korean/3-relay/2-relay-expression)를 참고해 주십시오 
{% endhint %}
<br>
래더 편집 기능에서는 HRLadder와 동일한 방식으로 4가지 형식 중 1가지를 선택하여 래더 다이어그램에 보여주는 기능을 가지고 있습니다.<br>

1. 보기 버튼을 누른후 태그형식 버튼을 누릅니다. <br><br>
<img src="../_assets/f_btn_layout.png" width ="415"><br>
<img src="../_assets/f_btn_tag_format.png" width ="250"><br>

2. 태그형식 버튼을 누를 때 마다, 표시 형식은 1비트 -> 8비트 -> 16비트 -> 32비트로 순환합니다.# 3.4 찾기 및  바꾸기
래더 파일의 전체를 검색하여 지정한 문자열을 찾아내거나 찾은 문자열을 지정한 다른 문자열로 바꾸는 기능입니다.<br>

HRLadder와 동일한 기능이기에 각 항목들에 대한 설명은 HRLadder 설명서의 찾기와 바꾸기 항목을 참고해 주십시오.<br>

1. 하단 버튼바 편집 > 찾기 및 바꾸기 버튼을 클릭하면<br><Br>
    <img src="../_assets/f_btn_edit.png" width ="415" ><br>
    <img src="../_assets/f_btn_find_and_change.png" width ="500" ><br>
<br>
2. 찾기 및 바꾸기 대화상자가 나타납니다.<br><br>
<img src="../_assets/find_and_change_dlg.png" width = "" ><br>

{% hint style="info" %}문자 입력은 전부 바꾸기 버튼 아래의 키보드 버튼을 누른 후 소프트 키보드를 사용하시면 됩니다.

{% endhint %}  
# 3.5 문법 검사
작성된 래더 다이어그램이 문법적으로 틀린 곳이 없는 지 체크하는 기능입니다.

1. 하단 버튼 바 도구 > 문법 검사 버튼을 클릭하십시오.<br><br>
    <img src="../_assets/f_btn_tool.png" width ="400" ><br>
    <img src="../_assets/f_btn_chk_syntax.png" width ="320" ><br><br>

2. 에러가 존재한다면 에러 총 갯수와 첫 에러의 위치 및 내용이 담긴 메시지가 팝업됩니다.<br><br>
    <img src="../_assets/error_message.png" width ="400" ><br><br>
    만약 에러가 없다면 "No Error" 라는 문구가 담긴 메시지가 팝업됩니다.<br><br>
    <img src="../_assets/no_error_message.png" width ="400" ><br>
# 3.6 래더 파일
파일 저장 및 불러오는 방법에 대한 설명입니다.
# 3.6.1 파일 저장하기
래더 파일을 저장하는 방법입니다.

1.  하단 버튼 바 파일 > 저장하기 버튼을 누릅니다.<br>
    <img src="../../_assets/f_btn_file.png" width ="430" ><br>
    <img src="../../_assets/f_btn_save.png" width ="430" ><br>
    
2. 만약 문법 오류가 없다면 하단의 파일이름을 입력할 수 있는 입력창이 있는 파일 관리자 화면이 나타납니다.<br><br>
    <img src="../../_assets/file_save_intro.png" width ="500" ><br>
    - 1번 항목은 파일 디렉토리 항목이며 저장 될 디렉토리를 설정할 수 있습니다.
    - 2번 항목은 파일 디렉토리 내부의 파일 리스트 입니다. 
    - 3번 항목은 파일 이름 입력창으로 저장될 파일의 이름을 입력할 수 있습니다.
3. 파일 이름 입력창에 래더 파일 이름 형식에 맞추어 S00 으로 이름을 입력한 후 Enter 버튼을 눌러 저장을 완료하겠습니다.<br><br> 
    <img src="../../_assets/file_save_name_edit.png" width ="500" ><br><br>
    {% hint style="info" %}
    현재 포커스된 커서가 디렉토리 인 경우 Enter 버튼을 눌러도 저장되지 않습니다. 2번, 3번 항목에 커서를 둔 채로 Enter 버튼을 눌러야 저장이 됩니다.
    {% endhint %}
4. 만약 현재 파일을 다른 이름으로 저장하고 싶다면 하단 버튼 바 파일 > 다른 이름 저장 버튼을 통해 현재 래더 파일의 내용을 다른 이름으로 저장할 수 있습니다.<br><br>

5. 래더 번호 저장 버튼을 누르면 S{래더번호}{부가 설명} 형태의 파일이름이 파일 이름 입력창에 기록된 파일 관리자 화면이 나타납니다. <br><br>
    <img src="../../_assets/file_save_name_edit.png" width ="500" ><br>
    
    (현재 저장하고자 하는 래더파일이 래더 파일 이름 형식에 맞지 않다면 S00으로 파일이름이 지정됩니다.)
# 3.6.2 파일 불러오기
파일 불러오기 기능을 통해 저장한 파일이 잘 저장되었는지 확인해보겠습니다.

1. 먼저 하단 버튼 바 파일 > 새 파일 버튼을 통해 초기 상태로 돌아가겠습니다.<br><Br>
    <img src="../../_assets/f_btn_file.png" width ="430" ><br>
    <img src="../../_assets/f_btn_new_file.png" width ="430" ><br><br>
    <img src="../../_assets/new_file_result.png" width ="500" ><br>
    
2. 불러오기 버튼을 클릭하면 파일 관리자 화면이 나타납니다.<br><br>
    <img src="../../_assets/f_btn_load_file.png" width ="430" ><br><br>
    <img src="../../_assets/file_load_screen.png" width ="500" ><br><br>

3. 저장한 S00.lad 파일에 커서를 두고 Enter 버튼을 누르면 현재 화면에 저장한 파일이 출력되는 것을 확인할 수 있습니다.<br>

    {% hint style="info" %}파일 불러오기 기능을 통해서 확장자가 lad 혹은 LAD 인 파일만 불러올 수 있습니다.
    
    {% endhint %}# 3.6.3 새 파일
새로운 래더 파일을 만들고 싶거나 초기 상태의 래더 편집 기능으로 돌아가고 싶은 경우 새 파일 기능을 사용할 수 있습니다. 

1. 하단 버튼 바의 파일 > 새 파일 버튼을 눌러보겠습니다.<br><br>
    <img src="../../_assets/f_btn_file.png" width ="430" ><br>
    <img src="../../_assets/f_btn_new_file.png" width ="430" ><br><br>
2. 새 파일 버튼을 실행한 결과 입니다.<br><br>
    <img src="../../_assets/new_file_result.png" width ="600" ><br>
    
3. 만약 래더 파일을 수정하던 중 새파일 기능을 사용하는 경우 변경 사항 저장 여부를 확인하는 팝업이 생성됩니다.<br><br>
    <img src="../../_assets/new_file_pop_up.png" width ="300" ><br>
    - 예를 누르게 되면 파일 저장 화면으로 이동됩니다. 이미 저장된 파일인 경우 변경 사항이 파일에 적용됩니다.
    - 아니요를 누르게 되면 새 파일 상태가 됩니다.
    - 취소를 누르게 되면 새파일 기능 호출이 취소됩니다.

# 4. 모니터링
래더 다이어그램의 모니터링 기능에 대해서 설명드립니다.# 4.1. PLC 모니터링
로봇제어기의 내장 PLC의 현재 릴레이값 상태를 모니터링 하는 기능입니다.<br>

{% hint style="info" %}  
- 모니터링 결과는 HRLadder와 동일하므로 자세한 설명은 HRLadder 설명서를 참고해 주십시오.<br>
- 내장 PLC 동작 모드에 대한 자세한 설명은 [Hi6 내장 PLC 설명서](https://hrbook-hrc.web.app/#/view/doc-hi6-embedded-plc/korean/2-rc-setting/1-plc-mode-set)를  참고해 주십시오.  
{% endhint %}

1. 하단 버튼 바 도구 > R.RUN 혹은 R.STOP 버튼을 통해 내장 PLC의 동작모드를 Remote Run 혹은 Remote Stop 상태로 변경할 수 있습니다.<br><Br>
    <img src="../_assets/f_btn_tool.png" width ="430"><br>
    <img src="../_assets/f_btn_remote.png" width ="340"><br>

2. Remote Run 상태로 PLC 모드를 변경하는 할 때. S00.lad 파일이 main의 project/lads 디렉토리 내에 없거나 S00.lad 파일에 문법적 오류가 있는 경우 래더 파일이 로드 되지 않아 "PLC 프로그램 없음" 이라는 메시지를 출력합니다. <br><br>
    <img src="../_assets/remote_run_error.png" width ="430"><br>

3. 만약 문법적 오류가 없는 S00.lad 파일이 main의 project/lads 경로에 존재한다면 내장 PLC 모드는 Remote Run으로 변경되며 TP화면 우측 상단에 아이콘이 생기는 것을 볼 수 있습니다.<br><br>
    <img src="../_assets/remote_run_header.png" width ="500"><br><br>

4. 내장 PLC가 STOP 혹은 Remote STOP인 상태에서는 오퍼랜드의 모니터링 값이 표시되지 않습니다.<br><br>
    <img src="../_assets/remote_stop_header.png" width ="500"><br><br>



# 4.2 체크섬 비교
내장 PLC가 RUN 혹은 Remote Run 상태인 경우, 현재 확인 중인 래더 다이어그램과 내장 PLC에 다운로드된 파일을 비교해주는 체크섬 비교 기능을 제공합니다. <br>

1. 만약 현재 확인 중인 래더 다이어그램이 내장 PLC에 다운로드 된 파일과 다르다면 모니터링 창 상단 제목 옆에는 다르다는 표시(<>) 가 표시됩니다.<br>
    <img src="../_assets/chksum_diff_state.png" width ="300"><br>

2. 래더 다이어그램이 내장 PLC에 다운로드된 파일과 같다면 그림 4.7과 같이 같다는 표시 (=) 가 표시됩니다.<br>
    <img src="../_assets/chksum_same_state.png" width ="300"><br>

3. 하단 버튼 바 도구 > 비교 버튼을 통해서도 직접 체크섬 비교가 가능합니다. <br><br>
    <img src="../_assets/f_btn_tool.png" width ="400"><br>
    <img src="../_assets/f_btn_compare.png" width ="320"><br>

