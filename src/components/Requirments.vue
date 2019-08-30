<template>
    <div class="requirements_container">
        <div>
            <h2>
                Requirements
            </h2>
            <p class="subtitle">Check If Your App is Eligible to be Uploaded to Google Play Store via SG Builder Console</p>
            <hr>
            <p v-for="point in points" :key="point.text" class="points">
							<i :class="point.icon" aria-hidden="true"></i> {{ point.text }}
						</p>
        </div>
    </div>
</template>

<style lang="css" scoped>
	.requirements_container{
			min-height: 75vh;
	}
	.subtitle{
		font-size: 0.9rem;
		color: #777;
	}
	.points{
		margin-bottom: 2vh;
		font-size: 1.2rem;
	}
</style>

<script>
export default {
	data(){
		return{
			points: [
				{
					icon: 'fa fa-check',
					text: 'App Should have Enough Content'
				},
				{
					icon: 'fa fa-times',
					text: 'Apps which contain Only Web View and a Few Components Are not Allowed.'
				},
				{
					icon: 'fa fa-dot-circle-o',
					text: 'Apps Made for the Purpose of Earning Money or Apps which contains more than 3 Ads per Screen are not Allowed(Maximum of 2 Banners, Interstitial/Rewarded Should not Be called before 15 sec of Launch)'
				},
				{
					icon: 'fa fa-clone',
					text: 'Apps which are Similar to Other Apps in UI or Design will not be Allowed'
				},
				{
					icon: 'fa fa-codepen',
					text: 'The App Should Contain "Made with SG Builder" on the Splash OR on the 1st Screen.'
				},
				{
					icon: 'fa fa-cloud',
					text: 'The App Should be made From SG Builder.'
				}
			]
		}
	}
}
</script>>