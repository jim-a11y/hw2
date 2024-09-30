```mermaid
graph TD;
    A[研擬計劃<br/>開始: 2024-09-30<br/>結束: 2024-09-30] -->|1天| B[任務分配<br/>開始: 2024-09-30<br/>結束: 2024-10-04];
    A -->|1天| C[取得硬體<br/>開始: 2024-09-30<br/>結束: 2024-10-17];
    B -->|4天| D[程式開發<br/>開始: 2024-10-05<br/>結束: 2024-12-26];
    C -->|17天| E[安裝硬體<br/>開始: 2024-10-18<br/>結束: 2024-10-27];
    D -->|70天| F[程式測試<br/>開始: 2024-12-27<br/>結束: 2025-01-25];
    E -->|10天| G[撰寫使用手冊<br/>開始: 2024-10-28<br/>結束: 2024-12-01];
    E -->|20天| H[轉換檔案<br/>開始: 2024-10-28<br/>結束: 2024-12-15];
    F -->|30天| I[系統測試<br/>開始: 2025-01-26<br/>結束: 2025-02-25];
    G -->|25天| J[使用者訓練<br/>開始: 2024-12-02<br/>結束: 2024-12-26];
    H -->|20天| J;
    I -->|25天| K[使用者測試<br/>開始: 2025-02-26<br/>結束: 2025-03-02];
    J -->|20天| K;

    style A fill:#ffcccc,stroke:#333,stroke-width:2px;
    style D fill:#ffcccc,stroke:#333,stroke-width:2px;
    style F fill:#ffcccc,stroke:#333,stroke-width:2px;
    style I fill:#ffcccc,stroke:#333,stroke-width:2px;
    style K fill:#ffcccc,stroke:#333,stroke-width:2px;

```

```mermaid
gantt
    title 工作分解結構清單
    dateFormat  YYYY-MM-DD
    section 項目階段
        研擬計劃          :a1, 2024-10-01, 1d
        任務分配          :a2, after a1, 4d
        取得硬體          :a3, after a1, 17d
        程式開發          :a4, after a2, 70d
        安裝硬體          :a5, after a3, 10d
        程式測試          :a6, after a4, 30d
        撰寫使用手冊      :a7, after a5, 25d
        轉換檔案          :a8, after a5, 20d
        系統測試          :a9, after a6, 25d
        使用者訓練        :a10, after a7, 20d
        使用者測試        :a11, after a9, 25d
