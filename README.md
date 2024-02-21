# OpenVINO2023LTS_on_Colab_Samples
可運行於 Google Colab 環境之 OpenVINO 2023 LTS 範例（包括舊版 Open Model Zoo 範例）

## OpenVINO Open Model Zoo (OMZ) & Tools

Intel OpenVINO 自20018發行後 Open Model Zoo (OMZ) 一直提供很豐富的預訓練模型庫，很方便進行AI應用的實驗，其中包含：
* Intel's Pre-Trained
  Intel 提供之預設訓練模型，包括物件偵測、物件辨識、影像分割、姿態偵測、行為分析、語音處理、時間預測等數十種模型。此部份已直接轉成IR格式(Bin + Xml)，可直接載入運行。
* Public Pre-Trained
  常用公開預訓練模型，有數十種應用及數百個模型，下載後需依原始框架格式（如TensorFlow, PyTorch, Caffe等）轉換到IR格式才能載入運行。
* Demos
  提供整合型範例，使用單一或組合不同模型完成特定功能，搭配簡易顯示畫面，更方便使用者理解。

另外亦提供OMZ相關工具，方便使用者處理模型，主要包括下列四項工具。

| Tool             | Command             | Description                  |
|:-----------------|:--------------------|:---------------------------- |
| Model Downloader | `omz_downloader`    | 從Open Model Zoo下載模型      |
| Model Converter  | `omz_converter`     | 將模型轉換成 OpenVINO IR 格式  |
| Info Dumper      | `omz_info_dumper`   | 列印模型完整資訊               |
| Benchmark Tool   | `benchmark_app`     | 比較模型推論效能               |

隨著OpenVINO版本的迭代更新，在2023.1版後， OMZ 及相關工具在官方說明文件中就移到[舊版功能(Legacy Features)](https://docs.openvino.ai/2023.3/openvino_docs_OV_Converter_UG_prepare_model_convert_model_MO_OVC_transition.html)，不再持續維護。

舊版 Open Model Zoo 相關文件及範例仍於開源於 [Github](https://github.com/openvinotoolkit/open_model_zoo) 上，有需要可行下載研究。另外原始模型及說明文件亦可從[官方共用區](https://storage.openvinotoolkit.org/repositories/open_model_zoo/)中取得。

## OpenVINO Notebooks

為了讓大家更容易使用 OpenVINO ，自2021.4版後就開始提供 Jupyter Notebook 格式的範例程式庫 [Notebooks](https://github.com/openvinotoolkit/openvino_notebooks) ，主要分為五大部份。
* 第一步(First steps)（編號001~099）
* 轉換與優化(Covert & Optimize)（編號100~199）
* 模型展示(Model Demos)（編號200~299）
* 模型訓練(Model Training)（編號300~399）
* 即時展示(Live Demos)（編號400~499）

2022.1版後部份範例已支援直接在 Binder 線上運行。 2023.0版後除增加更多範例外，亦有部份範例支援直接在 Google Colab 環境下安裝 OpenVINO 及運行。

不過 Notebooks 範例中並未納入原先 OMZ Pri-Trained Model 及 Demos 範例，為了讓大家能繼續使用原先 OMZ 模型下載及轉檔功能， 2022.1版後就有提供範例 104-model-tools 教大家如何處理。


