<template>
  <div class="inner-form">
    <div class="input-field second-wrap">
      <input 
        id="search"
        v-model="inputValue"
        type="text"
        placeholder="I need to change the lamp" />
    </div>
    <div class="input-field third-wrap">
      <button 
        class="btn-search"
        type="button"
        @click="$emit('value',inputValue)">
        <svg class="svg-inline--fa fa-search fa-w-16" aria-hidden="true" data-prefix="fas" data-icon="search" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
          <path fill="currentColor" d="M505 442.7L405.3 343c-4.5-4.5-10.6-7-17-7H372c27.6-35.3 44-79.7 44-128C416 93.1 322.9 0 208 0S0 93.1 0 208s93.1 208 208 208c48.3 0 92.7-16.4 128-44v16.3c0 6.4 2.5 12.5 7 17l99.7 99.7c9.4 9.4 24.6 9.4 33.9 0l28.3-28.3c9.4-9.4 9.4-24.6.1-34zM208 336c-70.7 0-128-57.2-128-128 0-70.7 57.2-128 128-128 70.7 0 128 57.2 128 128 0 70.7-57.2 128-128 128z"></path>
        </svg>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'InputSearch',
  data: function() {
    return {
      inputValue: '',
    };
  }

}
</script>

<style>
.s003 form .inner-form .input-field {
  height: 68px;
}
.s003 form .inner-form .input-field input {
  height: 100%;
  background: transparent;
  border: 0;
  display: block;
  width: 100%;
  padding: 10px 32px;
  font-size: 16px;
  color: #555;
}

.s003 form .inner-form .input-field input.placeholder {
  color: #888;
  font-size: 16px;
}

.s003 form .inner-form .input-field input:-moz-placeholder {
  color: #888;
  font-size: 16px;
}

.s003 form .inner-form .input-field input::-webkit-input-placeholder {
  color: #888;
  font-size: 16px;
}

.s003 form .inner-form .input-field input:hover, .s003 form .inner-form .input-field input:focus {
  box-shadow: none;
  outline: 0;
  border-color: #fff;
}

.s003 form .inner-form .input-field.first-wrap {
  width: 200px;
  border-right: 1px solid rgba(0, 0, 0, 0.1);
}

.s003 form .inner-form .input-field.first-wrap .choices__inner {
  background: transparent;
  border-radius: 0;
  border: 0;
  height: 100%;
  color: #fff;
  display: -ms-flexbox;
  display: flex;
  -ms-flex-align: center;
      align-items: center;
  padding: 10px 30px;
}

.s003 form .inner-form .input-field.first-wrap .choices__inner .choices__list.choices__list--single {
  display: -ms-flexbox;
  display: flex;
  padding: 0;
  -ms-flex-align: center;
      align-items: center;
  height: 100%;
}

.s003 form .inner-form .input-field.first-wrap .choices__inner .choices__item.choices__item--selectable.choices__placeholder {
  display: -ms-flexbox;
  display: flex;
  -ms-flex-align: center;
      align-items: center;
  height: 100%;
  opacity: 1;
  color: #888;
}

.s003 form .inner-form .input-field.first-wrap .choices__inner .choices__list--single .choices__item {
  display: -ms-flexbox;
  display: flex;
  -ms-flex-align: center;
      align-items: center;
  height: 100%;
  color: #555;
}

.s003 form .inner-form .input-field.first-wrap .choices[data-type*="select-one"]:after {
  right: 30px;
  border-color: #e5e5e5 transparent transparent transparent;
}

.s003 form .inner-form .input-field.first-wrap .choices__list.choices__list--dropdown {
  border: 0;
  background: #fff;
  padding: 20px 30px;
  margin-top: 2px;
  border-radius: 4px;
  box-shadow: 0px 8px 20px 0px rgba(0, 0, 0, 0.15);
}

.s003 form .inner-form .input-field.first-wrap .choices__list.choices__list--dropdown .choices__item--selectable {
  padding-right: 0;
}

.s003 form .inner-form .input-field.first-wrap .choices__list--dropdown .choices__item--selectable.is-highlighted {
  background: #fff;
  color: #63c76a;
}

.s003 form .inner-form .input-field.first-wrap .choices__list--dropdown .choices__item {
  color: #555;
  min-height: 24px;
}

.s003 form .inner-form .input-field.second-wrap {
  -ms-flex-positive: 1;
      flex-grow: 1;
}

.s003 form .inner-form .input-field.third-wrap {
  width: 74px;
}

.s003 form .inner-form .input-field.third-wrap .btn-search {
  height: 100%;
  width: 100%;
  white-space: nowrap;
  color: #fff;
  border: 0;
  cursor: pointer;
  background: #63c76a;
  transition: all .2s ease-out, color .2s ease-out;
}

.s003 form .inner-form .input-field.third-wrap .btn-search svg {
  width: 16px;
}

.s003 form .inner-form .input-field.third-wrap .btn-search:hover {
  background: #50c058;
}

.s003 form .inner-form .input-field.third-wrap .btn-search:focus {
  outline: 0;
  box-shadow: none;
}

@media screen and (max-width: 992px) {
  .s003 form .inner-form .input-field {
    height: 50px;
  }
}

@media screen and (max-width: 767px) {
  .s003 form .inner-form {
    -ms-flex-wrap: wrap;
        flex-wrap: wrap;
    padding: 20px;
  }
  .s003 form .inner-form .input-field {
    margin-bottom: 20px;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
  }
  .s003 form .inner-form .input-field input {
    padding: 10px 15px;
  }
  .s003 form .inner-form .input-field.first-wrap {
    width: 100%;
    border-right: 0;
  }
  .s003 form .inner-form .input-field.first-wrap .choices__inner {
    padding: 10px 15px;
  }
  .s003 form .inner-form .input-field.first-wrap .choices[data-type*="select-one"]:after {
    right: 11.5px;
    border-color: #e5e5e5 transparent transparent transparent;
  }
  .s003 form .inner-form .input-field.second-wrap {
    width: 100%;
    margin-bottom: 30px;
  }
  .s003 form .inner-form .input-field.second-wrap input {
    border: 1px solid rgba(255, 255, 255, 0.3);
  }
  .s003 form .inner-form .input-field.third-wrap {
    margin-bottom: 0;
    width: 100%;
  }
}
</style>