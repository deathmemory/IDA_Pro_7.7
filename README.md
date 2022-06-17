# IDA_Pro_7.7

2022/03/26 更新

1. 更新了部分插件
2. 新增了 BinDiff（程序本體需手動安裝） 和 ret-sync 插件
3. 新增了 BinCAT 插件，需要手動導入腳本安裝
4. 新增了 diaphora 腳本，每次使用都需要手動導入
5. 修改了說明文檔

------------------------------------------------------------------------------

2022/02/15 更新

1. 新增了 patching 插件，用來替代 Keypatch（依然保留）
2. 修復了 LazyIDA 的 Bug，沒下載過的可以不用下載附件了
3. 更新了綠化工具

------------------------------------------------------------------------------

IDA Pro 7.7.220118 (SP1) 綠色版由 Binwalker 基於 Think-Cell Operations GmbH 公司泄露版本和 TOM_RUS 的 Keygen 方案制作，包含全套 Hex-Rays Decompiler 插件（部分為老版本添加而來），解壓後運行【IDA_InitTool.exe】即可一鍵綠化，默認配置為綠色版 Python 3.8.10

## 【需要注意】
  1. 路徑不能含有中文
  2. 使用綠色版 Python 安裝插件的時，務必使用【-m】參數來指定以導入模塊方式運行 pip，如：python.exe -m pip install + 包名
  3. IDA 下的【idapyswitch.exe】可以切換 Python 版本，但請注意切換到非綠色版 Python 後需要自行安裝插件所需的依賴
  4. IDA 下的【SDK77.7z】為 IDA 7.7 SDK
  5. IDA 下的【Kengen.7z】為 IDA Key 生成程序
  6. IDA 下的【msdia140.dll】、【symsrv.dll】和【symsrv.yes】以及 IDA/plugins 下的【pdb.dll】和【pdb64.dll】用於 PDB 修復增強，如有問題可刪除，其中【pdb.dll.bak】和【pdb64.dll.bak】為原程序的備份
  7. IDA/plugins 下的【BinCAT/install_plugin.py】為 BinCAT 插件的安裝腳本，需要手動在 IDA 中導入腳本安裝
  8. IDA/plugins 下的【bindiff7.msi】為 BinDiff 安裝程序，可選安裝，安裝後可配合其插件使用
  9. IDA/plugins 下的【diaphora/diaphora.py】為 diaphora 插件的腳本，每次使用都需要手動在 IDA 中導入

## 【修改說明】
###  1. 增加了一些常用插件
      BinCAT
      diaphora
      patching
      ret-sync
      Auto Re
      BinDiff
      Findcrypt
      IDA Signsrch
      Keypatch
      LazyIDA
      StrongCC

###  2. 修改了一些默認配置
      cfg/ida.cfg
          增加：
              GB2312: Chinese
          修改：
              STORE_USER_INFO = YES --> NO
              OPCODE_BYTES = 0 --> 10
              INDENTION = 16 --> 0
              MAX_DATALINE_LENGTH = 70 --> 100
              SHOW_BASIC_BLOCKS = NO --> YES
              SHOW_XREFS = 2 --> 15
              SHOW_SOURCE_LINNUM = NO --> YES
      cfg/Chinese.clt
          增加：
              u2000..u206F,
              u3000..u303F,
###  3.  IDA DLL 修改
        ida.dll
            0027AA97 10 --> 00
            00383CF3 5C --> C8
        ida64.dll
            00283695 10 --> 00
            0038CE63 5C --> C8

### ※ 由 Binwalker 制作綠化工具，功能包含：綠化 Python 3.8.10、禁用 IDA 自動聯網、設置 IDA 桌面快捷方式
### ※ 僅作學習交流使用，不得用於商業或者非法用途，請測試後盡快刪除，購買正版進行支持


### Download:　https://www.asuswebstorage.com/navigate/a/#/s/C544E0CA37B34DC3AD94BA6BC73D97D5Y
