<template>
  <div>
    <header class="navbar navbar-expand-lg navbar-dark bg-dark"  style="padding-top: 30px; padding-bottom: 30px; padding-left: 20px; padding-right: 20px;" >

        <div class="container-fluid">

        <!-- Icon di sebelah kiri -->
        <a class="navbar-brand" href="#">
        <img src="https://static.vecteezy.com/system/resources/previews/011/973/413/non_2x/cat-face-cute-free-download-transparent-image-illustration-clipart-pet-wildlife-free-png.png" alt="icon kucing" style="width: 50px; height: auto;">
        </a>

        <!-- Navbar -->
        <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
          <div class="container-fluid">
            <a class="navbar-brand" href="#">CURRICULUE VITAE</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
              <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
              <ul class="navbar-nav">
                <li class="nav-item">
                  <a class="nav-link" href="#" data-bs-toggle="modal" data-bs-target="#contactModal">Contact</a>
                </li>
              </ul>
            </div>
          </div>
        </nav>

        <!-- Modal -->
        <div class="modal fade" id="contactModal" tabindex="-1" aria-labelledby="contactModalLabel" aria-hidden="true">
          <div class="modal-dialog">
            <div class="modal-content">
              <div class="modal-header">
                <h5 class="modal-title" id="contactModalLabel">Contact Information</h5>
                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
              </div>
              <div class="modal-body">
                <p>Email: fatina0819@gmail.com</p>
                <p>Phone: +62 8 5763304788</p>
              </div>
              
            </div>
          </div>
        </div>

      </div>
    </header>

  <div class="container">
    <div class="left">
      <img src="/assets/wahyupict2.png" alt="Profile Picture"  class="boomerang">
    </div>

    <div class="right">
      <h1>{{ nama }}</h1>
      <h2>{{ npm  }}</h2>
      <h3>{{ disukai }}</h3>
      
      <p>{{ bio }}</p>
      <!-- Ikon Instagram -->
      <a href="https://www.instagram.com/wahyu_shiregaru/" target="_blank" class="icon instagram"><i class="fab fa-instagram"></i></a>
      <!-- Ikon GitHub -->
      <a href="https://github.com/Wahyusrg0819" target="_blank" class="icon github"><i class="fab fa-github"></i></a>
      <!--ikon reddit-->
      <a href="https://www.reddit.com/user/Wahyuu_srg/" target="_blank" class="icon reddit"><i class="fab fa-reddit"></i></a>
    </div>

  </div>

</div>

</template>


<script>
export default {
  data() {
    return {
      nama: 'Haii, Saya Wahyu Muliadi Siregar',
      npm: "Npm : 223510883",
      disukai: 'Badminton enthusiast',
      bio: 'Saya berasal dari Tapanuli Selatan, Sumatera Utara dan sedang kuliah di Universitas Islam Riau, Riau Pekan Baru. Saat ini Saya sedang berada dijenjang semester 5, Hobi saya adalah bermain Badminton, dan saya belum mempunya pengalaman pekerjaan😁🗿',
       
    }
  }
}
</script>

<style scoped>
/* Animasi untuk gambar naik dan turun */
@keyframes boomerang {
  0% { transform: translateY(0); } /* Posisi awal (tidak berubah) */
  50% { transform: translateY(-20px); } /* Posisi naik */
  100% { transform: translateY(0); } /* Posisi turun ke posisi awal */
}

/* Mengatur tampilan gambar */
.boomerang {
  animation: boomerang 2s ease-in-out infinite; /* Terapkan animasi boomerang */
}
</style>

