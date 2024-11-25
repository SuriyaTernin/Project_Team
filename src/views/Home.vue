<template>
   <!-- ***** MENU ***** -->
  <div class="Home">
 <!-- ***** ICON ***** -->



  <!-- ***** Area ***** -->
 <div class="main-banner">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 align-self-center">
          <div class="caption header-text">
            <h6>สวัสดีครับ/ค่ะ ยินดีต้อนรับ</h6>
            <h2><b style="color: antiquewhite;"> DONUT SHOP </b></h2>
            <p>ยินดีต้อนรับสู่โลกแห่งความหวานที่เต็มไปด้วยโดนัทสดใหม่และรสชาติเยี่ยม!</p>
            <p>โดนัทของเราใช้วัตถุดิบคุณภาพเยี่ยม คัดสรรอย่างดีเพื่อให้คุณได้รับประสบการณ์การทานที่ดีที่สุด</p>
            <p>มาลองชิมโดนัทหลากหลายรสชาติของเรา และพบกับความสุขในทุกคำที่กัด!</p>


            <div class="search-input">
              <form id="search" action="#">
                <input type="text" placeholder="ค้นหาเมนูที่ท่านต้องการได้เลย!!" id='searchText' name="searchKeyword" onkeypress="handle" />
                <button role="button">Search Now</button>
              </form>
            </div>
          </div>
        </div>
        <div class="col-lg-4 offset-lg-2">
          <div class="right-image">
            <img src="../assets/Donut/5.png" alt="">
            <span class="price">$22</span>
            <span class="offer">-40%</span>
          </div>
        </div>
      </div>
    </div>
  </div>

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
            <h6>NEW</h6>
            <h2>โปรโมชั่นสุดพิเศษ</h2>
          </div>
        </div>
        <div class="col-lg-6">
        </div>
        <div class="col-lg-3 col-md-6">
          <div class="item">
            <div class="thumb">
              <img src="../assets/Donut/png/1.png" alt="">
              <span class="price"><em class="text-danger">$28</em>$20</span>
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
              <span class="price"><em class="text-danger">$39</em>$19</span>
            </div>
            <div class="down-content">
              <span class="category">โดนัท : รสช็อกโกแลต</span>
              <h4>เลือกเมนู</h4>
              <a href="#" class="select-menu"  @click="showAlert"><i class="fa fa-shopping-bag"></i></a>
            </div>
          </div>
        </div>
        <div class="col-lg-3 col-md-6">
          <div class="item">
            <div class="thumb">
              <img src="../assets/Donut/png/6.png" alt="">
              <span class="price"><em class="text-danger">$19</em>$10</span>
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
              <span class="price"><em class="text-danger">$64</em>$44</span>
            </div>
            <div class="down-content">
              <span class="category">โดนัท : ช็อกโกแลตใส่ท็อปปิ้ง</span>
              <h4>เลือกเมนู</h4>
              <a href="#" class="select-menu"  @click="showAlert"><i class="fa fa-shopping-bag"></i></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>



  <div class="section categories">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <div class="section-heading">
            <h2>สินค้าขายดี</h2>
          </div>
        </div>
        <div class="col-lg col-sm-6 col-xs-12">
          <div class="item">
            <h4>โดนัท : ช็อคโกแลต</h4>
            <div class="image-container">
            <img src="../assets/Donut/png/4.png" alt="">
          </div>
          </div>
        </div>
        <div class="col-lg col-sm-6 col-xs-12">
          <div class="item">
            <h4>โดนัท : คาราเมล</h4>
            <div class="image-container">
            <img src="../assets/Donut/png/1.png" alt="">
          </div>
          </div>
        </div>
        <div class="col-lg col-sm-6 col-xs-12">
          <div class="item">
            <h4>โดนัท : นมชมพู</h4>
            <div class="image-container">
            <img src="../assets/Donut/png/7.png" alt="">
          </div>
          </div>
        </div>
        <div class="col-lg col-sm-6 col-xs-12">
          <div class="item">
            <h4>โดนัท : น้ำตาล</h4>
            <div class="image-container">
            <img src="../assets/Donut/png/6.png" alt="">
          </div>
          </div>
        </div>
        <div class="col-lg col-sm-6 col-xs-12">
          <div class="item">
            <h4>โดนัท : นม</h4>
            <div class="image-container">
            <img src="../assets/Donut/png/9.png" alt="">
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
@import '../assets/css/home.css';
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

