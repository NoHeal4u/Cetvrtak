<template>
	<div class = "container mt-4">
	Contacts
	<div class = "row">
	<div class = "col">

	<ContactList :contacts="contacts"/>
	</div>
	<div class = "col">
	<ContactDetails/>
	</div>

	</div>

	</div>

	
</template>


<script>

import ContactList from '../components/ContactList'
import ContactDetails from '../components/ContactDetails'
	
	

	export default {
		components: {
			ContactList,
			ContactDetails
		},

		data(){
			return {
				contacts: [
				{name: 'John doe'},
				{name: 'John doe'},
				{name: 'John doe'}
				]
			}
		}
		
	}

</script>