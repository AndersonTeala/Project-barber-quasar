<template class="absolute-top">
  <q-page style="background: #34495e">
  	<div class="row">
  		<div class="col">
		  	<q-img
		      src="https://images.unsplash.com/photo-1588771930296-88c2cb03f386?ixid=MXwxMjA3fDB8MHxzZWFyY2h8MzB8fGJhcmJlcnNob3B8ZW58MHx8MHw%3D&ixlib=rb-1.2.1&w=1000&q=80"
		      :ratio="16/9"
		    />
  		</div>
  	</div>
	<div class="row q-ma-sm">
		<div class="col">
			<q-tabs
	        v-model="tab"
	        indicator-color="21BA45"
	        class="bg-primary text-dark shadow-2"
		      >
	        <q-tab @click="abreAgenda = true" name="agenda" icon="event" label="AGÊNDA" />
	        <q-tab @click="bar2 = true" name="servico" icon="shopping_basket" label="SERVIÇOS" />
	        <q-tab @click="abreBarbers = true" name="profissionais" icon="3p" label="BARBERS" />
      		</q-tabs>
		</div>
	</div>
	<div class="row q-ma-sm">
		<div class="col">
			<q-tabs
	        v-model="tab"
	        indicator-color="21BA45"
	        class="bg-primary text-dark shadow-2"
		      >
	        <q-tab name="promocoes" icon="card_giftcard" label="PROMO" />
	        <q-tab name="fidelidade" icon="insert_emoticon" label="FIDE" />
	        <q-tab name="localizacao" icon="room" label="ONDE" />
      		</q-tabs>
		</div>
	</div>
	<div class="row q-ma-sm">
		<div class="col">
			<q-tabs
	        v-model="tab"
	        indicator-color="21BA45"
	        class="bg-primary text-dark shadow-2"
		      >
	        <q-tab name="perfil" icon="how_to_reg" label="CONTA" />
	        <q-tab name="ligar" icon="settings_phone" label="LIGAR" />
	        <q-tab name="firego" icon="whatshot" label="FIREGO" />
      		</q-tabs>
		</div>
	</div>
	<q-dialog v-model="abreAgenda">
	<div class="row q-ma-sm">
		<div class="col">
			<div class="q-pa-md">
				<div class="q-gutter-md row items-start">
					<q-date v-model="date" />
				</div>
			</div>
		</div>
	</div>
	</q-dialog>
	<q-dialog v-model="abreBarbers">
	<div class="row q-ma-sm">
		
	</div>
	</q-dialog>
  </q-page>
</template>

<script>

	import { Quasar, QImg, QExpansionItem, QSlideItem, QDialog, QAvatar } from 'quasar'

export default {
  name: 'PageIndex',
  data () {
    return {
      tab: 'mails',
			date: '2021/04/05',
			logged: false,
			abreAgenda: false,
			abreBarbers: false
    }
  },
	methods: {
		//
	}
}
</script>
