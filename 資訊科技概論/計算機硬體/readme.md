# 
- 描述電腦硬體的每個元件 ==> 范紐曼型架構  CU ALU Memory I O  BUS
- 3-2 電腦如何表示資料
- 二進位系統（binary system）
- 位元（bit，binary digit 的縮寫）
- 位元組（byte）
- 3-2-2 編碼系統
- ASCII
- Unicode
- 3-2-3 常見的數字系統
- 二進位數字系統(Binary number system)
- 十六進位（hexadecimal number system）數字系統的基底為 16
  - 使用 16 個符號代表數值（hex 表示 16）。使用 0 到 9 之外，十進位的 10 到 15 則是分別用英文字母的 A 到 F 表示。
- 八進位數字系統(Octal Number System)
  - 使用從 0 到 7 一共 8 個數字
  - 最大的數字符號是 7，累積到 8 就進一位。
- 3-2-4 數字系統的轉換
- 3-2-5 負數的表示法
  - 1. 帶符號大小表示法（signed-magnitude）
  - 2. 1’s 補數表示法（1’s complement）
  - 3. 2’s 補數表示法（2’s complement）





## 名詞解釋
- 范紐曼型架構（[Von Neumann architecture](https://en.wikipedia.org/wiki/Von_Neumann_architecture)），也稱馮·紐曼模型（Von Neumann model）或普林斯頓架構（Princeton architecture）
  - A processing unit that contains an arithmetic logic unit and processor registers
  - A control unit that contains an `instruction register` and `program counter`
  - Memory that stores data and instructions
  - External mass storage
  - Input and output mechanisms
- stored-program ==> `instructions(指令)`
  -  instructions(機器指令|第一代程式) ==> 組合語言(機器指令翻成人看得懂的程式語言|第二代程式)
  -  statement| program ==> C (高階語言|第三代程式)
- 機器週期（machine cycle）或指令週期（instruction cycle）
  - 當 CPU 在執行每個指令時，會經過一組 4 個步驟 ==> 機器週期（machine cycle）或指令週期（instruction cycle）
  - 機器週期是由擷取（fetch）、解碼（decode）、執行（execute）和儲存（store） 4 個步驟所組成。
  - 擷取和解碼指令是由控制單元負責
  - 執行和儲存指令則是由 ALU 負責進行。
- 記憶體階層 (Memory hierarchy)
  - 隨機存取記憶體（random access memory, RAM）  vs  唯讀記憶體（read-only memory, ROM）
  - 虛擬記憶體（virtual memory）
  - 置換檔（swap file）分頁檔（paging file）
- 唯讀記憶體（read-only memory, ROM）
  - 永久安裝在電腦，而且是附著在主機板上
  - ROM 晶片內含 BIOS，它負責告訴電腦如何啟動。
  - BIOS 也會進行所謂的開機自我檢測（power-on self test, POST），這道程序會測試電腦的全部元件是否能正常運作
  - 電腦廠商會時常更新 ROM 晶片上的指令，也稱作`韌體（firmware）`
- 處理器的`時脈速度（clock speed）`
  - 測量它能以多快的速度執行指令。
  - 時脈速度可以用 MHz（megahertz，百萬赫茲）或 GHz（gigahertz，十億赫茲）為單位。
  - 百萬赫茲是每秒百萬次時脈週期，而十億赫茲則是每秒十億次時脈週期。
- 一個`時脈週期（cycle）`
  - 是測量處理程序（process）的最小時間單位。
  - CPU 的效率則是以每個時脈週期能執行的指令個數（instructions per cycle, IPC）為單位。
- BUS
  - 匯流排的速度和寬度是影響電腦效能的另一個重要因素。
  - 匯流排是一種能讓 CPU 與電腦內部或外接的各種裝置相互通訊的電子通道。
  - 匯流排寬度（bus width）會決定資料傳輸的速度，它也被稱為字組大小（word size）。
- 不斷電電源供應器（uninterruptable power supply, UPS） 
- 突波抑制器（surge suppressor） 









  
## 研究所必考 ==> 計算機組織與架構
- [計算機組織與設計 : 硬體/軟體的介面, 5/e ](https://www.tenlong.com.tw/products/9789574838110)
- Patterson: Computer Organization and Design: The Hardware/Software Interface, 5/e
- David A. Patterson , John L. Hennessy 著、鍾崇斌、楊惠親 譯
