# CSS_layout_flex
240120_CSS_flex_repeat

1. flex (flex container , flex item) 활용 -> 다양한 레이아웃 가능
2. .flex{
   diplay: flex;
   }
   
1) flex container 속성
   1. flex-direction
      : 아이템 배열 방향
      -row(default): 행, 옆으로 배열
      -column: 열, 아래로 배열, 옆으로 늘어남
```
예제 1
      <style>
        .flex{
            display: flex;
        }
        #box1{
            width: 150px;
            height: 100px;
        }
        #box2{
            width: 150px;
            height: 100px;
        }
        
        .flex-row{
            flex-direction: row;
        }

        .flex-col{
            flex-direction: column;
        }

        #italy .item{
            width: 50px;
            height: 100px;
        }
        #germany .item{
            width: 150px;
            height: 33.3333px;
        }

        .green{
            background-color: green;
            
        }
        .white{
            background-color: white;
          
        }
        .red{
            background-color: red;
            
        }
        .black{
            background-color: black;
           
        }
        .gold{
            background-color: gold;
           
        }
        
      </style>

      <h3>Italy</h3>
      <div id="italy" class="flex flex-row">
        <div class="item green"></div>
        <div class="item white"></div>
        <div class="item red"></div>
      </div>
      
      <h3>Germarny</h3>
      <div id="germany"class="flex flex-col">
          <div class="item black"></div>
          <div class="item red"></div>
          <div class="item gold"></div>
      </div>
```
   2. flex-wrap
   3. justify-contenet-(row,column)
   5. align-items-(row,column)

2). flex item 속성
   1. flex-basis
   2. flex-grow
   3. flex-shrink
   4. flex-order
