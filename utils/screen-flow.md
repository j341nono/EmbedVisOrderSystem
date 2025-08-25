graph TD
    A[ログイン画面] --> B[ホーム画面]
    B --> C[商品一覧画面]
    B --> D[商品検索画面]
    B --> E[埋め込み可視化画面]
    B --> F[マイページ]
    
    C --> G[商品詳細画面]
    D --> G
    E --> G
    
    G --> H[カート画面]
    H --> I[注文確認画面]
    I --> J[注文完了画面]
    
    E --> K[2D可視化ビュー]
    E --> L[3D可視化ビュー]
    K --> G
    L --> G
    
    F --> M[注文履歴画面]
    F --> N[プロフィール設定画面]
    
    O[管理者ログイン] --> P[管理画面]
    P --> Q[商品管理画面]
    P --> R[注文管理画面]
    P --> S[ユーザー管理画面]
    
    Q --> T[商品追加・編集画面]
    T --> U[埋め込み生成実行]
    
    %% レコメンド機能の表示
    G --> V[類似商品表示]
    B --> W[パーソナライズ推薦表示]
    
    %% スタイリング
    classDef userScreens fill:#e1f5fe
    classDef adminScreens fill:#fff3e0
    classDef visualScreens fill:#f3e5f5
    classDef processScreens fill:#e8f5e8
    
    class A,B,C,D,F,G,H,I,J,M,N userScreens
    class O,P,Q,R,S,T adminScreens
    class E,K,L,U visualScreens
    class V,W processScreens

