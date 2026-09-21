# Jiaxian-DisasterShelter-GIS

A GIS-Based Disaster Shelter and Resource Allocation Framework

基於 GIS 的災害避難收容與資源調度系統

以高雄市甲仙區為案例，利用 GIS、路網分析與空間資料處理技術，建立災害發生時的避難收容分配、收容容量分析、避難路徑分析與資源調度決策支援框架。

---

## Project Background

本專案為國立成功大學 INHPC Lab 與防災研究中心合作計畫之議題四：

**災害收容與資源調度（Disaster Shelter and Resource Allocation）**

研究區域以高雄市甲仙區大田里為主，整合避難收容所、人口分布、保全戶、道路路網與物資儲放點等資料，建立災害應變決策支援模型。

---

## Research Objectives

### 1. 避難收容分配（Shelter Allocation）

- 保全戶指派至最近避難所
- 分析避難所服務範圍
- 評估收容資源覆蓋能力
- 找出服務缺口區域

### 2. 收容容量分析（Capacity Analysis）

計算：

```
Load Ratio = Assigned Population / Shelter Capacity
```

分析內容：

- 收容人口
- 收容容量
- 負載率
- 超載情況

輸出成果：

- Shelter Assignment Map
- Shelter Load Map

### 3. 避難路網分析（Evacuation Network Analysis）

利用道路路網建立：

- 最短避難路徑
- Service Area Analysis
- Accessibility Analysis
- Coverage Analysis

輸出成果：

- Evacuation Route Map
- Shelter Service Area Map

### 4. 物資調度規劃（Resource Dispatch Planning）

未來將進一步研究：

- 物資配送路徑規劃
- 資源優先分配策略
- 配送效率分析
- 決策支援系統

---

## Study Area

Location:

- Jiaxian District
- Kaohsiung City
- Taiwan

Case Type:

- Landslide Hazard
- Large-scale Collapse Hazard
- Shelter Allocation
- Disaster Resource Dispatch

---

## Methodology

```text
Protected Households
         │
         ▼
 Shelter Allocation
         │
         ▼
 Capacity Analysis
         │
         ▼
 Evacuation Network Analysis
         │
         ▼
 Resource Dispatch Planning
         │
         ▼
 Decision Support System
```

---

## Data Sources

### Local Validation Data

Provided by Disaster Research Center:

- Shelter locations
- Shelter capacities
- Protected household records
- Population statistics
- Resource storage locations
- Road network data
- Hazard maps

### Open Data

- OpenStreetMap (OSM)
- TDX Transportation Data eXchange
- Taiwan Open Government Data
- Ministry of the Interior Open Data

---

## GIS Dataset

GitHub is not suitable for storing large GIS datasets.

Large spatial datasets are stored on Google Drive:

### Download Link

https://drive.google.com/drive/u/1/folders/1RRHgRfps-1BkhPoauqxh3KRfSCPqxOFQ

Datasets may include:

- BaseData.gpkg
- QGIS Project Files
- Road Network Layers
- Shelter Layers
- Population Data
- Analysis Results

---

## Recommended Project Structure

```text
Jiaxian-DisasterShelter-GIS
│
├── README.md
├── LICENSE
│
├── data
│   ├── raw
│   ├── processed
│   └── external
│
├── qgis
│   ├── projects
│   └── styles
│
├── src
│   ├── preprocessing
│   ├── analysis
│   ├── network
│   └── visualization
│
├── notebooks
│
├── outputs
│   ├── maps
│   ├── figures
│   └── reports
│
└── docs
```

---

## Software

Recommended environment:

- QGIS 3.34+
- Python 3.11+
- GeoPandas
- Shapely
- NetworkX
- Pandas
- Matplotlib

Install commonly used packages:

```bash
pip install geopandas networkx shapely pandas matplotlib
```

---

## Current Progress

### Completed

- GIS data integration
- Shelter database preparation
- Population data collection
- Road network preparation

### In Progress

- Shelter capacity analysis
- Evacuation network analysis
- Service area analysis

### Future Work

- Resource dispatch model
- Vehicle routing problem (VRP)
- Dynamic allocation model
- Web GIS dashboard

---

## Author

**Po-Hsun Chang (張伯熏)**

National Cheng Kung University

INHPC Lab

---

## License

This project is licensed under the MIT License.
