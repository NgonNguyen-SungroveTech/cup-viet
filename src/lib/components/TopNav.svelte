<script>
  let listIcon = [
    {
      icon: "/icon/CUPVODICH-2.png",
      alt: "CUPVODICH",
      url: "/",
    },
    {
      icon: "/icon/CUPEAGEL-2.png",
      alt: "CUPEAGEL",
      url: "/",
    },
    {
      icon: "/icon/CUPGOLF-2.png",
      alt: "CUPGOLF",
      url: "/",
    },
    {
      icon: "/icon/CUPKYTHUAT-2.png",
      alt: "CUPKYTHUAT",
      url: "/category/cupkythuat",
    },
    {
      icon: "/icon/QUATANG-2.png",
      alt: "QUATANG",
      url: "/",
    },
    {
      icon: "/icon/HUYCHUONG-2.png",
      alt: "HUYCHUONG",
      url: "/",
    },
    {
      icon: "/icon/KINIEMCHUONG-2.png",
      alt: "KINIEMCHUONG",
      url: "/",
    },
  ];
</script>
<div class='top-nav flex justify-center mt-2 h-full'>
  <div class="sm:flex hidden w-[1200px]">
    <div class="flex justify-between items-center w-full">
      <a href="/">
        <img src="/images/logo.png" class='h-[90px] w-[250px]' atl="pig-logo"/>
      </a>
      {#each listIcon as { icon, alt, url }}
        <a href={url}>
          <img class="logo-header category_img" src={icon} alt={alt} />
        </a>
      {/each}
    </div>
    <!-- <form class='w-[300px] mt-3'>
      <div class="col-xs-2 search-wrap" style="float:right;">
        <input
          type="text"
          class="input-search py-2 !text-gray-800"
          placeholder="Tìm kiếm sản phẩm"
          autocomplete="off"
        />
        <img src="/images/ic-search.svg" alt="key search" />
      </div>
    </form> -->
  </div>
</div>

<style>

  .top-nav {
    padding: 10px 80px;
    background: #ffcd36;
    opacity: 0.9;
    margin-bottom: 10px;
  }
  .search-wrap {
    width: 100%;
    display: flex;
    align-items: center;
    border: none;
    border-radius: 30px;
    padding: 5px 15px;
    height: 40px;
    background: #f4d804;
  }
  .input-search {
    background: transparent;
    border: none;
    outline: none;
    width: 100%;
    height: 100%;
    font-size: 14px;
    font-weight: 400;
  }
  .bugger {
    position: relative;
    top: -2px;
    right: 0px;
    width: 15px;
    height: 15px;
    border: 0;
    display: inline-block;
    vertical-align: middle;
    transition: all 0.5s;
    z-index: 1;
  }

  .bugger i {
    height: 4px;
    width: 35px;
    position: absolute;
    top: calc(50% - 1px);
    left: 0px;
    background: #ffe766;
  }

  .bugger i:before {
    content: "";
    display: block;
    width: 30px;
    height: 3px;
    position: absolute;
    background: #000;
  }

  .bugger i:after {
    content: "";
    display: block;
    width: 40px;
    height: 4px;
    position: absolute;
    background: #000;
  }

  .bugger i:before {
    top: -9px;
  }

  .bugger i:after {
    bottom: -9px;
  }
  .category_img {
    width: 80px;
  }
</style>
