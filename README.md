# 키친포스

## 요구 사항

### 상품

- 상품을 등록할 수 있다.
- 상품의 가격이 올바르지 않으면 등록할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 이름이 올바르지 않으면 등록할 수 없다.
    - 상품의 이름에는 비속어가 포함될 수 없다.
- 상품의 가격을 변경할 수 있다.
- 상품의 가격이 올바르지 않으면 변경할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 가격이 변경될 때 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 크면 메뉴가 숨겨진다.
- 상품의 목록을 조회할 수 있다.

### 메뉴 그룹

- 메뉴 그룹을 등록할 수 있다.
- 메뉴 그룹의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴 그룹의 이름은 비워 둘 수 없다.
- 메뉴 그룹의 목록을 조회할 수 있다.

### 메뉴

- 1 개 이상의 등록된 상품으로 메뉴를 등록할 수 있다.
- 상품이 없으면 등록할 수 없다.
- 메뉴에 속한 상품의 수량은 0 이상이어야 한다.
- 메뉴의 가격이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴는 특정 메뉴 그룹에 속해야 한다.
- 메뉴의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 이름에는 비속어가 포함될 수 없다.
- 메뉴의 가격을 변경할 수 있다.
- 메뉴의 가격이 올바르지 않으면 변경할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴를 노출할 수 있다.
- 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 높을 경우 메뉴를 노출할 수 없다.
- 메뉴를 숨길 수 있다.
- 메뉴의 목록을 조회할 수 있다.

### 주문 테이블

- 주문 테이블을 등록할 수 있다.
- 주문 테이블의 이름이 올바르지 않으면 등록할 수 없다.
    - 주문 테이블의 이름은 비워 둘 수 없다.
- 빈 테이블을 해지할 수 있다.
- 빈 테이블로 설정할 수 있다.
- 완료되지 않은 주문이 있는 주문 테이블은 빈 테이블로 설정할 수 없다.
- 방문한 손님 수를 변경할 수 있다.
- 방문한 손님 수가 올바르지 않으면 변경할 수 없다.
    - 방문한 손님 수는 0 이상이어야 한다.
- 빈 테이블은 방문한 손님 수를 변경할 수 없다.
- 주문 테이블의 목록을 조회할 수 있다.

### 주문

- 1개 이상의 등록된 메뉴로 배달 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 포장 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 매장 주문을 등록할 수 있다.
- 주문 유형이 올바르지 않으면 등록할 수 없다.
- 메뉴가 없으면 등록할 수 없다.
- 매장 주문은 주문 항목의 수량이 0 미만일 수 있다.
- 매장 주문을 제외한 주문의 경우 주문 항목의 수량은 0 이상이어야 한다.
- 배달 주소가 올바르지 않으면 배달 주문을 등록할 수 없다.
    - 배달 주소는 비워 둘 수 없다.
- 빈 테이블에는 매장 주문을 등록할 수 없다.
- 숨겨진 메뉴는 주문할 수 없다.
- 주문한 메뉴의 가격은 실제 메뉴 가격과 일치해야 한다.
- 주문을 접수한다.
- 접수 대기 중인 주문만 접수할 수 있다.
- 배달 주문을 접수되면 배달 대행사를 호출한다.
- 주문을 서빙한다.
- 접수된 주문만 서빙할 수 있다.
- 주문을 배달한다.
- 배달 주문만 배달할 수 있다.
- 서빙된 주문만 배달할 수 있다.
- 주문을 배달 완료한다.
- 배달 중인 주문만 배달 완료할 수 있다.
- 주문을 완료한다.
- 배달 주문의 경우 배달 완료된 주문만 완료할 수 있다.
- 포장 및 매장 주문의 경우 서빙된 주문만 완료할 수 있다.
- 주문 테이블의 모든 매장 주문이 완료되면 빈 테이블로 설정한다.
- 완료되지 않은 매장 주문이 있는 주문 테이블은 빈 테이블로 설정하지 않는다.
- 주문 목록을 조회할 수 있다.

