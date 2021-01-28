<script src="./js/jquery.nouislider.all.min.js"></script>
<script>
  // @formatter:off
  noUiSlider.create(document.getElementById('range-simple'),
  {
start: 20,
connect: [true, false],
step: 10,
range: {
min: 0,
max: 100
}
  });
  // @formatter:on
</script>
<script>
  // @formatter:off
  noUiSlider.create(document.getElementById('range-connect'), {
start: [60, 90],
connect: [false, true, false],
step: 10,
range: {
min: 0,
max: 100
}
  });
  // @formatter:on
</script>
<script>
  // @formatter:off
  noUiSlider.create(document.getElementById('range-color'), {
start: 40,
connect: [true, false],
step: 10,
range: {
min: 0,
max: 100
}
  });
  // @formatter:on
</script>
<script>
  document.addEventListener("DOMContentLoaded", function () {
flatpickr(document.getElementById('calendar-simple'), {

});
});
</script>
<script>
  document.addEventListener("DOMContentLoaded", function () 
{
flatpickr(document.getElementById('calendar-time'), {
});
});
</script>
<script>
  document.addEventListener("DOMContentLoaded", function () {
flatpickr(document.getElementById('calendar-inline'), {
inline: true,
});
});
</script>
<script>
  $(document).ready(function () {
$('#select-tags').selectize({
maxItems: 15,
});
});
</script>
<script>
  $(document).ready(function () {
$('#select-tags-advanced').selectize({
maxItems: 15,
plugins: ['remove_button'],
});
});
</script>
<script>
  $(document).ready(function () {
$('#select-users').selectize({
});
});
</script>
<script>
  $(document).ready(function () {
$('#select-people').selectize({
render: {
option: function (data, escape) {
return '<div class="option">' + data.avatar + '' + escape(data.text) + '</div>';
},
item: function (data, escape) {
return '<div class="d-flex align-items-center">' + data.avatar + '' + escape(data.text) + '</div>';
}
}
});
});
</script>
<script>
  $(document).ready(function () {
$('#select-countries').selectize({
render: {
option: function (data, escape) {
return '<div class="option"><span class="flag flag-country-' + data.flag + ' me-2"></span>' + escape(data.text) + '</div>';
 },
item: function (data, escape) {
return '<div class="d-flex align-items-center"><span class="flag flag-country-' + data.flag + ' me-2"></span>' + escape(data.text) + '</div>';
}
}
});
});
</script>
<script>
  $(document).ready(function () {
$('#select-states').selectize({
render: {
option: function (data, escape) {
return '<div class="option"><span class="flag flag-country-' + data.flag + ' me-2"></span>' + escape(data.text) + '</div>';
},
item: function (data, escape) {
return '<div class="d-flex align-items-center"><span class="flag flag-country-' + data.flag + ' me-2"></span>' + escape(data.text) + '</div>';
}
}
});
});
</script>
<script>
  let sliderTriggerList = [].slice.call(document.querySelectorAll("[data-slider]"));
  sliderTriggerList.map(function (sliderTriggerEl) 
{
let options = {};
if (sliderTriggerEl.getAttribute("data-slider")) {
options = JSON.parse(sliderTriggerEl.getAttribute("data-slider"));
}
let slider = noUiSlider.create(sliderTriggerEl, options);
if (options['js-name']) {
window[options['js-name']] = slider;
}
});
</script>

///////////////
<script src="./js/jquery.nouislider.all.min.js">

  // @formatter:off
  noUiSlider.create(document.getElementById('range-simple'),
  {
start: 20,
connect: [true, false],
step: 10,
range: {
min: 0,
max: 100
}
  });
  // @formatter:on

  // @formatter:off
  noUiSlider.create(document.getElementById('range-connect'), {
start: [60, 90],
connect: [false, true, false],
step: 10,
range: {
min: 0,
max: 100
}
  });
  // @formatter:on

  // @formatter:off
  noUiSlider.create(document.getElementById('range-color'), {
start: 40,
connect: [true, false],
step: 10,
range: {
min: 0,
max: 100
}
  });
  // @formatter:on

  document.addEventListener("DOMContentLoaded", function () {
flatpickr(document.getElementById('calendar-simple'), {

});
});

  document.addEventListener("DOMContentLoaded", function () 
{
flatpickr(document.getElementById('calendar-time'), {
});
});

  document.addEventListener("DOMContentLoaded", function () {
flatpickr(document.getElementById('calendar-inline'), {
inline: true,
});
});

  $(document).ready(function () {
$('#select-tags').selectize({
maxItems: 15,
});
});

  $(document).ready(function () {
$('#select-tags-advanced').selectize({
maxItems: 15,
plugins: ['remove_button'],
});
});

  $(document).ready(function () {
$('#select-users').selectize({
});
});

  $(document).ready(function () {
$('#select-people').selectize({
render: {
option: function (data, escape) {
return '<div class="option">' + data.avatar + '' + escape(data.text) + '</div>';
},
item: function (data, escape) {
return '<div class="d-flex align-items-center">' + data.avatar + '' + escape(data.text) + '</div>';
}
}
});
});

  $(document).ready(function () {
$('#select-countries').selectize({
render: {
option: function (data, escape) {
return '<div class="option"><span class="flag flag-country-' + data.flag + ' me-2"></span>' + escape(data.text) + '</div>';
 },
item: function (data, escape) {
return '<div class="d-flex align-items-center"><span class="flag flag-country-' + data.flag + ' me-2"></span>' + escape(data.text) + '</div>';
}
}
});
});

  $(document).ready(function () {
$('#select-states').selectize({
render: {
option: function (data, escape) {
return '<div class="option"><span class="flag flag-country-' + data.flag + ' me-2"></span>' + escape(data.text) + '</div>';
},
item: function (data, escape) {
return '<div class="d-flex align-items-center"><span class="flag flag-country-' + data.flag + ' me-2"></span>' + escape(data.text) + '</div>';
}
}
});
});

  let sliderTriggerList = [].slice.call(document.querySelectorAll("[data-slider]"));
  sliderTriggerList.map(function (sliderTriggerEl) 
{
let options = {};
if (sliderTriggerEl.getAttribute("data-slider")) {
options = JSON.parse(sliderTriggerEl.getAttribute("data-slider"));
}
let slider = noUiSlider.create(sliderTriggerEl, options);
if (options['js-name']) {
window[options['js-name']] = slider;
}
});
</script>

