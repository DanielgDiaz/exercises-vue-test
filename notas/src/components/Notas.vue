<template>
    <form action="@submit.prevent">

 <label>Selecciona tu nota</label>
    <select v-model="nota">
      <option value=1>1</option>
      <option value=2>2</option>
      <option value=3>3</option>
      <option value=4>4</option>
      <option value=5>5</option>
      <option value=6>6</option>
      <option value=7>7</option>
      <option value=8>8</option>
      <option value=9>9</option>
      <option value=10>10</option>
    </select>

     <div class="submit">
      <button>Nota</button>
    </div>
    </form>
</template>
<script>
export default {
    name: "Notas",
  
  data() {
    return {
      nota: "",

    };
  },
  methods: {
    submitForm() {
      console.log("Funciona!");
    },
  },
};
</script>

<style>
form {
  max-width: 420px;
  margin: 30px auto;
  background: white;
  text-align: left;
  padding: 40px;
  border-radius: 10px;
}
label {
  color: #aaa;
  display: inline-block;
  margin: 25px 0 15px;
  font-size: 0.6em;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: bold;
}
input,
select {
  display: block;
  padding: 10px 6px;
  width: 100%;
  box-sizing: border-box;
  border: none;
  border-bottom: 1px solid #ddd;
  color: #555;
}
input[type="checkbox"] {
  display: inline-block;
  width: 16px;
  margin: 0 10px 0 0;
  position: relative;
  top: 2px;
}
.pills {
  display: flex;
  flex-wrap: wrap;
  gap: 5px;
  margin-top: 10px;
}
.pills .pill {
  background: rgba(34, 130, 255, 0.15);
  padding: 5px 10px;
  border-radius: 15px;
  color: rgb(34, 130, 255);
  letter-spacing: 1px;
  display: flex;
  align-items: center;
}
.pills .pill span {
  margin-left: 10px;
  font-size: 20px;
  cursor: pointer;
}
.submit {
  text-align: center;
  margin-top: 20px;
}
.submit button {
  background: rgb(8, 163, 125);
  border: none;
  border-radius: 5px;
  color: white;
  padding: 15px 25px;
  font-size: 18px;
}
.error {
  color: #ff0062;
  margin-top: 10px;
  font-size: 0.8em;
  font-weight: bold;
}
</style>