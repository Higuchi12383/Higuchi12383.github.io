*{
 list-style-type:none;
 margin:0;
 padding:0;
}
body {
	margin: 0px;
	padding: 0px;
	color: #111;	/*全体の文字色*/
	font-family:"ヒラギノ角ゴ Pro W3", "Hiragino Kaku Gothic Pro", "メイリオ", Meiryo, Osaka, "ＭＳ Ｐゴシック", "MS PGothic", sans-serif;	/*フォント種類*/
	font-size: 15px;	/*文字サイズ*/
	line-height: 2;		/*行間*/
    background-color:#fff;
    background-image: url(img/back.png); 
         
    /* 画像を常に天地左右の中央に配置 */
    background-position: center center;
   
    /* 画像をタイル状に繰り返し表示しない */
    background-repeat: no-repeat;
   
    /* コンテンツの高さが画像の高さより大きい時、動かないように固定 */
    background-attachment: fixed;
   
    /* 表示するコンテナの大きさに基づいて、背景画像を調整 */
    background-size: cover;
   
    /* 背景画像が読み込まれる前に表示される背景のカラー */
    background-color: #464646
	-webkit-text-size-adjust: none;
	border-top: 5px solid #e71c64;
}
img{
outline:none;
border-style:none;
}

a{
	color:blue;
	-webkit-transition: all 0.5s;
	-moz-transition: all 0.5s;
	transition: all 0.5s;
}
a:visited{
	color:blue;
	-webkit-transition: all 0.5s;
	-moz-transition: all 0.5s;
	transition: all 0.5s;
}
a:hover {
	color: #F5A862;
	-webkit-transition: all 0.5s;
	-moz-transition: all 0.5s;
	transition: all 0.5s;
}
#header{
	display: block;
	width:70%;
	margin-left: 20%;
	overflow: hidden
        }
//------------メイン画像---------------//
#mainimg {
	margin-bottom: 20px;
}        
#left{
         height:550px;
         width:175px;
         margin-left: 12%;
         float:left;
         background-color:#ff9933
        }
#center{
         width:50%;
         height:1100px;
         float:left;
         background-color:rgba(255,225,225,0.7);
        }
#right{
         width:175px;
         height:550px;
         float:left;
         background-color:#ff9933;
        }
        
/*スライド設定
------------------------------------------------------------------------------------------------------------------------------------------------------*/

#slide_wrapp{
  position: relative;
  overflow: hidden;
  
.slide_item{
    opacity: 0;
    transform: scale(1);
    transition: opacity 2s linear, transform 7.5s linear;  //transformはFadeTime + IntarvalTime + α秒
    position: relative;
    
    &:not(:first-child){
     position: absolute;
     top: 0;
     left : 0;
    }
  
     &.show_{
     opacity: 1;
    }
     &.zoom_{
     transform: scale(1.1);
    }
     img{
     display: block; //下に余白できないように
    }
  }
}

#footer{
	font-size: 80%;	/*フォントサイズの指定*/
	width: 100%;	/*横幅の指定*/
	text-align: center;	/*文字の中央寄せ*/
	padding-top: 10px;	/*文字上部の余白指定*/
	padding-bottom: 10px;	/*文字下部の余白指定*/
	background-color: #313131;	/*背景色の指定*/
}
#footer address{
	color: #fff;	/*文字色の指定*/
	letter-spacing: 5px;	/*文字と文字の間隔をあける*/
	font-style: normal; /*文字の斜体を取り消す*/
}
/*画面幅750px以下の設定
------------------------------------------------------------------------------------------------------------------------------------------------------*/
@media screen and (max-width:750px){

/*ヘッダー（ロゴが入った最上段のブロック）
---------------------------------------------------------------------------*/
/*メイン画像*/
@media screen and (max-width: 600px){
  .main, .left-navi,.main-contents, .right-navi{
  width: 100%;
  }
}
}
