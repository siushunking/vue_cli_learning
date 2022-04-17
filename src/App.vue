<template>
<section>
  <h3> MY Friends </h3>
  <ul>
    <li>
      <friend-contact /> 
    </li>
  </ul>
 </section>   
</template>

<script>
export default{
  data() {
    return {
      friends:[
        {
          id: 'manuel',
          name: 'ivan',
          phone: '123456789',
          email: 'manuel@gmail.com'
        },
          {
          id: 'manuel',
          name: 'ivan',
          phone: '123456789',
          email: 'manuel@gmail.com'
        }
      ]
    }
  }
}
</script>