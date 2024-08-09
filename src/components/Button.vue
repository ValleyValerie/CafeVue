<template>
    <button 
      class="outlined-button" 
      :class="{ disabled: isDisabled }"
      @click="handleClick"
      :disabled="isDisabled"
    >
      {{ text }}
    </button>
  </template>
  
  <script>
  export default {
    name: 'OutlinedButton',
    props: {
      text: {
        type: String,
        default: 'More'
      },
      isDisabled: {
        type: Boolean,
        default: false
      }
    },
    methods: {
      handleClick() {
        if (!this.isDisabled) {
          this.$emit('click')
        }
      }
    }
  }
  </script>
  
  <style scoped>
  .outlined-button {
    padding: 10px 10px;
    
    border: 2px solid #381b00;
    background-color: transparent;
    color: #381b00;
    border-radius: 25px;
    cursor: pointer;
    transition: all 0.3s ease;
    width: 40%;
  }
  
  .outlined-button:hover:not(.disabled) {
    background-color: #ffffff00;
    color: #381b00;
    transform: translateY(-5px);
  
  }

  @media (min-width: 1024px) {
            .lg\:text-2xl {
                font-size: 1.5rem /* 24px */;
                line-height: 2rem /* 32px */;
            }
        }

  @media (min-width: 640px) {
            .sm\:text-xl {
                font-size: 1.25rem /* 20px */;
                line-height: 1.75rem /* 28px */;
            }
        }
  
  .outlined-button.disabled {
    border-color: #381b00;
    color:#381b00;
    cursor: not-allowed;
  }
  </style>