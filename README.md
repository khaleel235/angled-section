<style>
/* # angled-sectionn */
/* create a customized section in landing page without using backgroud */
/*This ensures diagonal bg doesn't block page content*/

.lp-positioned-content{
  z-index: 100;  
}
/*Replace #lp-pom-block-21 with your section ID to create an angled bottom*/
#lp-pom-block-21:after{
  background: inherit;
  bottom: 0;
  content: '';
  display: block;
  height: 50%;
  left: 0;
  position: absolute;
  right: 0;
  transform: skewY(-3.75deg); /*change to increase/decrease angle*/
  transform-origin: 100%;
  z-index: 1; 
}
/*Replace #lp-pom-block-21 with your section ID to create an angled top*/  
#lp-pom-block-21:before{
  background: inherit;
  top: 0;
  content: '';
  display: block;
  height: 50%;
  left: 0;
  position: absolute;
  right: 0;
  transform: skewY(-3.75deg); /*change to increase/decrease angle*/
  transform-origin: 0;
  z-index: 1;   
}
</style>  
