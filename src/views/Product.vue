<template>
    <!-- ***** MENU ***** -->
   <div class="Product">
  <!-- ***** ICON ***** -->
 
 
 
   <!-- ***** Area ***** -->
 
   <div class="menu_detail">
     <div class="container">
       <div class="row">
        <div class="col-lg-3 col-md-6">
    <a href="#" @click="showPayment">
      <div class="item">
        <div class="icon-menu">
          <i class="fa-regular fa-credit-card fa-2x"></i>
        </div>
        <h4>ชำระเงิน</h4>
      </div>
    </a>
  </div>
  <div class="col-lg-3 col-md-6">
  <router-link to="/Product">
    <div class="item">
      <div class="icon-menu">
        <i class="fa-solid fa-bars fa-2x"></i>
      </div>
      <h4>เลือกเมนู</h4>
    </div>
  </router-link>
</div>

         <div class="col-lg-3 col-md-6">
    <a href="#" class="select-menu" @click="showPromotion">
      <div class="item">
        <div class="icon-menu">
          <i class="fa-regular fa-credit-card fa-2x"></i>
        </div>
        <h4>โปรโมชั่น</h4>
      </div>
    </a>
  </div>
         <div class="col-lg-3 col-md-6">
          <router-link to="/Contact">
             <div class="item">
               <div class="icon-menu">
                 <i class="fa-solid fa-user fa-2x"></i>
               </div>
               <h4>ติดต่อพนักงาน</h4>
             </div>
            </router-link>
         </div>
       </div>
     </div>
   </div>
 
   <div class="section trending most-played">
     <div class="container">
       <div class="row">
         <div class="col-lg-6">
           <div class="section-heading">
             <h2>รายการสินค้า</h2>
           </div>
         </div>
         <div class="col-lg-6">
         </div>
         <div class="col-lg-3 col-md-6">
           <div class="item">
             <div class="thumb">
               <img src="../assets/Donut/png/1.png" alt="">
             </div>
             <div class="down-content">
               <span class="category">โดนัท : รสครีม</span>
               <h4>เลือกเมนู</h4>
               <a href="#" class="select-menu"  @click="showAlert"><i class="fa fa-shopping-bag"></i></a>
             </div>
           </div>
         </div>
         <div class="col-lg-3 col-md-6">
           <div class="item">
             <div class="thumb">
               <img src="../assets/Donut/png/10.png" alt="">
             </div>
             <div class="down-content">
               <span class="category">โดนัท : รสช็อกโกแลต</span>
               <h4>เลือกเมนู</h4>
               <a href="#" class="select-menu" @click="showAlert"><i class="fa fa-shopping-bag"></i></a>
             </div>
           </div>
         </div>
         <div class="col-lg-3 col-md-6">
           <div class="item">
             <div class="thumb">
               <img src="../assets/Donut/png/6.png" alt="">
             </div>
             <div class="down-content">
               <span class="category">โดนัท : รสน้ำตาล</span>
               <h4>เลือกเมนู</h4>
               <a href="#" class="select-menu"  @click="showAlert"><i class="fa fa-shopping-bag"></i></a>
             </div>
           </div>
         </div>
         <div class="col-lg-3 col-md-6">
           <div class="item">
             <div class="thumb">
               <img src="../assets/Donut/png/4.png" alt="">
             </div>
             <div class="down-content">
               <span class="category">โดนัท : ช็อกโกแลตใส่ท็อปปิ้ง</span>
               <h4>เลือกเมนู</h4>
               <a href="#" class="select-menu"  @click="showAlert"><i class="fa fa-shopping-bag"></i></a>
             </div>
           </div>
         </div>
         <div class="col-lg-3 col-md-6">
           <div class="item">
             <div class="thumb">
               <img src="../assets/Donut/png/8.png" alt="">
             </div>
             <div class="down-content">
               <span class="category">โดนัท : นมฮอกไกโด</span>
               <h4>เลือกเมนู</h4>
               <a href="#" class="select-menu" @click="showAlert"><i class="fa fa-shopping-bag"></i></a>
             </div>
           </div>
         </div>
         <div class="col-lg-3 col-md-6">
           <div class="item">
             <div class="thumb">
               <img src="../assets/Donut/png/7.png" alt="">
             </div>
             <div class="down-content">
               <span class="category">โดนัท : นมชมพู</span>
               <h4>เลือกเมนู</h4>
               <a href="#" class="select-menu"  @click="showAlert"><i class="fa fa-shopping-bag"></i></a>
             </div>
           </div>
         </div>
         <div class="col-lg-3 col-md-6">
           <div class="item">
             <div class="thumb">
               <img src="../assets/Donut/png/5.png" alt="">
             </div>
             <div class="down-content">
               <span class="category">โดนัท : ครีมใส่ท็อปปิ้ง</span>
               <h4>เลือกเมนู</h4>
               <a href="#" class="select-menu"  @click="showAlert"><i class="fa fa-shopping-bag"></i></a>
             </div>
           </div>
         </div>
         <div class="col-lg-3 col-md-6">
           <div class="item">
             <div class="thumb">
               <img src="../assets/Donut/png/2.png" alt="">
             </div>
             <div class="down-content">
               <span class="category">โดนัท : เรนโบว์</span>
               <h4>เลือกเมนู</h4>
               <a href="#" class="select-menu"  @click="showAlert"><i class="fa fa-shopping-bag"></i></a>
             </div>
           </div>
         </div>

       </div>
       
     </div>
   </div>
   
 
   <footer>
     <div class="container">
       <div class="col-lg-12">
         <p>Sripatum University at Chonburi | มหาวิทยาลัยศรีปทุม ชลบุรี <br>
  <a href="http://www.chonburi.spu.ac.th" target="_blank" rel="noopener noreferrer"> www.chonburi.spu.ac.th</a></p>
       </div>
     </div>
   </footer>
   </div>
 </template>
 
 <style>
 @import '../assets/css/product.css';
 </style>
 
 <script>
 import Swal from "sweetalert2";
 
 export default {
  name: 'PromotionItem',
  methods: {
    showAlert(event) {
      event.preventDefault(); 
      Swal.fire({
        title: "เพิ่มสินค้าในตะกร้า!",
        text: "คุณต้องการเพิ่มเมนูนี้ในตะกร้าหรือไม่?",
        icon: "question",
        showCancelButton: true,
        confirmButtonText: "เพิ่ม",
        cancelButtonText: "ยกเลิก",
      }).then((result) => {
        if (result.isConfirmed) {
          Swal.fire("สำเร็จ!", "เมนูนี้ถูกเพิ่มในตะกร้าเรียบร้อยแล้ว", "success");
        }
      });
    },
    showPromotion(event) {
      event.preventDefault(); 

      Swal.fire({
        title: 'โปรโมชั่นส่วนลด!',
        text: 'ลด 10% สำหรับการสั่งซื้อทุกๆ 100 บาท',
        icon: 'info',
        confirmButtonText: 'รับโปรโมชั่น',
      }).then((result) => {
        if (result.isConfirmed) {
          Swal.fire("สำเร็จ!", "คุณได้รับโปรโมชั่นแล้ว", "success");
        }
      });
    },
    showPayment(event) {
      event.preventDefault(); 

      Swal.fire({
        title: 'ชำระเงิน',
        text: 'กสิกร : 077XXX3156',
        icon: 'warning',
        confirmButtonText: 'ชำระเงินสำเร็จ',
        cancelButtonText: 'ยกเลิก',
        showCancelButton: true,
      }).then((result) => {
        if (result.isConfirmed) {
          Swal.fire("สำเร็จ!", "ขอบคุณที่ใช้บริการ", "success");
          // ที่นี่คุณสามารถเพิ่มโค้ดเพื่อไปยังหน้าชำระเงินจริง ๆ เช่นการใช้ router หรือ redirection
        }
      });
    }
  }
};
 </script>



 
 