## 용어 사전

### 메뉴
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 메뉴 그룹 | Menu Group | 메뉴들의 집합으로 하나의 메뉴 그룹 안에 여러 메뉴가 속할 수 있다. |
| 메뉴 그룹 | Menu Group Name | 메뉴 그룹의 이름으로 메뉴 그룹 등록시 반드시 지정되어야 한다. |
| 메뉴 | Menu | 손님들에게 판매하기 위한 상품으로 메뉴는 반드시 특정 메뉴 그룹에 속해야 한다. |
| 메뉴 이름 | Menu Name | 메뉴를 지칭하는 것으로 메뉴 등록시 반드시 지정되어야 하며 비속어를 포함할 수 없다. |
| 메뉴에 속한 제품 | Menu Product | 메뉴에 속해 있는 특정 제품군에 대한 명세로서 한개 이상의 제품과 해당 제품의 수량으로 이루어진다. |
| 메뉴 가격 | Menu Price | 사용자에게 제공하기 위한 가격으로 구성된 제품 가격의 합보다 클 수 없다 |
| 메뉴 노출 여부 | Display | 사용자에게 특정 메뉴를 노출 혹은 숨김 처리 할 수 있다. 만약 메뉴의 가격이 메뉴를 구성하는 제품들의 가격의 합보다 높을 경우 메뉴를 숨김처리 해야 한다. |

### 주문
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 주문 | Order | 손님들이 메뉴를 구매 혹은 이용할 수 있도록 돕는 시스템 |
| 주문 유형 | Order Type | 주문은 각각 유형을 갖고 있으며 배달, 테이크아웃, 매장 중 하나의 값을 갖는다. |
| 주문 상태 | Order Status |주문은 각각의 진행 상태를 갖고 있으며 주문대기, 주문수락, 주문제공, 배달중, 배달완료, 주문완료 중 하나의 값을 갖는다. |
| 주문 항목 | Order Line Item| 손님들이 구매하려 하는 항목으로 해당 항목은 한 개 이상의 메뉴와 해당 메뉴의 수량을 포함한다. |
| 주문 시간 | Order Date Time | 손님들이 주문을 요청한 날짜와 시간 |
| 배달 주소 | Delivery Address | 손님이 배달을 받기 위한 주소로, 주문 유형이 배달일 경우 해당 주소를 반드시 포함해야 한다. |

### 제품
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 제품 | Product | 손님들에게 판매하기 위한 음식으로 제품은 여러개의 메뉴에 속할 수 있다. |
| 제품 이름 | Product Name | 손님들에게 판매하기 위한 제품의 이름으로 제품 등록시 반드시 지정되어야 한다. |
| 제품 가격 | Product Price | 손님들에게 판매하기 위한 제품의 가격으로 반드시 0보다 커야하고 변경 될 수 있다. |

### 주문 테이블
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 주문 테이블 | Order Table | 가게 안에서 손님들을 수용하기 위한 테이블 |
| 주문 테이블 이름 | Order Table Name | 주문 테이블의 이름으로 주문 테이블 등록시 반드시 지정되어야 한다. |
| 주문 테이블 이용자 수 | Number Of Guests | 주문 테이블에 앉아있는 손님 수 |
| 주문 테이블 이용 유무 | Used | 해당 주문 테이블을 손님이 이용하고 있는지 나타낸다 |


## 모델링

