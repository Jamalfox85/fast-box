<template lang="">
  <div class="calculate_price_wrapper">
    <div class="inside_wrapper">
      <div class="inside_wrapper_left">
        <h2>Calculate your price</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad, nulla sit
          similique itaque error suscipit.
        </p>
        <img
          src="../assets/images/Delivery-address.png"
          class="inside_wrapper_left_img"
        />
      </div>
      <div class="inside_wrapper_right">
        <div class="form_wrapper">
          <div class="form-block">
            <div class="form-block-section-1">
              <div class="form-icon-block">
                <img
                  src="../assets/icons/calendar.svg"
                  class="form-icon-block"
                />
              </div>
              <h3 id="bookingDate">Booking Date</h3>
            </div>
            <div
              class="form-block-section-2"
              :style="{
                position: 'relative',
                display: 'flex',
                alignItems: 'center',
              }"
            >
              <input
                type="date"
                class="form-input"
                aria-labelledby="bookingDate"
                placeholder="Enter Booking Date"
              />
              <img
                src="../assets/icons/calendar-green.svg"
                class="input-triangle"
                :style="{ width: '1em', position: 'absolute', right: '1em' }"
              />
            </div>
          </div>
          <div class="form-block">
            <div class="form-block-section-1">
              <div class="form-icon-block">
                <img src="../assets/icons/box.svg" class="form-icon-block" />
              </div>
              <h3 id="bookingDate">Type of Parcel</h3>
            </div>
            <div
              class="form-block-section-2"
              :style="{
                position: 'relative',
                display: 'flex',
                alignItems: 'center',
              }"
            >
              <input
                type="text"
                class="form-input"
                aria-labelledby="bookingDate"
                placeholder="  Select Parcel Type"
              />
              <img
                src="../assets/icons/triangle.svg"
                class="input-triangle"
                :style="{ width: '1em', position: 'absolute', right: '1em' }"
              />
            </div>
          </div>
          <div class="form-block">
            <div class="form-block-section-1">
              <div class="form-icon-block">
                <img
                  src="../assets/icons/location-dot-solid.svg"
                  class="form-icon-block"
                />
              </div>
              <h3 id="bookingDate">Destination</h3>
            </div>
            <div class="form-block-section-2">
              <div
                :style="{
                  position: 'relative',
                  width: '50%',
                  display: 'flex',
                  alignItems: 'center',
                }"
              >
                <input
                  type="text"
                  class="form-input"
                  aria-labelledby="bookingDate"
                  placeholder="   To"
                />
                <img
                  src="../assets/icons/triangle.svg"
                  class="input-triangle"
                  :style="{ width: '1em', position: 'absolute', right: '1em' }"
                />
              </div>
              <div
                :style="{
                  position: 'relative',
                  width: '50%',
                  display: 'flex',
                  alignItems: 'center',
                }"
              >
                <input
                  type="text"
                  class="form-input"
                  aria-labelledby="bookingDate"
                  placeholder="   From"
                />
                <img
                  src="../assets/icons/triangle.svg"
                  class="input-triangle"
                  :style="{ width: '1em', position: 'absolute', right: '1em' }"
                />
              </div>
            </div>
          </div>
          <button class="form-cta">Calculate</button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.calculate_price_wrapper {
  height: 800px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 4em 0;
  .inside_wrapper {
    background-color: rgb(227, 248, 231);
    height: 90%;
    width: 75%;
    border-radius: 16px;
    display: flex;
    padding: 4em 7em;
    overflow: hidden;
    .inside_wrapper_left {
      display: flex;
      flex-direction: column;
      h2 {
        color: rgb(58, 86, 83);
        font-size: 3em;
        font-weight: bold;
      }
      p {
        color: #777;
        width: 65%;
      }
    }
    .inside_wrapper_right {
      width: 50%;
      .form_wrapper {
        background-color: #fff;
        height: 100%;
        width: 100%;
        border-radius: 12px;
        padding: 2em;
        .form-block {
          display: flex;
          flex-direction: column;
          .form-block-section-1 {
            display: flex;
            align-items: center;
            .form-icon-block {
              height: 2.75em;
              width: 2.75em;
              background-color: rgb(60, 189, 150);
              border-radius: 8px;
              display: flex;
              align-items: center;
              justify-content: center;
            }
            h3 {
              font-size: 1.25em;
              font-weight: bold;
              margin-left: 1em;
            }
          }
          .form-block-section-2 {
            display: flex;
            position: relative;
            .form-input {
              width: 100%;
              height: 2em;
              margin: 0.25em;
              color: #fff;
              box-shadow: 0 4px 4px rgba(204, 204, 204, 0.358);
              position: relative;
            }
            .form-input[type="date"]::-webkit-calendar-picker-indicator {
              display: none;
              -webkit-appearance: none;
            }
            .form-input[type="date"]:before {
              content: attr(placeholder) !important;
              color: #777;
              margin: 0.5em;
            }
            input[type="date"]:focus:before,
            input[type="date"]:valid:before {
              content: "";
            }
            .form-input[type="text"]::placeholder {
              color: #777;
              margin: 0.5em;
            }
          }
        }
        .form-cta {
          background-color: rgb(60, 189, 150);
          padding: 0 1.25em;
          border-radius: 8px;
          color: #fff;
          cursor: pointer;
          font-size: 16px;
          height: 2.75em;
          width: 8.5em;
          transition: 0.1s ease-in;
          &:hover {
            background-color: rgb(30, 146, 112);
          }
        }
      }
    }
  }
}
</style>
