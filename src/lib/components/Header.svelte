<script>
  import {modal} from '../../stores/modalStore.js';
  import PopupLong from '$lib/components/ui/PopupLong.svelte';

  const showPopup = () => {
    modal.set(PopupLong);
  };
</script>

<header class="top-area">
  <div class="header-area">
    <div class="container">
      <div class="row">
        <div class="col-sm-2">
          <div class="logo">
            <a href="index.html">
              tour<span>Nest</span>
            </a>
          </div><!-- /.logo-->
        </div><!-- /.col-->
        <div class="col-sm-10">
          <div class="main-menu">
            <!-- Brand and toggle get grouped for better mobile display -->
            <div class="navbar-header">
              <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse">
                <i class="fa fa-bars"></i>
              </button><!-- / button-->
            </div><!-- /.navbar-header-->
            <div class="collapse navbar-collapse">
              <ul class="nav navbar-nav navbar-right">
                <li class="smooth-menu"><a href="#home">home</a></li>
                <li class="smooth-menu"><a href="#gallery">Destination</a></li>
                <li class="smooth-menu"><a href="#pack">Packages </a></li>
                <li class="smooth-menu"><a href="#spo">Special Offers</a></li>
                <li class="smooth-menu"><a href="#blog">blog</a></li>
                <li class="smooth-menu"><a href="#subs">subscription</a></li>
                <li>
                  <button on:click={showPopup} class="book-btn">book now
                  </button>
                </li><!--/.project-btn-->
              </ul>
            </div><!-- /.navbar-collapse -->
          </div><!-- /.main-menu-->
        </div><!-- /.col-->
      </div><!-- /.row -->
      <div class="home-border"></div><!-- /.home-border-->
    </div><!-- /.container-->
  </div><!-- /.header-area -->

</header>
