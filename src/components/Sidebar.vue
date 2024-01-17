<script setup>
</script>

<template>
  <div class="sidebar">
    <div class="logo">
      <img src="/assets/img/logo.svg" alt="logo" class="logo__image">
      <span class="logo__text">
        <span class="logo__text__title">Dashboard</span>
        <span class="logo__text__version">v.01</span>
      </span>
    </div>

    <div class="navigation">
      <ul class="navigation__list">
        <li class="navigation__item">
          <a href="#" class="navigation__item__link">
            <img src="/assets/img/menu/dashboard-icon.svg" alt="dashboard">
            <span>Dashboard</span>
          </a>
        </li>
        <li class="navigation__item">
          <a href="#" class="navigation__item__link">
            <img src="/assets/img/menu/product-icon.svg" alt="product">
            <span>Product</span>
          </a>
        </li>
        <li class="navigation__item">
          <a href="#" class="navigation__item__link navigation__item__link--active">
            <img src="/assets/img/menu/customer-icon.svg" alt="customer">
            <span>Customers</span>
          </a>
        </li>
        <li class="navigation__item">
          <a href="#" class="navigation__item__link">
            <img src="/assets/img/menu/income-icon.svg" alt="Income">
            <span>Income</span>
          </a>
        </li>
        <li class="navigation__item">
          <a href="#" class="navigation__item__link">
            <img src="/assets/img/menu/promote-icon.svg" alt="Promote">
            <span>Promote</span>
          </a>
        </li>
        <li class="navigation__item">
          <a href="#" class="navigation__item__link">
            <img src="/assets/img/menu/help-icon.svg" alt="Help">
            <span>Help</span>
          </a>
        </li>
      </ul>
    </div>
    
    <div class="user">
      <img src="/assets/img/user-01.png" alt="user" class="user__img">
      <div class="user__info">
        <div class="user__info__name">Evano</div>
        <div class="user__info__position">Project Manager</div>
      </div>
    </div>
  </div>
</template>

<style>

</style>
