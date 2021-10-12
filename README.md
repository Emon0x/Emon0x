- 👋 Hi, I’m @Emon0x
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Emon0x/Emon0x is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body{
    font-family: Arial, Helvetica, sans-serif;
}
.container{
    width: 1000px;
    margin:100px auto;
}
ul{
  list-style: none;
}
a{
  color: #fff;

  text-decoration: none;
}

/*dropdown menu*/
.menu {
  background-color: teal;
  margin-bottom: 35px;
}
.menu ul {
  display: flex;
  flex-direction: row;
}
.menu ul li a {
  display: block;
  padding: 20px;
  text-transform: capitalize;
  transition: .3s;
  font-size: 20px;
  font-weight: 500;
}
.menu ul li a:hover {
  background-color: green;
}
.menu ul li {
  border-right: 2px solid#999;
  position: relative;
}
.menu ul li:last-child{
  border-bottom: 0;
}
.menu ul li:hover ul{
  top: 100%;
  visibility: visible;
  opacity: 1;
}
.menu ul li ul li{
  border-bottom: 2px solid #999;
  border-right: 0;
}
.menu ul li ul{
 position: absolute;
 flex-direction: column;
 background-color: teal;
 width:200px ;
 top: 120%;
 visibility: hidden;
 opacity: 0   ;
 transition: .3s;
}

.menu ul li ul li ul.hidden{
  position: absolute;
  left: 100%;
  top: 50%;
  visibility: hidden;
  opacity: 0;
}
.menu ul li ul li:hover ul.hidden{
  visibility: visible;
  opacity: 1;
  top: 0;
}
.menu ul li ul li ul.hidden li ul.Hidden{
  position: absolute;
  left: 100%;
  top:50%;
  visibility: hidden;
  opacity: 0;
}
.menu ul li ul li ul.hidden li:hover ul.Hidden{
  visibility: visible;
  opacity: 1;
  top: 0;
}

/*vertical-timeline*/



.container h2 {
  text-align: center;
  text-transform: capitalize;
  color: #333;
  font-size: 40px;
  font-weight: 700;
  margin-bottom: 30px;
}
.timeline-content {
  border: 2px solid #ff7720;
  width: 45%;
  float: left;
  padding: 20px;
}
.timeline-content span {
  font-size: 25px;
  font-weight: 400;
  color: #333;
}
.timeline-content h1 {
  color: #333;
  margin: 14px 0;
  text-transform: capitalize;
  font-size: 35px;
}
.timeline-content p {
  line-height: 23px;
}

.vertical-time li {
  display: table;
  clear: both;
  position: relative;
  margin-bottom: 30px;
}

.vertical-time li:after{
position: absolute;
content: ""
;
width: 25px;
height: 25px;
left: 50%;
top: 50%;
transform: translate(-50%, -50%);
background-color: #ff7720;
border-radius: 50%;
}


.vertical-time {
  position: relative;
}
.vertical-time::after {
  position: absolute;
  content: "";
  width: 3px;
  height: 100%;
  background-color: #ff7720;
  left: 50%;
  top: 0;
  transform: translate(-50%);
}

.vertical-time li:nth-child(even) .timeline-content {
  float: right;
}
