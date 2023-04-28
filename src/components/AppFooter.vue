<script>
import FooterTop from "./FooterTop.vue";
import FooterBottom from "./FooterBottom.vue";


export default {
    name: 'AppFooter',

    data() {
        return {
            footerLinks: [
				[	
					{
						text: 'Providing Life Changing',
						href: '#',
					},
					{
						text: 'Experiences Through',
						href: '#',
					},
					{
						text: 'Education. Class That fit Your',
						href: '#',
					},
					{
						text: 'Busy Life. Closer to Home',
						href: '#',
					}
				],
                [	
					{
						text: 'Business English',
                        name: 'Preston Marshall',
					},
					{
						text: 'Social Computing',
                        name: 'David Sanders',
					},
					{
						text: 'Learn Spanish',
                        name: 'Jennie King',
					}
				],
                [	
					{
						text: 'User dashboard',
						href: '#',
					},
					{
						text: 'Contact Us',
						href: '#',
					},
					{
						text: 'FAQ',
						href: '#',
					},
					{
						text: 'Course Offer',
						href: '#',
					},
                    {
						text: 'Events',
						href: '#',
					}
				],
                [	
					{
						text: 'Copyrights 2017',
						href: '#',
					},
					{
						text: ' Mikado Themes',
						href: '#',
					},
					{
						text: 'CALL +44 300 303 0266',
						href: '#',
					},
					{
						text: 'Course Offer',
						href: '#',
					},
                    {
						text: 'FOLLOW US',
						href: '#',
					}
				],
			],
            bottomFooterText: [
                "Copyrights 2017 Mikado Themes",
                "CALL +44 300 303 0266 ",
                "FOLLOW US"
            ]
        }
    },
    components: {
        FooterTop,
        FooterBottom
    }
}
</script>

<template>
    <div class="footer">
        <FooterTop :list="footerLinks"/>
        <FooterBottom :text="bottomFooterText"/>
    </div>
        
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables' as *;
    .footer{
        background-color: $bg-dark;
    }
</style>