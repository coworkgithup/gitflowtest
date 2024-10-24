%% 유스케이스 다이어그램 예시
graph TD
    %% 액터 정의
    actor Admin as "관리자"
    actor Investor as "일반회원"
    actor Trader as "트레이더"
    
    %% 시스템 정의
    classDef system fill:#f9f,stroke:#333,stroke-width:2px;
    
    %% 관리자 유스케이스
    Admin --> UC1[회원 관리]
    Admin --> UC2[전략 관리]
    Admin --> UC3[사이트 관리]
    
    %% 일반회원 유스케이스
    Investor --> UC4[전략 검색]
    Investor --> UC5[전략 팔로우]
    Investor --> UC6[리뷰 작성]
    Investor --> UC7[문의하기]
    
    %% 트레이더 유스케이스
    Trader --> UC8[전략 등록]
    Trader --> UC9[팔로워 관리]
    Trader --> UC10[문의 답변]
    
    %% 시스템 상자
    subgraph 시스템 "소셜 트레이딩 플랫폼"
        UC1
        UC2
        UC3
        UC4
        UC5
        UC6
        UC7
        UC8
        UC9
        UC10
    end
