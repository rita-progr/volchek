<template>
  <div class="volchekImage"></div>
  <div class="container">
    <div class="wrapper">
      <div class="banner-image"> </div>
        <h1>Булочная номер 7</h1>
        <button class="btn outline">Выйти</button>
        <ul class="responsive-table">
          <li class="table-header">
            <div class="col col-1">Номер заказа</div>
            <div class="col col-1">Время заказа</div>
            <div class="col col-1">Детали заказа</div>
            <div class="col col-1">Цена заказа</div>
            <div class="col col-1">Статус заказа</div>
          </li>
          <li class="table-row">
            <div class="col col-1" data-label="Номер заказа">42235</div>
            <div class="col col-1" data-label="Время заказа">12:45</div>
            <div class="col col-1" data-label="Детали заказа">булка, кофе, пицца, чипсы, круасан</div>
            <div class="col col-1" data-label="Цена заказа">$350</div>
            <div class="col col-1" data-label="Статус заказа">Делается</div>
          </li>
        </ul>
  </div>
</div>
</template>

<script>

</script>

<style scoped>
  .volchekImage{
    position: fixed; 
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image:url('https://static.sobaka.ru/images/image/01/09/21/41/_normal.jpg?v=1550933199');
    background-size: cover;
    background-position: center;
    filter: blur(0.5px);
    z-index: -1; 
  }

  .container{
    position: fixed;
    top: 20px;
    left: 20px;
    right: 20px;
    bottom: 20px;
    backdrop-filter: blur(16px) saturate(180%);
    -webkit-backdrop-filter: blur(16px) saturate(180%);
    background-color: rgba(17, 25, 40, 0.25);
    border-radius: 12px;
    border: 1px solid rgba(255, 255, 255, 0.125);
    padding: 0px 38px;
    filter: drop-shadow(0 30px 10px rgba(0,0,0,0.125));
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content:center;
    text-align: center;
  }

  .wrapper{
    width: 100%;
    height: 100%;
    margin-top: 0px;
  }

  .banner-image {
    margin-top: 20px;
    background-image: url(https://i.pinimg.com/originals/8e/77/a2/8e77a225c8c9e32154ac3529ec6d2d36.jpg);
    background-position: center;
    background-size: cover;
    height: 300px;
    width: 100%;
    border-radius: 12px;
    border: 1px solid rgba(255,255,255, 0.255)
  }

  h1{
    font-family: 'Lato', sans-serif;
    color: rgba(255,255,255,0.98);
    text-transform: uppercase;
    font-size: 2.4rem;
    letter-spacing: 2px;
  }

  .btn {
    border: none;
    padding: 12px 14px;
    border-radius: 14px;
    font-size: 12px;
    font-size: 1.3rem;  
    letter-spacing: 2px;  
    cursor: pointer;
    margin-top: 15px;
    margin-bottom: 15px;
  }

  .outline {
    background: transparent;
    color: #95A5A6;
    border: 1px solid #95A5A6;
    transition: all .3s ease;
  }

  .outline:hover{
    transform: scale(1.125);
    color: rgba(255, 255, 255, 0.9);
    border-color: rgba(255, 255, 255, 0.9);
    transition: all .3s ease;  
  }

  .responsive-table li {
    font-family: 'Lato', sans-serif;
    border-radius: 9px;
    padding: 25px 30px;
    display: flex;
    justify-content: space-between;
    margin-bottom: 25px;
    color:black;
  }

  .responsive-table .table-header {
    background-color: #95A5A6;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 0.03em;
  }

  .responsive-table .table-row {
    background-color: #ffffff;
    box-shadow: 0px 0px 9px 0px rgba(0,0,0,0.1);
  }

  .responsive-table .col-1 {
    flex-basis: 20%;
    text-align: center;
    
  }

  @media (max-width: 767px) {
    .responsive-table .table-header {
      display: none;
    }

    .responsive-table li {
      display: block;
    }

    .responsive-table .col {
      flex-basis: 100%;
    }

    .responsive-table .col {
      overflow-wrap: break-word;
      word-wrap: break-word;
      word-break: break-all;
    }

    .responsive-table .col {
      display: flex;
      padding: 10px 0;
    }

    .responsive-table .col:before {
      color: #6C7A89;
      padding-right: 10px;
      content: attr(data-label);
      flex-basis: 50%;
      text-align: right;
    }
  }
</style>
