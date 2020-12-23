# style.css
@charset "UTF-8";




html {
  font-size: 62.5%;
}
body {
  color: #333;
  font-size: 1.2rem;
  font-family: "Hiragino Kaku Gothic ProN",  Meiryo,  sans-serif;
}
*, *::before, *::after {
  box-sizing: border-box;
}
a:link, a:visited, a:hover, a:active {
  color: #d03c56;
  text-decoration: none;
}





.clearfix::after {
  content: '';
  display: block;
  clear: both;
}
.heading {
  padding: 10px 12px;
  background: url('../images/bg-slash.gif');
  letter-spacing: 1px;
  font-size: 1.6rem;
}
.hidden {
  display: none;
}




.header {
  width: 100%;
  padding: 28px 0 10px;
  background: url('../images/bg-header.gif') repeat-x;
  box-shadow: 0 0 10px 1px #e3e3e3;
}
.logo {
  width: 225px;
  height: 56px;
  margin: 0 auto;
  background: url('../images/logo.png') no-repeat;
  overflow: hidden;
  text-indent: 100%;
  white-space: nowrap;
}
.logo a {
  display: block;
  width: 100%;
  height: 100%;
}
.global-nav {
  margin-top: 15px;
  text-align: center;
}
.global-nav .nav-item {
  display: inline-block;
  margin: 0 10px;
}
.global-nav .nav-item a {
  display: inline-block;
  width: 100px;
  height: 30px;
  line-height: 30px;
  text-align: center;
  border-radius: 8px;
  color: #666;
  font-size: 1.3rem;
  letter-spacing: 1px;
  transition: 0.15s;
}
.global-nav .nav-item.aclive a,
.global-nav .nav-item a:hover {
  background-color: #d03c56;
  color: #fff;
}





.wrapper {
  width: 970px;
  margin: 30px auto 40px;
}





