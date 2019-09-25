// CreateComponent.vue

addPost(){
    let uri = 'http://vuelaravelcrud.test/api/post/create';
    this.axios.post(uri, this.post).then((response) => {
       this.$router.push({name: 'posts'});
    });
}