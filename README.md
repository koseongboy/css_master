# CSS

## FlexBox

### 정렬 관련

justify-content: main axis 요소 옮기기  
align-items: cross axis 요소 옮기기  
flex-wrap -> 기본: 모든 flexbox 내부 요소는 원래 지정한 크기를 줄여서라도 한 줄에 있어야함, wrap인 경우: 길이 유지하고 넘어가면 줄바꿈

> flex-wrap: wrap; 인 경우
>
> > align-items: 만약 content가 두 줄일 경우 자기 줄 안에서 cross-axis 위치 조절
> > align-content: 요소가 몇 줄이든 전체를 wrapper 기준에서 cross-axis 위치 조절

### 크기 관련

flex-shrink: 자식 요소한테 부여하는 속성, 화면이 줄어들어 요소가 찌그러질 때 찌그러지는 비율을 조절 가능 (기본: 1)  
flex-grow: 자식 요소한테 부여하는 속성, 요소 사이에 빈 공간을 차지함. 숫자가 클 수록 빈 공간을 가져가는 비율이 커짐 (기본: 0)  
flex-basis: main-axis 상에서의 기본 길이를 정하는 요소

## Grid

### 정렬 관련

gap: 요소 사이 간격  
repeate(number, element): element를 number만큼 반복

> grid-template-areas: 표 안에 들어갈 거 설정 가능  
> ex)grid-template-areas  
> "header header header header"  
> "content content content nav"  
> "content content content nav"  
> "footer footer footer footer"  
> ;

> > 이후 자식 요소에 이름 입력
> > ex) grid-area: footer;

grid-row / grid-column: 자식 요소에 입력, startNum / finishNum 으로 구분, start에서 finish까지, (줄 구분은 row 한 칸이 아니라 구분선 한 칸). 뒤에서 부터도 가능(음수)  
span num: num만큼의 칸을 가진다.
