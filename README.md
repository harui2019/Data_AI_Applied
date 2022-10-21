# Data_AI_Applied

國立政治大學 National ChengChi University
1111_701893001/751842001_人工智慧應用專題
個人課程作業存放處

---

## Usage

- 將每週的jupyter notebook上傳至colab，並將同層資料夾的隨附檔案上傳至kernel所在儲存空間應即可使用。

---

## Environment

- 所有jupyter notebook皆編輯並運行於 **Python 3.9.7** installed by **Anaconda** on **Ubuntu 20.04/22.04 LTS**.
- 如用低於 **Python 3.9.7** (**< Python 3.9.7**) 可能會有版本不相容的問題
- 所有jupyter notebook的開頭都應有環境檢查，用以確認是否為Colab並準備環境，如下列

    ```python
    ### [1] - 建立環境用的指令
    cmdLineForColab = [
        "pip install jieba"
    ]

    ### [2] - 檢查環境如果，是Colab則運行安裝
    import os
    try: 
        from google.colab import drive
        print("Running on CoLab, preparing environment.")
        for l in cmdLineForColab:
            os.system(l)
    except ImportError as err:
        print(err, "\nThis is not on CoLab, please preparing environment.")

    ```

    如果有缺漏也請聯絡作者