### 메뉴

 - 속성
    1. `Menu Group Name` 이 반드시 존재 해야 한다.
    2. `Menu Name` 이 반드시 존재 해야 한다.
    3. `Menu Group` 이 반드시 존재 해야 한다.
    4. `Menu Price` 는 반드시 존재해야 하고, 0 보다 커야 한다.
    5. `Display`의 기본 값은 True 이다.
 
 - 기능
    1. `Menu Group` 을  생성한다.
        - `Menu Group` 생성시 `Menu Group Name` 은 반드시 지정 되어야 한다.
    
    2. `Menu Group` 을 조회 한다.
        - 모든 `Menu Group` 을 조회 할 수 있다.
        - 특정 `Menu Group` 을 조회 할 수 있다.
    
    3. `Menu` 를 생성한다.
        - `Menu` 생성 시 `Menu Name` 이 지정 되어야 한다. `Menu Name` 은 비속어 존재 유무 체크를 통해 
        비속어가 존재 하지 않음을 보장해야 한다.
        - `Menu` 생성시 `Menu Price` 가 명시 되어야 한다. `Menu Price` 는  `Menu Product` 의 `Product Price` 의 합보다 클 수 없다.
        - `Menu` 생성 시 반드시 `Menu Group` 이 지정 되어야 한다.
    
    4. `Menu Price` 를 변경 한다.
        - `Menu Price` 변경 시 요청된 `Menu Price` 는 반드시 0 보다 커야 한다.
        - 요청된 `Menu Price` 는 `Menu Product` 의 `Product Price` 의 합보다 클 수 없다.
    
    5. `Menu` 의 `Display`를 노출로 변경 한다.
        - 해당 메뉴의 `Menu Price` 가 `Menu Product` 의 `Product Price` 의 합보다 크다면 노출로 변경 할 수 없다.
    
    6. `Menu` 를 조회 한다.
        - 특정 `Menu` 를 조회 한다.
        - 모든 `Menu` 를 조회 한다.

### 주문
 - 속성
    1. `Order Type` 은 반드시 지정되어야 하며 `Delivery`, `Takeout`, `Eat In` 중 하나이다
    2. `Order Line Item` 이 반드시 지정 되어야 한다.
    3. `Order Status`는 반드시 지정 되어야 하며, `Waiting`, `Accepted`, `Delivery`, `Served`,  `Completed` 중 하나이다.
   
 - 기능
    1. `Order` 를 조회 한다.
        - 특정 `Order` 를 조회 한다.
        - 모든 `Order` 를 조회 한다.
    
    2. `Order` 를 등록 한다.
        - `Order` 등록시 `Order Type` 이 지정 되어야 한다. `Order Type` 은 `Delivery`, `Takeout`, `Eat In` 중 하나이다
        - `Order` 등록시 `Order Line Item` 이 반드시 지정 되어야 한다. `Order Line Item` 에 포함 된 `Menu` 의 `Display` 는 노출된 상태여야 한다. `Order Line Item` 에 포함된 `Menu` 의 `Menu Price` 는 실제 `Menu` 의 `Menu Price` 와 같아야 한다.
        - `Order` 등록시 `Order Type`이 `Delivery` 인 경우 `Delivery Address` 가 지정 되어야 한다.
        - `Order` 등록시 `Order Type`이 `Eat in` 인 경우 `Order Table Number` 가 지정 되어야 하며 해당 `Order Table` 의 `Used`는 이용 하고 있지 않은 상태이어야 한다.
        - `Order` 등록이 완료 되면 `Order Status`는 `Waiting`이 된다.
        - `Order` 등록이 요청된 시간이 해당 `Order`의 `Order Date Time` 이다.
    
    3. `Order` 를 수락 한다.
        - 해당 `Order`의 `Order Status`는 `Waiting` 상태 이어야 한다.
        - 해당 `Order`의 `Order Type`이 `Delivery` 일 경우 `Order Price` 와 `Delivery Address` 로 `Request Delivery` 를 해야 한다.
        - `Order` 의 `Order Status` 를 `Accepted` 로 변경 한다.
    
    4. `Order` 를 제공 한다.
        - 해당 `Order` 의 `Order Status` 는 `Accepted` 이어야 한다.
        - `Order` 의 `Order Status` 를 `Served` 로 변경 한다.
    
    5. `Order` 배달을 시작 한다.
        - 해당 `Order` 의 `Order Type` 은 반드시 `Delivery` 이어야 한다.
        - 해당 `Order` 의 `Order Status` 는 반드시 `Served` 이어야 한다.
        - `Order` 의 `Order Status` 를 `Delivering` 으로 변경 한다.
    
    6. `Order` 배달을 완료 한다.
        - 해당 `Order` 의 `Order Type` 은 반드시 `Delivery` 이어야 한다.
        - 해당 `Order` 의 `Order Status` 는 반드시 `Delivering` 이어야 한다.
        - `Order` 의 `Order Status` 를 `Delivered` 로 변경 한다.
    
    7. `Order` 를 완료 처리 한다.
        - 해당 `Order` 의 `Order Type` 이 `Delivery` 인 경우 `Order Status` 는 `Delivered` 이어야 한다.
        - 해당 `Order` 의 `Order Type` 이 `Takeout` 이거나 `Eat in` 인 경우 `Order Status` 는 `Served` 이어야 한다.
        - 해당 `Order` 의 `Order Type` 이 `Eat In` 인 경우 해당 `Order Table` 의 `Number Of Guest` 는 `0` 그리고 `Used` 는 이용 하지 않음 처리 되어야 한다.

