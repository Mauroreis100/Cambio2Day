<template>
    <div class="item">
      <i >
        <slot name="icon"></slot>
      </i>
      <div class="details">
        <h3>
          <slot name="heading"></slot>
        </h3>
        <slot></slot>
      </div>
    </div>
  </template>
  
  <style scoped>
  .item {
    margin: 2rem;
    display: flex;
    position: relative;
    align-content: center;
  }
  
  .details {
    flex: 1;
    align-content: center;
  }
  
  i {
    display: flex;
    flex: 1;
    place-items: center;
    place-content: center;
    width: 32px;
    height: 32px;
  
    color: var(--color-text);
  }
  
  h3 {
    font-size: 1.2rem;
    font-weight: 500;
    margin-bottom: 0.4rem;
    padding-left: 15px;
    color: var(--color-heading);
  }
  
  @media (min-width: 1024px) {
    .item {
    display: flex;
      margin-top: 20;
     
    }
  
    i {
      top: calc(50% - 25px);
      left: -26px;      
      border: 1px solid var(--color-border);
      background: var(--color-background);
      border-radius: 8px;
      width: 50px;
      height: 50px;
    }
  
    .item:before {
      content: ' ';
      border-left: 1px solid var(--color-border);
      position: absolute;
      left: 0;
      bottom: calc(50% + 25px);
      height: calc(50% - 25px);
    }
  
    .item:after {
      content: ' ';
      border-left: 1px solid var(--color-border);
      position: absolute;
      left: 0;
      top: calc(50% + 25px);
      height: calc(50% - 25px);
    }
  
    .item:first-of-type:before {
      display: none;
    }
  
    .item:last-of-type:after {
      display: none;
    }
  }
  </style>
  