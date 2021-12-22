# 
- 描述電腦硬體的每個元件 ==> 范紐曼型架構  CU ALU Memory I O  BUS
- 
- 
- 
- 


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

 
  - 





  
## 研究所必考 ==> 計算機組織與架構
- [計算機組織與設計 : 硬體/軟體的介面, 5/e ](https://www.tenlong.com.tw/products/9789574838110)
- Patterson: Computer Organization and Design: The Hardware/Software Interface, 5/e
- David A. Patterson , John L. Hennessy 著、鍾崇斌、楊惠親 譯