### 제품

 - 속성
    1. `Product Name` 는 반드시 지정 되어야 한다.
    2. `Product Price` 는 반드시 지정 되어야 하고 `0` 보다 커야 한다. 

 - 기능
    1. `Product` 를 등록 한다.
        - `Product` 등록 시 `Product Name` , `Product Price` 는 반드시 지정 되어야 한다.
        - `Product Name` 은 비속어 존재 유무 체크를 통해 비속어가 존재 하지 않음을 보장해야 한다.
        - `Product Price` 는 반드시 `0` 보다 커야 한다.
    
    2. `Product` 의 `Product Price` 를 변경 한다.
        - 변경 요청 된 `Product Price` 값은 `0`보다 커야 한다.
        - 변경 요청 된 `Product` 는  이미 구성되어 있는  `Menu` 의 `Menu Price`  영향을 미치므로 `Product Price` 가 변경 될 때 변경 된 값을 기준 으로 해당 `Menu` 의 `Menu Price` 는 `0` 보다 커야하며, `0`보다 작다면 해당 `Menu` 의 `Display` 는 숨김처리 되어야 한다.
    
    3. `Product` 를 조회 한다.
        - 특정 `Product` 를 조회 한다.
        - 모든 `Product` 를 조회 한다.
    
### 주문 테이블
    
 - 속성
    1. `Order Table Name` 이 반드시 지정 되어야 한다.
    2. `Used` 는 반드시 지정 되어있어야 하고 기본 값은 이용 하고 있지 않음이다.
    3. `Number Of Guests` 는 반드시 지정 되어야 하고 기본 값은 `0` 이다.
     
 - 기능
    1. `Order Table` 을 등록 한다.
        - 등록 시 `Order Table Name` 이 반드시 지정 되어야 한다.
        - 등록 완료 시 `Number Of Guests` 는 `0` , `Used` 는 이용 하고 있지 않음 으로 설정 된다.
    
    2. `Order Table` 를 이용하고 있음으로 변경 한다.
        - `Order Table` 의 `Used` 를 이용함으로 변경 한다.
    
    3. `Order Table` 을 이용하고 있지 않음으로 변경 한다.
        - 요청된 `Order Table` 에 해당 되는 `Order` 의 `Order Status` 는 `Completed` 이어야 한다.
        - `Order Table` 의 `Number of Guests` 를 `0` 으로 변경한다.
        - `Order Table` 의 `Used` 를 이용하고 있지 않음으로 변경 한다.
    
    4. `Order Table` 의 이용자 수를 변경 한다.
        - 변경 요청 된 `Number Of Guests` 의 값은 `0` 보다 커야 한다.
        - 해당 `Order Table` 의 `Used` 는 이용하고 있는 상태 이어야 한다.
        - 해당 `Order Table` 의 `Number Of Guests` 의 값을 변경 한다.
    
    5. `Order Table` 을 조회 한다.
        - 모든 `Order Table` 을 조회 한다.
