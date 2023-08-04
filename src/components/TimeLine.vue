<template>
  <q-page>
    <div class="resume">
      <div class="func">
        <div class="work">
          <h3><i class="fa fa-briefcase"></i>Experiencia de trabalho</h3>
          <ul>
            <li><span>Technical Consultant -<br>Web Design</span><small>Fiserv</small><small>Apr 2018 - Now</small></li>
            <li><span>Web Designer</span><small>Lynden</small><small>Jan 2018 - Apr 2018</small></li>
            <li><span>Intern - Web Design</span><small>Lynden</small><small>Aug 2017 - Dec 2017</small></li>
          </ul>
        </div>
        <div class="edu">
          <h3><i class="fa fa-graduation-cap"></i>Experiencia na area da educação</h3>
          <ul>
            <li><span>Bachelor of Science<br>Web Design and Development</span><small>BYU-Idaho</small><small>Jan. 2016 -
                Apr. 2018</small></li>
            <li><span>Computer Science</span><small>Edmonds Community College</small><small>Sept. 2014 - Dec. 2015</small>
            </li>
            <li><span>High School</span><small>Henry M. Jackson High School</small><small>Jan. 2013 - Jun. 2015</small>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script>
export default {

}
</script>

<style scoped>
/*
$darkest-blue: #1a237e;
$darker-blue: #283593;
$dark-blue: #303f9f;
$medium-blue: #3949ab;
$light-blue: #3f51b5;
$lighter-blue: #5c6bc0;
$lightest-blue: #9fa8da;
$white: #ffffff;
$black: #0e1442;
$orange: #ffb300;
$yellow: #fdd835;
$dark-pink: #ad1457;
$light-pink: #d81b60;
*/

a {
  text-decoration: none;
  color: #ffffff;
  display: block;
  transition-duration: 0.3s;
}

ul {
  list-style-type: none;
  padding: 0;
}

/*h2 {} */

h3 {
  color: #ffb300;
  margin: 10px 0;
  text-transform: lowercase;
  font-size: 1.25em;
}

.resume {
  width: 100%;
  background: #1a237e;
  color: #ffffff;
  margin: 20px auto;
  position: relative;
  display: flex;
}

.resume .func {
  box-sizing: border-box;
  float: left;
}

.resume .func>div {
  padding-bottom: 10px;
}

.resume .func>div:last-of-type {
  padding-bottom: 0;
}

.resume .func {
  width: 100%;
  padding: 30px;
}

.resume .func:hover>div {
  transition-duration: 0.5s;
}

.resume .func:hover>div:hover h3 i {
  transform: scale(1.25);
}

.resume .func:hover>div:not(:hover) {
  opacity: 0.5;
}

.resume .func h3 {
  transition-duration: 0.3s;
  margin-top: 0;
}

.resume .func h3 i {
  color: #283593;
  background: #ffb300;
  width: 42px;
  height: 42px;
  font-size: 20px;
  line-height: 42px;
  border-radius: 50%;
  text-align: center;
  vertical-align: middle;
  margin-right: 8px;
  transition-duration: 0.3s;
}

.resume .func .work,
.resume .func .edu {
  float: left;
}

.resume .func .work small,
.resume .func .edu small {
  display: block;
  opacity: 0.7;
}

.resume .func .work ul li,
.resume .func .edu ul li {
  position: relative;
  margin-left: 15px;
  padding-left: 25px;
  padding-bottom: 15px;
}

.resume .func .work ul li:hover::before,
.resume .func .edu ul li:hover::before {
  animation: circle 1.2s infinite;
}

.resume .func .work ul li:hover span,
.resume .func .edu ul li:hover span {
  color: #fdd835;
}

@keyframes circle {
  from {
    box-shadow: 0 0 0 0px #ffb300;
  }

  to {
    box-shadow: 0 0 0 6px rgba(255, 255, 255, 0);
  }
}

.resume .func .work ul li:first-of-type::before,
.resume .func .edu ul li:first-of-type::before {
  width: 10px;
  height: 10px;
  left: 1px;
}

.resume .func .work ul li:last-of-type,
.resume .func .edu ul li:last-of-type {
  padding-bottom: 3px;
}

.resume .func .work ul li:last-of-type::after,
.resume .func .edu ul li:last-of-type::after {
  border-radius: 1.5px;
}

.resume .func .work ul li::before,
.resume .func .work ul li::after,
.resume .func .edu ul li::before,
.resume .func .edu ul li::after {
  content: "";
  display: block;
  position: absolute;
}

.resume .func .work ul li::before,
.resume .func .edu ul li::before {
  width: 7px;
  height: 7px;
  border: 3px solid #ffffff;
  background: #ffb300;
  border-radius: 50%;
  left: 3px;
  z-index: 1;
}

.resume .func .work ul li::after,
.resume .func .edu ul li::after {
  width: 3px;
  height: 100%;
  background: #ffffff;
  left: 5px;
  top: 0;
}

.resume .func .work ul li span,
.resume .func .edu ul li span {
  transition-duration: 0.3s;
}

.resume .func .work {
  width: 48%;
  background: #283593;
  padding: 15px;
  margin: 0 4% 15px 0;
}

.resume .func .edu {
  width: 48%;
  background: #283593;
  padding: 15px;
}

.resume .func .skills-prog {
  clear: both;
  background: #283593;
  padding: 15px;
}

.resume .func .skills-prog ul {
  margin-left: 15px;
}

.resume .func .skills-prog ul li {
  margin-bottom: 8px;
  display: flex;
  align-items: center;
  transition-duration: 0.3s;
}

.resume .func .skills-prog ul li:hover {
  color: #fdd835;
}

.resume .func .skills-prog ul li:hover .skills-bar .bar {
  background: #fdd835;
  box-shadow: 0 0 0 1px #fdd835;
}

.resume .func .skills-prog ul li span {
  display: block;
  width: 120px;
}

.resume .func .skills-prog ul li .skills-bar {
  background: #ffffff;
  height: 2px;
  width: calc(100% - 120px);
  position: relative;
  border-radius: 2px;
}

.resume .func .skills-prog ul li .skills-bar .bar {
  position: absolute;
  top: -1px;
  height: 4px;
  background: #ffb300;
  box-shadow: 0 0 0 #ffb300;
  border-radius: 5px;
}
</style>
