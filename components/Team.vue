<style>

.our-team {
  padding: 30px 0 40px;
  margin-bottom: 30px;
  background-color: #f7f5ec;
  text-align: center;
  overflow: hidden;
  position: relative;
}

.our-team .picture {
  display: inline-block;
  height: 130px;
  width: 130px;
  margin-bottom: 50px;
  z-index: 1;
  position: relative;
}

.our-team .picture::before {
  content: "";
  width: 100%;
  height: 0;
  border-radius: 50%;
  background-color: #1369ce;
  position: absolute;
  bottom: 135%;
  right: 0;
  left: 0;
  opacity: 0.9;
  transform: scale(3);
  transition: all 0.3s linear 0s;
}

.our-team:hover .picture::before {
  height: 100%;
}

.our-team .picture::after {
  content: "";
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background-color: #1369ce;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
}

.our-team .picture img {
  width: 100%;
  height: auto;
  border-radius: 50%;
  transform: scale(1);
  transition: all 0.9s ease 0s;
}

.our-team:hover .picture img {
  box-shadow: 0 0 0 14px #f7f5ec;
  transform: scale(0.7);
}

.our-team .title {
  display: block;
  font-size: 15px;
  color: #4e5052;
  text-transform: capitalize;
}

.our-team .social {
  width: 100%;
  padding: 0;
  margin: 0;
  background-color: #1369ce;
  position: absolute;
  bottom: -100px;
  left: 0;
  transition: all 0.5s ease 0s;
}

.our-team:hover .social {
  bottom: 0;
}

.our-team .social li {
  display: inline-block;
}

.our-team .social li a {
  display: block;
  padding: 10px;
  font-size: 17px;
  color: white;
  transition: all 0.3s ease 0s;
  text-decoration: none;
}

.our-team .social li a:hover {
  color: #1369ce;
  background-color: #f7f5ec;
}

</style>

<template>
  <div class="relative flex items-top justify-center">
      <div class="container">
      <div class="row">
        <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="our-team">
              <div class="picture">
                <img class="img-fluid" src="jayare.jpg" alt="Jay Are Galinada">
              </div>
              <div class="team-content">
                <h3 class="name">Jay Are Galinada</h3>
                <h4 class="title">LaravelPH chief Head</h4>
              </div>
              <ul class="social">
                <li><a href="https://github.com/jayaregalinada" class="fa fa-github" aria-hidden="true"></a></li>
              </ul>
            </div>
          </div>
        <div class="col-12 col-sm-6 col-md-4 col-lg-3">
            <div class="our-team">
              <div class="picture">
                <img class="img-fluid" src="joe.jpg" alt="Joe Palala">
              </div>
              <div class="team-content">
                <h3 class="name">Joe Palala</h3>
                <h4 class="title">LaravelPH Co-founder</h4>
              </div>
              <ul class="social">
                <li><a href="https://facebook.com/jpalala.me" class="fa fa-facebook" aria-hidden="true"></a></li>
                <li><a href="https://github.com/joepalala" class="fa fa-github" aria-hidden="true"></a></li>
              </ul>
            </div>
          </div>

        </div>
      </div>
  </div>
</template>

            