.main {
  display: block;
  float: left;
  width: 660px;
}
.hot-topic {
  display:block;
  height:300px;
  margin-bottom: 30px;
  box-shadow: 0 6px 4px -4px rgba(0,0,0,0.15);
  transition: opacity 0.15;
}
.hot-topic:hover {
  opacity: 0.85;
}
.hot-topic .image {
  float:left;
  width:50%;
  height:100%;
}
.hot-topic .content {
  position:relative;
  float:left;
  width:50%;
  height:100%;
  padding:105px 25px 0;
  background-color:#2d3d54;
  line-height:1.6;
}
.hot-topic .title {
  margin-bottom:15px;
  color:#fff;
  font-weight:normal;
  font-size:2.0rem;
}
.hot-topic .desc {
  color:#ddc;
}
.hot-topic .date {
  position:absolute;
  top:60px;
  left:0;
  width:140px;
  padding:4px;
  background-color:#fff;
  color:#2d3d54;
  text-align:center;
  letter-spacing: 1px;
  font-weight:bold;
  font-size:1.1rem;
  line-height:1;
}
.scroll-list {
  max-height:220px;
  overflow-y:auto;
  margin-bottom:30px;
  list-style:none;
}
.scroll-list .scroll-item a {
  display: block;
  padding: 10px 15px;
  color: #333;
  font-size: 0;
  transition: background-color 0.1s;
}
.scroll-list .scroll-list:nth-of-type(even) {
  background: url('../images/bg-slash.gif');
}
.scroll-list .scroll-item a:hover {
  background-color: #fafaf8;
}
.scllor-list .date {
  display: inline-block;
  width: 19%;
  letter-spacing: 1px;
  font-weight:bold;
  font-size: 1.0rem;
}
.scllor-list .category {
  display: inline-block;
  width:8%;
  border-radius: 5px;
  background-color: #d03c56;
  color: #fff;
  text-align: center;
  letter-spacing: 1px;
  font-size: 1.0rem;
  line-height:16px;
}
.scllor-list .category .news {
  background-color: #2c3c53;
}
.scllor-list .title {
  display :inline-block;
  width:73%;
  padding-left: 15px;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  font-size: 1.2rem;
}
.article-box {
  position: relative;
  display: block;
  width: 315px;
  height:360px;
  margin-bottom: 30px;
  padding:210px 15px 0;
  box-shadow: 6px 6px 8px -4px rgba(0,0,0,0.15);
  transition:opacity 0.15s;
}
.article-box:hover {
  opacity:0.8;
}
.article-box:nth-of-type(odd) {
  float: left;
}
.article-box:nth-of-type(even) {
  float:right;
}
.article-box .title {
  margin-top: 30px;
  color: #555;
  font-size: 1.4rem;
  line-height: 1.6;
}
.article-box .desc {
  margin-top: 5px;
  color: #333;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
.article-box .date {
  position: absolute;
  right: 0;
  bottom: 15px;
  display: block;
  width: 160px;
  padding: 4px;
  border-color: #b5d264;
  color: #2d3d54;
  text-align: center;
  letter-spacing: 1px;
  font-weight: bold;
  font-size: 1.1rem;
}
.article-box .image {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
}
.ranking {
  margin-bottom: 30px;
  list-style: none;
  counter-reset: ranking;
}
.ranking .ranking-item {
  margin-top: 15px;
}
.ranking .ranking-item a {
  display:block;
  /* font-size: 0;  */
  transition: opacity 0.15s;
}
.ranking .ranking-item  a:hover {
  opacity: 0.8;
}
.ranking .image {
  width: 55px;
  height: 55px;
}
.ranking .text {
  display: inline-block;
  width: 182px;
  color: #000;
  vertical-align: top;
  line-height: 1.5;
}
.ranking .order {
  display: inline-block;
  width: 18px;
  height: 18px;
  margin: 0 10px;
  border: 1px solid #ccc;
  color: #aaa;
  vertical-align: 20px;
  text-align: center;
  font-weight: bold;
  line-height: 16px;
  -webkit-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  transform: rotate(45deg);
}
.ranking .ranking-item:nth-of-type(1) .order,
.ranking .ranking-item:nth-of-type(2) .order,
.ranking .ranking-item:nth-of-type(3) .order, {
  border: none;
  color: #fff;
  font-weight: normal;
  line-height: 18px;
}
.ranking .ranking-item:nth-of-type(1) .order {
  background-color: #dab413;
}
.ranking .ranking-item:nth-of-type(2) .order {
  background-color: #6e7b84;
}
.ranking .ranking-item:nth-of-type(3) .order {
  background-color: #a0541a;
}
.ranking .order ::before {
  content: counter(ranking);
  counter-increment: ranking;
  content: '1';
  display: inline-block;
  font-size: 1.0rem;
  -webkit-transform: rotate(-45deg);
  -ms-transform: rotate(-45deg);
  transform: rotate(-45deg);
.documents {
  margin: 15px 0;
}
.documents,
.documents ul {
  list-style-type: none;
}
.documents > li .title {
  margin: 15px 0;
  padding-left: 8px;
  border-left: 5px solid #d03c56;
  font-size: 1.4rem;
  line-height: 1.2;
}
.documents > li + li {
  margin-top: 25px;
}
.documents > li ul {
  margin: 15px;
}
.documents > li ul {
  margin-bottom: 15px;
  padding-left: 10px;
  background-color: url('../images/arrow.gif') no-repeat left center;
}
.documents a:hover {
  text-decoration: underline;
}
.serch-box {
  padding: 15px;
  background-color: #ccc;
  font-size: 0;
}
.serch-box > * {
  font-size: 1.2rem;
}
.serch-box .serch-input {
  width: 205px;
  height: 26px;
  padding: 0 10px;
  border: none;
}
.serch-box .serch-button {
  width: 40px;
  height: 26px;
  border: none;
  border-color: #d03c56;
  color: #fff;
  cursor: pointer;
}
.serch-box .text {
  margin-top: 12px;
}
.footer {
  width: 100%;
  padding: 20px 0 30px;
  background: #2d3d54 url('../images/bg-footer.gif');
  color: #fff;
}
.horizontal-list {
  width: 970px;
  margin: 0 auto;
  text-align: right;
  font-size: 0;
}
.horizontal-list .horizontal-item {
  display: inline-block;
  padding: 0 15px;
  letter-spacing: 1px;
}
.horizontal-list .horizontal-item + .horizontal-item {
  border-left: 1px solid #bbb;
}
.horizontal-list .horizontal-item a {
  border-bottom: 1px dashed #777;
  color: #bbb;
  font-size: 1.1rem;
  transition: color 0.15s;
}
.horizontal-list .horizontal-item a:hover {
  color: #ddd;
}
.copyright {
  margin-top: 30px;
  text-align: center;
  letter-spacing: 1px;
}
