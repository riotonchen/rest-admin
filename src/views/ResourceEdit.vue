<template>
  <div >
    <b-row>
      <b-col cols="12">
       
          <b-data-form :resource="resource" :id="id" :languages="$store.state.site.languages"></b-data-form>
        
      </b-col>
    </b-row>
  </div>
</template>

<script>
import BDataForm from '../components/DataForm'
export default {
  name: "resource-edit",
  components: {
    BDataForm
  },
  data() {
    return {

    };
  },
  computed: {
    id() {
      return this.$route.params.id
    },
    resource() {
      return this.$route.params.resource
    }
  },
  methods: {
    
  },
  created() {
    
  }
};
</script>
