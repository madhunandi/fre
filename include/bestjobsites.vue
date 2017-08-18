<template>
 <div class="jobsitescontent">
 	<div class="eachjobsite" v-for="item in jobSitesData">
 		<!-- <p>{{item.title}}</p>
 		<p>{{item.siteurl}}</p> -->
 		<div class="each-link">
	 		<a class="button" v-bind:href="item.siteurl">
	      <text class="text">{{item.title}}</text>
	    </a>
    </div>
 	</div>
 </div>
	
</template>

<style scoped>
.jobsitescontent{
	display: flex;
	flex-direction: column;
}
.each-link{
  width: 700px;
  background-color: #f5f5f5;
  border:1px solid #ddd;
  margin: 10px 0;
  padding: 25px 0;
  align-self: center;
  align-items: center;
}
</style>

<script>
	module.exports = {
		data : function(){
	   return {
       jobSitesData : [{
       	title : "Angel.co",
       	siteurl : "http://www.angel.co/jobs"
       },
       {
       	title : "hasjob.co",
       	siteurl : "http://www.hasjob.co"
       },
       {
       	title : "Angel.co",
       	siteurl : "http://www.angl.co/jobs"
       },
       {
       	title : "Angel.co",
       	siteurl : "http://www.angl.co/jobs"
       }]
      }
		}
	}
</script>