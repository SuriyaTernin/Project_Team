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
        <router-link to="/About">
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
          <h2>ติดต่อ</h2>
        </div>
      </div>

      <!-- คอลัมน์ของข้อมูลนักศึกษา -->
      <div class="col-lg-6 col-md-12">
  <div class="student-info">
    <iframe 
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3880.9272011300823!2d100.99023347508421!3d13.41683318694101!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x311d3617ee04db97%3A0x2250cf181ed25837!2z4Lih4Lir4Liy4Lin4Li04LiX4Lii4Liy4Lil4Lix4Lii4Lio4Lij4Li14Lib4LiX4Li44LihIOC4p-C4tOC4l-C4ouC4suC5gOC4guC4leC4iuC4peC4muC4uOC4o-C4tQ!5e0!3m2!1sth!2sth!4v1732505798879!5m2!1sth!2sth" 
      width="100%" 
      height="450" 
      style="border: 0;" 
      allowfullscreen="" 
      loading="lazy" 
      referrerpolicy="no-referrer-when-downgrade">
    </iframe>
    <p>มหาวิทยาลัยศรีปทุม ชลบุรี 79 ถนนบางนา-ตราด ตำบลคลองตำหรุ อำเภอเมือง จังหวัดชลบุรี 20000 โทรศัพท์ 038-146-123 e-mail : computer@chonburi.spu.ac.th. Sripatum</p>
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
@import '../assets/css/contact.css';
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




