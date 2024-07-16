<template>
    <div>
      <header>
        <div style="width: 100%; height: 5vw;">
          <a-flex gap="middle">
            <a-flex gap="middle" justify='space-evenly' style="width: 50%;height: 5vw; display: flex; align-items: center;">
              <div>
                <h1>лого</h1>
              </div>
              <a-button type="link" href="/">Гланая</a-button>
              <a-button type="link" href="/">Квартиры</a-button>
              <a-button type="link" href="/">Контакты</a-button>
              <a-button type="link" href="/">О нас</a-button>
            </a-flex>
            <div style="background-color: #2B7AF1; width: 50%; display: flex; align-items: center">
              <a-flex gap="middle" justify='space-evenly' style="padding: 0 8px; width: 100%;">
                <a-flex gap="5">
                  <div class="card">
                    <MailTwoTone style="font-size: 20px;" />
                  </div>
                  <span class="text">mail@yandex.ru</span>
                </a-flex>
                <a-flex gap="5">
                  <div class="card">
                    <PhoneTwoTone style="font-size: 20px;" />
                  </div>
                  <span class="text">+7 (919) 714-25-00</span>
                </a-flex>
                <div style="position: relative; bottom: 5px;">
                  <a-button type="primary" size="middle" style="background-color: #FF7A00; border-radius: 15px;">Заказать звонок</a-button>
                </div>
              </a-flex>
            </div>
          </a-flex>
        </div>
      </header>
      <main>
        <div class="pages"> 
    <div> pages home </div>


        </div>
        
        <div class="recurring_element ">
           <div class="About_us">
            <div>
                <h1 class="span_blue">О нас</h1>
            </div>
             
             <div>
            <a-row  class="justify_center">
               <a-col :span="6" style="columns: auto;">
                Сегодня «Домашняя гостиница» — одна из крупнейших в Пермском крае гостиничных сетей, 
                динамично расширяющая географический охват и повышающая качество сервиса.
            </a-col>
              <a-col :span="6" class="justify_center">
                <a-flex gap="middle">
                <UserOutlined style="font-size: 45px; color: #2B7AF1;" />
                <div>
                    <h1 class="span_blue" >40+</h1>
                    <h3>Клиентов</h3>
                </div>
            </a-flex>
              </a-col>
              <a-col :span="6" class="justify_center">
               
                <a-flex gap="middle">
               <AliwangwangOutlined  style="font-size: 45px; color: #2B7AF1;"/>
                <div>
                    <h1 class="span_blue" >100+</h1>
                    <h3>Отзывов</h3>
                </div>
            </a-flex>
            </a-col>
              <a-col :span="6" class="justify_center">
               
                <a-flex gap="middle">
               <HomeOutlined  style="font-size: 45px; color: #2B7AF1;"/>
                <div>
                    <h1 class="span_blue" >10+</h1>
                    <h3>Квартир</h3>
                </div>
            </a-flex>
            </a-col>
             </a-row>
             </div>

           </div>
           <div class="gradient-line"></div>
        </div>
      </main>
    </div>
  </template>
  

<script>
 import { MailTwoTone , PhoneTwoTone ,UserOutlined, AliwangwangOutlined ,HomeOutlined  } from '@ant-design/icons-vue';
 import { defineComponent } from 'vue';
 export default defineComponent({
    components: {
        MailTwoTone,PhoneTwoTone , UserOutlined , AliwangwangOutlined, HomeOutlined
    },
  });
</script>
<style>
*{
    margin: 0;
    padding: 0;
}
.card{
    background-color: rgb(255, 255, 255);
     border-radius: 3rem; 
    width: 30px;
    height: 30px;
     text-align: center; 
    display: flex;
     align-items: center;
     justify-content: center;
     position: relative;
     bottom: 5px;
}
.text{
    color: white;
}
.About_us{
    padding: 0  50px ;
}
.gradient-line {
            width: 100%;
            height: 1px;
            background: linear-gradient(to right, rgba(255, 255, 255, 0), #f2b632, rgba(255, 255, 255, 0));
            margin: 20px 0; /* Adjust margin as needed */
        }
.span_blue{
    color: #2B7AF1;
}
.justify_center{
    display: flex; 
    justify-content: center;
}

</style>