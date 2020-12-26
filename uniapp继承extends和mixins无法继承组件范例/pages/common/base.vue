<script>
	import TestComp from "@/pages/components/TestComp.vue"
	export default{
		name: 'friendbase',
		props: {},
		data(){
			return {
				testval:'777'
			}
		},
		components: {
		  TestComp,
		},
		methods: {
			testFunction() {
				console.log('[2020-12-26 18:21:52 666]:',null);
			},
		}
	}
</script>
