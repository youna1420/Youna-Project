<template>
  <div class="card mb-4">
    <div class="card-header pb-0">
      <h6>{{ this.$store.state.isRTL ? 'صاحبین کسب و کار' : 'Business Owners'}}</h6>
    </div>
    <div class="card-body px-0 pt-0 pb-2">
      <div class="table-responsive p-0">
        <table class="table align-items-center mb-0">
          <thead>
            <tr>
              <th
                class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
              >
              {{ this.$store.state.isRTL ? 'نام' : 'Name' }}
              </th>
              <th
                class="text-uppercase text-secondary text-xxs font-weight-bolder opacity-7 ps-2"
              >
              {{ this.$store.state.isRTL ? 'حوزه فعالیت' : 'Function' }}
              </th>
              <th
                class="text-center text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
              >
              {{ this.$store.state.isRTL ? 'تماس' : 'Contact' }}
              </th>
              <th
                class="text-center text-uppercase text-secondary text-xxs font-weight-bolder opacity-7"
              >
              {{ this.$store.state.isRTL ? 'امتیاز' : 'Rating' }}
              </th>
              <th class="text-secondary opacity-7"></th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>
                <div class="d-flex px-2 py-1">
                  <div class="d-flex flex-column justify-content-center">
                    <h6 class="mb-0 text-sm">{{ this.$store.state.isRTL ? 'سورین اکسپورت' : 'Sorin Export' }}</h6>
                    <p class="text-xs text-secondary mb-0">
                      {{ this.$store.state.isRTL ? 'با مدیریت علی جهانی' : 'By Ali Jahani' }}
                    </p>
                  </div>
                </div>
              </td>
              <td>
                <p class="text-xs font-weight-bold mb-0">{{ this.$store.state.isRTL ? 'صادرات و واردات' : 'Import & Export' }}</p>
                <p class="text-xs text-secondary mb-0">{{ this.$store.state.isRTL ? 'روسیه' : 'Russian' }}</p>
              </td>
              <td class="align-middle text-center text-sm">
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-phone.png" style="height: 30px;"/>
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-mail.png" style="height: 30px;"/>
              </td>
              <td class="align-middle text-center">
                <div class="rate">
                  <input type="radio" id="star5" name="rate" value="5" />
                  <label for="star5" title="text">5 stars</label>
                  <input type="radio" id="star4" name="rate" value="4" />
                  <label for="star4" title="text">4 stars</label>
                  <input type="radio" id="star3" name="rate" value="3" />
                  <label for="star3" title="text">3 stars</label>
                  <input type="radio" id="star2" name="rate" value="2" />
                  <label for="star2" title="text">2 stars</label>
                  <input type="radio" id="star1" name="rate" value="1" />
                  <label for="star1" title="text">1 star</label>
                </div>
              </td>
              <td class="align-middle">
                <a
                  href="javascript:;"
                  class="text-secondary font-weight-bold text-xs"
                  data-toggle="tooltip"
                  data-original-title="{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }} user"
                  >{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }}</a
                >
              </td>
            </tr>
            <tr>
              <td>
                <div class="d-flex px-2 py-1">
                  <div class="d-flex flex-column justify-content-center">
                    <h6 class="mb-0 text-sm">{{ this.$store.state.isRTL ? 'سنگ هیرا' : 'Hira Stone' }}</h6>
                    <p class="text-xs text-secondary mb-0">
                      {{ this.$store.state.isRTL ? 'با مدیریت مانويل لی' : 'By Manuel Lee' }}
                    </p>
                  </div>
                </div>
              </td>
              <td>
                <p class="text-xs font-weight-bold mb-0">{{ this.$store.state.isRTL ? 'صنایع سنگ' : 'Stone Industry' }}</p>
                <p class="text-xs text-secondary mb-0">{{ this.$store.state.isRTL ? 'کانادا' : 'Canadian' }}</p>
              </td>
              <td class="align-middle text-center text-sm">
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-phone.png" style="height: 30px;"/>
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-mail.png" style="height: 30px;"/>
              </td>
              <td class="align-middle text-center">
                <div class="rate">
                  <input type="radio" id="star5" name="rate" value="5" />
                  <label for="star5" title="text">5 stars</label>
                  <input type="radio" id="star4" name="rate" value="4" />
                  <label for="star4" title="text">4 stars</label>
                  <input type="radio" id="star3" name="rate" value="3" />
                  <label for="star3" title="text">3 stars</label>
                  <input type="radio" id="star2" name="rate" value="2" />
                  <label for="star2" title="text">2 stars</label>
                  <input type="radio" id="star1" name="rate" value="1" />
                  <label for="star1" title="text">1 star</label>
                </div>
              </td>
              <td class="align-middle">
                <a
                  href="javascript:;"
                  class="text-secondary font-weight-bold text-xs"
                  data-toggle="tooltip"
                  data-original-title="{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }} user"
                  >{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }}</a
                >
              </td>
            </tr>
            <tr>
              <td>
                <div class="d-flex px-2 py-1">
                  <div class="d-flex flex-column justify-content-center">
                    <h6 class="mb-0 text-sm">{{ this.$store.state.isRTL ? 'کشاورزی قدیری' : 'Ghadiri agriculture' }}</h6>
                    <p class="text-xs text-secondary mb-0">
                      {{ this.$store.state.isRTL ? 'با مدیریت محمد قدیری' : 'By Mohammad Ghadiri' }}
                    </p>
                  </div>
                </div>
              </td>
              <td>
                <p class="text-xs font-weight-bold mb-0">{{ this.$store.state.isRTL ? 'صنایع کشاورزی' : 'Agriculture industry' }}</p>
                <p class="text-xs text-secondary mb-0">{{ this.$store.state.isRTL ? 'ایران' : 'Iranian' }}</p>
              </td>
              <td class="align-middle text-center text-sm">
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-phone.png" style="height: 30px;"/>
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-mail.png" style="height: 30px;"/>
              </td>
              <td class="align-middle text-center">
                <div class="rate">
                  <input type="radio" id="star5" name="rate" value="5" />
                  <label for="star5" title="text">5 stars</label>
                  <input type="radio" id="star4" name="rate" value="4" />
                  <label for="star4" title="text">4 stars</label>
                  <input type="radio" id="star3" name="rate" value="3" />
                  <label for="star3" title="text">3 stars</label>
                  <input type="radio" id="star2" name="rate" value="2" />
                  <label for="star2" title="text">2 stars</label>
                  <input type="radio" id="star1" name="rate" value="1" />
                  <label for="star1" title="text">1 star</label>
                </div>
              </td>
              <td class="align-middle">
                <a
                  href="javascript:;"
                  class="text-secondary font-weight-bold text-xs"
                  data-toggle="tooltip"
                  data-original-title="{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }} user"
                  >{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }}</a
                >
              </td>
            </tr>
            <tr>
              <td>
                <div class="d-flex px-2 py-1">
                  <div class="d-flex flex-column justify-content-center">
                    <h6 class="mb-0 text-sm">{{ this.$store.state.isRTL ? 'قطعات قطر' : 'Qatar Parts' }}</h6>
                    <p class="text-xs text-secondary mb-0">
                      {{ this.$store.state.isRTL ? 'با مدیریت محمد ال قطری' : 'By Mohammad Al Qatari' }}
                    </p>
                  </div>
                </div>
              </td>
              <td>
                <p class="text-xs font-weight-bold mb-0">{{ this.$store.state.isRTL ? 'طراحی و ساخت قطعات' : 'Parts Industry' }}</p>
                <p class="text-xs text-secondary mb-0">{{ this.$store.state.isRTL ? 'ایران' : 'Iranian' }}</p>
              </td>
              <td class="align-middle text-center text-sm">
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-phone.png" style="height: 30px;"/>
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-mail.png" style="height: 30px;"/>
              </td>
              <td class="align-middle text-center">
                <div class="rate">
                  <input type="radio" id="star5" name="rate" value="5" />
                  <label for="star5" title="text">5 stars</label>
                  <input type="radio" id="star4" name="rate" value="4" />
                  <label for="star4" title="text">4 stars</label>
                  <input type="radio" id="star3" name="rate" value="3" />
                  <label for="star3" title="text">3 stars</label>
                  <input type="radio" id="star2" name="rate" value="2" />
                  <label for="star2" title="text">2 stars</label>
                  <input type="radio" id="star1" name="rate" value="1" />
                  <label for="star1" title="text">1 star</label>
                </div>
              </td>
              <td class="align-middle">
                <a
                  href="javascript:;"
                  class="text-secondary font-weight-bold text-xs"
                  data-toggle="tooltip"
                  data-original-title="{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }} user"
                  >{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }}</a
                >
              </td>
            </tr>
            <tr>
              <td>
                <div class="d-flex px-2 py-1">
                  <div class="d-flex flex-column justify-content-center">
                    <h6 class="mb-0 text-sm">{{ this.$store.state.isRTL ? 'کشاورزی رضایی' : 'Rezaii agriculture' }}</h6>
                    <p class="text-xs text-secondary mb-0">
                      {{ this.$store.state.isRTL ? 'با مدیریت محمد رضایی' : 'By Mohammad Rezaii' }}
                    </p>
                  </div>
                </div>
              </td>
              <td>
                <p class="text-xs font-weight-bold mb-0">{{ this.$store.state.isRTL ? 'صنایع کشاورزی' : 'Agriculture industry' }}</p>
                <p class="text-xs text-secondary mb-0">{{ this.$store.state.isRTL ? 'ایران' : 'Iranian' }}</p>
              </td>
              <td class="align-middle text-center text-sm">
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-phone.png" style="height: 30px;"/>
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-mail.png" style="height: 30px;"/>
              </td>
              <td class="align-middle text-center">
                <div class="rate">
                  <input type="radio" id="star5" name="rate" value="5" />
                  <label for="star5" title="text">5 stars</label>
                  <input type="radio" id="star4" name="rate" value="4" />
                  <label for="star4" title="text">4 stars</label>
                  <input type="radio" id="star3" name="rate" value="3" />
                  <label for="star3" title="text">3 stars</label>
                  <input type="radio" id="star2" name="rate" value="2" />
                  <label for="star2" title="text">2 stars</label>
                  <input type="radio" id="star1" name="rate" value="1" />
                  <label for="star1" title="text">1 star</label>
                </div>
              </td>
              <td class="align-middle">
                <a
                  href="javascript:;"
                  class="text-secondary font-weight-bold text-xs"
                  data-toggle="tooltip"
                  data-original-title="{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }} user"
                  >{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }}</a
                >
              </td>
            </tr>
            <tr>
              <td>
                <div class="d-flex px-2 py-1">
                  <div class="d-flex flex-column justify-content-center">
                    <h6 class="mb-0 text-sm">{{ this.$store.state.isRTL ? 'چدن نیکبخت' : 'Nikbakht CastIron' }}</h6>
                    <p class="text-xs text-secondary mb-0">
                      {{ this.$store.state.isRTL ? 'با مدیریت محمد نیکبخت' : 'By Mohammad Nikbakht' }}
                    </p>
                  </div>
                </div>
              </td>
              <td>
                <p class="text-xs font-weight-bold mb-0">{{ this.$store.state.isRTL ? 'صنایع چدن' : 'Iron industry' }}</p>
                <p class="text-xs text-secondary mb-0">{{ this.$store.state.isRTL ? 'ایران' : 'Iranian' }}</p>
              </td>
              <td class="align-middle text-center text-sm">
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-phone.png" style="height: 30px;"/>
                <img src="https://img.icons8.com/ios-filled/50/82d61e/apple-mail.png" style="height: 30px;"/>
              </td>
              <td class="align-middle text-center">
                <div class="rate">
                  <input type="radio" id="star5" name="rate" value="5" />
                  <label for="star5" title="text">5 stars</label>
                  <input type="radio" id="star4" name="rate" value="4" />
                  <label for="star4" title="text">4 stars</label>
                  <input type="radio" id="star3" name="rate" value="3" />
                  <label for="star3" title="text">3 stars</label>
                  <input type="radio" id="star2" name="rate" value="2" />
                  <label for="star2" title="text">2 stars</label>
                  <input type="radio" id="star1" name="rate" value="1" />
                  <label for="star1" title="text">1 star</label>
                </div>
              </td>
              <td class="align-middle">
                <a
                  href="javascript:;"
                  class="text-secondary font-weight-bold text-xs"
                  data-toggle="tooltip"
                  data-original-title="{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }} user"
                  >{{ this.$store.state.isRTL ? 'مشاهده بیشتر' : 'See More' }}</a
                >
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: "authors-table",
  components: {
  },
};
</script>

<style>
.rate {
    height: 50px;
    padding-top: 5px;
}
.rate:not(:checked) > input {
    position:absolute;
    top:-9999px;
}
.rate:not(:checked) > label {
    width:1em;
    overflow:hidden;
    white-space:nowrap;
    cursor:pointer;
    font-size:20px;
    color:#ccc;
}
.rate:not(:checked) > label:before {
    content: '★ ';
}
.rate > input:checked ~ label {
    color: #ffc700;    
}
.rate:not(:checked) > label:hover,
.rate:not(:checked) > label:hover ~ label {
    color: #deb217;  
}
.rate > input:checked + label:hover,
.rate > input:checked + label:hover ~ label,
.rate > input:checked ~ label:hover,
.rate > input:checked ~ label:hover ~ label,
.rate > label:hover ~ input:checked ~ label {
    color: #c59b08;
}
</style>