<template>
  <table-props
    :props='props'>
  </table-props>
</template>

<script>
import TableProps from '../../app/tables/TableProps';
import props from '../../api/props';

export default {
  components: {
    TableProps,
  },
  data() {
    return {
      props: props.filter(p => p.themable),
    };
  },
};
</script>
