<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />

<title>Whats in your beer_</title>

<script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>



<style type="text/css">
    /*!
*
* Twitter Bootstrap
*
*/
/*!
 * Bootstrap v3.3.7 (http://getbootstrap.com)
 * Copyright 2011-2016 Twitter, Inc.
 * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
 */
/*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
html {
  font-family: sans-serif;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
}
body {
  margin: 0;
}
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
main,
menu,
nav,
section,
summary {
  display: block;
}
audio,
canvas,
progress,
video {
  display: inline-block;
  vertical-align: baseline;
}
audio:not([controls]) {
  display: none;
  height: 0;
}
[hidden],
template {
  display: none;
}
a {
  background-color: transparent;
}
a:active,
a:hover {
  outline: 0;
}
abbr[title] {
  border-bottom: 1px dotted;
}
b,
strong {
  font-weight: bold;
}
dfn {
  font-style: italic;
}
h1 {
  font-size: 2em;
  margin: 0.67em 0;
}
mark {
  background: #ff0;
  color: #000;
}
small {
  font-size: 80%;
}
sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}
sup {
  top: -0.5em;
}
sub {
  bottom: -0.25em;
}
img {
  border: 0;
}
svg:not(:root) {
  overflow: hidden;
}
figure {
  margin: 1em 40px;
}
hr {
  box-sizing: content-box;
  height: 0;
}
pre {
  overflow: auto;
}
code,
kbd,
pre,
samp {
  font-family: monospace, monospace;
  font-size: 1em;
}
button,
input,
optgroup,
select,
textarea {
  color: inherit;
  font: inherit;
  margin: 0;
}
button {
  overflow: visible;
}
button,
select {
  text-transform: none;
}
button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
  -webkit-appearance: button;
  cursor: pointer;
}
button[disabled],
html input[disabled] {
  cursor: default;
}
button::-moz-focus-inner,
input::-moz-focus-inner {
  border: 0;
  padding: 0;
}
input {
  line-height: normal;
}
input[type="checkbox"],
input[type="radio"] {
  box-sizing: border-box;
  padding: 0;
}
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: textfield;
  box-sizing: content-box;
}
input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}
fieldset {
  border: 1px solid #c0c0c0;
  margin: 0 2px;
  padding: 0.35em 0.625em 0.75em;
}
legend {
  border: 0;
  padding: 0;
}
textarea {
  overflow: auto;
}
optgroup {
  font-weight: bold;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
td,
th {
  padding: 0;
}
/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
@media print {
  *,
  *:before,
  *:after {
    background: transparent !important;
    box-shadow: none !important;
    text-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  abbr[title]:after {
    content: " (" attr(title) ")";
  }
  a[href^="#"]:after,
  a[href^="javascript:"]:after {
    content: "";
  }
  pre,
  blockquote {
    border: 1px solid #999;
    page-break-inside: avoid;
  }
  thead {
    display: table-header-group;
  }
  tr,
  img {
    page-break-inside: avoid;
  }
  img {
    max-width: 100% !important;
  }
  p,
  h2,
  h3 {
    orphans: 3;
    widows: 3;
  }
  h2,
  h3 {
    page-break-after: avoid;
  }
  .navbar {
    display: none;
  }
  .btn > .caret,
  .dropup > .btn > .caret {
    border-top-color: #000 !important;
  }
  .label {
    border: 1px solid #000;
  }
  .table {
    border-collapse: collapse !important;
  }
  .table td,
  .table th {
    background-color: #fff !important;
  }
  .table-bordered th,
  .table-bordered td {
    border: 1px solid #ddd !important;
  }
}
@font-face {
  font-family: 'Glyphicons Halflings';
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot');
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff') format('woff'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
}
.glyphicon {
  position: relative;
  top: 1px;
  display: inline-block;
  font-family: 'Glyphicons Halflings';
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.glyphicon-asterisk:before {
  content: "\002a";
}
.glyphicon-plus:before {
  content: "\002b";
}
.glyphicon-euro:before,
.glyphicon-eur:before {
  content: "\20ac";
}
.glyphicon-minus:before {
  content: "\2212";
}
.glyphicon-cloud:before {
  content: "\2601";
}
.glyphicon-envelope:before {
  content: "\2709";
}
.glyphicon-pencil:before {
  content: "\270f";
}
.glyphicon-glass:before {
  content: "\e001";
}
.glyphicon-music:before {
  content: "\e002";
}
.glyphicon-search:before {
  content: "\e003";
}
.glyphicon-heart:before {
  content: "\e005";
}
.glyphicon-star:before {
  content: "\e006";
}
.glyphicon-star-empty:before {
  content: "\e007";
}
.glyphicon-user:before {
  content: "\e008";
}
.glyphicon-film:before {
  content: "\e009";
}
.glyphicon-th-large:before {
  content: "\e010";
}
.glyphicon-th:before {
  content: "\e011";
}
.glyphicon-th-list:before {
  content: "\e012";
}
.glyphicon-ok:before {
  content: "\e013";
}
.glyphicon-remove:before {
  content: "\e014";
}
.glyphicon-zoom-in:before {
  content: "\e015";
}
.glyphicon-zoom-out:before {
  content: "\e016";
}
.glyphicon-off:before {
  content: "\e017";
}
.glyphicon-signal:before {
  content: "\e018";
}
.glyphicon-cog:before {
  content: "\e019";
}
.glyphicon-trash:before {
  content: "\e020";
}
.glyphicon-home:before {
  content: "\e021";
}
.glyphicon-file:before {
  content: "\e022";
}
.glyphicon-time:before {
  content: "\e023";
}
.glyphicon-road:before {
  content: "\e024";
}
.glyphicon-download-alt:before {
  content: "\e025";
}
.glyphicon-download:before {
  content: "\e026";
}
.glyphicon-upload:before {
  content: "\e027";
}
.glyphicon-inbox:before {
  content: "\e028";
}
.glyphicon-play-circle:before {
  content: "\e029";
}
.glyphicon-repeat:before {
  content: "\e030";
}
.glyphicon-refresh:before {
  content: "\e031";
}
.glyphicon-list-alt:before {
  content: "\e032";
}
.glyphicon-lock:before {
  content: "\e033";
}
.glyphicon-flag:before {
  content: "\e034";
}
.glyphicon-headphones:before {
  content: "\e035";
}
.glyphicon-volume-off:before {
  content: "\e036";
}
.glyphicon-volume-down:before {
  content: "\e037";
}
.glyphicon-volume-up:before {
  content: "\e038";
}
.glyphicon-qrcode:before {
  content: "\e039";
}
.glyphicon-barcode:before {
  content: "\e040";
}
.glyphicon-tag:before {
  content: "\e041";
}
.glyphicon-tags:before {
  content: "\e042";
}
.glyphicon-book:before {
  content: "\e043";
}
.glyphicon-bookmark:before {
  content: "\e044";
}
.glyphicon-print:before {
  content: "\e045";
}
.glyphicon-camera:before {
  content: "\e046";
}
.glyphicon-font:before {
  content: "\e047";
}
.glyphicon-bold:before {
  content: "\e048";
}
.glyphicon-italic:before {
  content: "\e049";
}
.glyphicon-text-height:before {
  content: "\e050";
}
.glyphicon-text-width:before {
  content: "\e051";
}
.glyphicon-align-left:before {
  content: "\e052";
}
.glyphicon-align-center:before {
  content: "\e053";
}
.glyphicon-align-right:before {
  content: "\e054";
}
.glyphicon-align-justify:before {
  content: "\e055";
}
.glyphicon-list:before {
  content: "\e056";
}
.glyphicon-indent-left:before {
  content: "\e057";
}
.glyphicon-indent-right:before {
  content: "\e058";
}
.glyphicon-facetime-video:before {
  content: "\e059";
}
.glyphicon-picture:before {
  content: "\e060";
}
.glyphicon-map-marker:before {
  content: "\e062";
}
.glyphicon-adjust:before {
  content: "\e063";
}
.glyphicon-tint:before {
  content: "\e064";
}
.glyphicon-edit:before {
  content: "\e065";
}
.glyphicon-share:before {
  content: "\e066";
}
.glyphicon-check:before {
  content: "\e067";
}
.glyphicon-move:before {
  content: "\e068";
}
.glyphicon-step-backward:before {
  content: "\e069";
}
.glyphicon-fast-backward:before {
  content: "\e070";
}
.glyphicon-backward:before {
  content: "\e071";
}
.glyphicon-play:before {
  content: "\e072";
}
.glyphicon-pause:before {
  content: "\e073";
}
.glyphicon-stop:before {
  content: "\e074";
}
.glyphicon-forward:before {
  content: "\e075";
}
.glyphicon-fast-forward:before {
  content: "\e076";
}
.glyphicon-step-forward:before {
  content: "\e077";
}
.glyphicon-eject:before {
  content: "\e078";
}
.glyphicon-chevron-left:before {
  content: "\e079";
}
.glyphicon-chevron-right:before {
  content: "\e080";
}
.glyphicon-plus-sign:before {
  content: "\e081";
}
.glyphicon-minus-sign:before {
  content: "\e082";
}
.glyphicon-remove-sign:before {
  content: "\e083";
}
.glyphicon-ok-sign:before {
  content: "\e084";
}
.glyphicon-question-sign:before {
  content: "\e085";
}
.glyphicon-info-sign:before {
  content: "\e086";
}
.glyphicon-screenshot:before {
  content: "\e087";
}
.glyphicon-remove-circle:before {
  content: "\e088";
}
.glyphicon-ok-circle:before {
  content: "\e089";
}
.glyphicon-ban-circle:before {
  content: "\e090";
}
.glyphicon-arrow-left:before {
  content: "\e091";
}
.glyphicon-arrow-right:before {
  content: "\e092";
}
.glyphicon-arrow-up:before {
  content: "\e093";
}
.glyphicon-arrow-down:before {
  content: "\e094";
}
.glyphicon-share-alt:before {
  content: "\e095";
}
.glyphicon-resize-full:before {
  content: "\e096";
}
.glyphicon-resize-small:before {
  content: "\e097";
}
.glyphicon-exclamation-sign:before {
  content: "\e101";
}
.glyphicon-gift:before {
  content: "\e102";
}
.glyphicon-leaf:before {
  content: "\e103";
}
.glyphicon-fire:before {
  content: "\e104";
}
.glyphicon-eye-open:before {
  content: "\e105";
}
.glyphicon-eye-close:before {
  content: "\e106";
}
.glyphicon-warning-sign:before {
  content: "\e107";
}
.glyphicon-plane:before {
  content: "\e108";
}
.glyphicon-calendar:before {
  content: "\e109";
}
.glyphicon-random:before {
  content: "\e110";
}
.glyphicon-comment:before {
  content: "\e111";
}
.glyphicon-magnet:before {
  content: "\e112";
}
.glyphicon-chevron-up:before {
  content: "\e113";
}
.glyphicon-chevron-down:before {
  content: "\e114";
}
.glyphicon-retweet:before {
  content: "\e115";
}
.glyphicon-shopping-cart:before {
  content: "\e116";
}
.glyphicon-folder-close:before {
  content: "\e117";
}
.glyphicon-folder-open:before {
  content: "\e118";
}
.glyphicon-resize-vertical:before {
  content: "\e119";
}
.glyphicon-resize-horizontal:before {
  content: "\e120";
}
.glyphicon-hdd:before {
  content: "\e121";
}
.glyphicon-bullhorn:before {
  content: "\e122";
}
.glyphicon-bell:before {
  content: "\e123";
}
.glyphicon-certificate:before {
  content: "\e124";
}
.glyphicon-thumbs-up:before {
  content: "\e125";
}
.glyphicon-thumbs-down:before {
  content: "\e126";
}
.glyphicon-hand-right:before {
  content: "\e127";
}
.glyphicon-hand-left:before {
  content: "\e128";
}
.glyphicon-hand-up:before {
  content: "\e129";
}
.glyphicon-hand-down:before {
  content: "\e130";
}
.glyphicon-circle-arrow-right:before {
  content: "\e131";
}
.glyphicon-circle-arrow-left:before {
  content: "\e132";
}
.glyphicon-circle-arrow-up:before {
  content: "\e133";
}
.glyphicon-circle-arrow-down:before {
  content: "\e134";
}
.glyphicon-globe:before {
  content: "\e135";
}
.glyphicon-wrench:before {
  content: "\e136";
}
.glyphicon-tasks:before {
  content: "\e137";
}
.glyphicon-filter:before {
  content: "\e138";
}
.glyphicon-briefcase:before {
  content: "\e139";
}
.glyphicon-fullscreen:before {
  content: "\e140";
}
.glyphicon-dashboard:before {
  content: "\e141";
}
.glyphicon-paperclip:before {
  content: "\e142";
}
.glyphicon-heart-empty:before {
  content: "\e143";
}
.glyphicon-link:before {
  content: "\e144";
}
.glyphicon-phone:before {
  content: "\e145";
}
.glyphicon-pushpin:before {
  content: "\e146";
}
.glyphicon-usd:before {
  content: "\e148";
}
.glyphicon-gbp:before {
  content: "\e149";
}
.glyphicon-sort:before {
  content: "\e150";
}
.glyphicon-sort-by-alphabet:before {
  content: "\e151";
}
.glyphicon-sort-by-alphabet-alt:before {
  content: "\e152";
}
.glyphicon-sort-by-order:before {
  content: "\e153";
}
.glyphicon-sort-by-order-alt:before {
  content: "\e154";
}
.glyphicon-sort-by-attributes:before {
  content: "\e155";
}
.glyphicon-sort-by-attributes-alt:before {
  content: "\e156";
}
.glyphicon-unchecked:before {
  content: "\e157";
}
.glyphicon-expand:before {
  content: "\e158";
}
.glyphicon-collapse-down:before {
  content: "\e159";
}
.glyphicon-collapse-up:before {
  content: "\e160";
}
.glyphicon-log-in:before {
  content: "\e161";
}
.glyphicon-flash:before {
  content: "\e162";
}
.glyphicon-log-out:before {
  content: "\e163";
}
.glyphicon-new-window:before {
  content: "\e164";
}
.glyphicon-record:before {
  content: "\e165";
}
.glyphicon-save:before {
  content: "\e166";
}
.glyphicon-open:before {
  content: "\e167";
}
.glyphicon-saved:before {
  content: "\e168";
}
.glyphicon-import:before {
  content: "\e169";
}
.glyphicon-export:before {
  content: "\e170";
}
.glyphicon-send:before {
  content: "\e171";
}
.glyphicon-floppy-disk:before {
  content: "\e172";
}
.glyphicon-floppy-saved:before {
  content: "\e173";
}
.glyphicon-floppy-remove:before {
  content: "\e174";
}
.glyphicon-floppy-save:before {
  content: "\e175";
}
.glyphicon-floppy-open:before {
  content: "\e176";
}
.glyphicon-credit-card:before {
  content: "\e177";
}
.glyphicon-transfer:before {
  content: "\e178";
}
.glyphicon-cutlery:before {
  content: "\e179";
}
.glyphicon-header:before {
  content: "\e180";
}
.glyphicon-compressed:before {
  content: "\e181";
}
.glyphicon-earphone:before {
  content: "\e182";
}
.glyphicon-phone-alt:before {
  content: "\e183";
}
.glyphicon-tower:before {
  content: "\e184";
}
.glyphicon-stats:before {
  content: "\e185";
}
.glyphicon-sd-video:before {
  content: "\e186";
}
.glyphicon-hd-video:before {
  content: "\e187";
}
.glyphicon-subtitles:before {
  content: "\e188";
}
.glyphicon-sound-stereo:before {
  content: "\e189";
}
.glyphicon-sound-dolby:before {
  content: "\e190";
}
.glyphicon-sound-5-1:before {
  content: "\e191";
}
.glyphicon-sound-6-1:before {
  content: "\e192";
}
.glyphicon-sound-7-1:before {
  content: "\e193";
}
.glyphicon-copyright-mark:before {
  content: "\e194";
}
.glyphicon-registration-mark:before {
  content: "\e195";
}
.glyphicon-cloud-download:before {
  content: "\e197";
}
.glyphicon-cloud-upload:before {
  content: "\e198";
}
.glyphicon-tree-conifer:before {
  content: "\e199";
}
.glyphicon-tree-deciduous:before {
  content: "\e200";
}
.glyphicon-cd:before {
  content: "\e201";
}
.glyphicon-save-file:before {
  content: "\e202";
}
.glyphicon-open-file:before {
  content: "\e203";
}
.glyphicon-level-up:before {
  content: "\e204";
}
.glyphicon-copy:before {
  content: "\e205";
}
.glyphicon-paste:before {
  content: "\e206";
}
.glyphicon-alert:before {
  content: "\e209";
}
.glyphicon-equalizer:before {
  content: "\e210";
}
.glyphicon-king:before {
  content: "\e211";
}
.glyphicon-queen:before {
  content: "\e212";
}
.glyphicon-pawn:before {
  content: "\e213";
}
.glyphicon-bishop:before {
  content: "\e214";
}
.glyphicon-knight:before {
  content: "\e215";
}
.glyphicon-baby-formula:before {
  content: "\e216";
}
.glyphicon-tent:before {
  content: "\26fa";
}
.glyphicon-blackboard:before {
  content: "\e218";
}
.glyphicon-bed:before {
  content: "\e219";
}
.glyphicon-apple:before {
  content: "\f8ff";
}
.glyphicon-erase:before {
  content: "\e221";
}
.glyphicon-hourglass:before {
  content: "\231b";
}
.glyphicon-lamp:before {
  content: "\e223";
}
.glyphicon-duplicate:before {
  content: "\e224";
}
.glyphicon-piggy-bank:before {
  content: "\e225";
}
.glyphicon-scissors:before {
  content: "\e226";
}
.glyphicon-bitcoin:before {
  content: "\e227";
}
.glyphicon-btc:before {
  content: "\e227";
}
.glyphicon-xbt:before {
  content: "\e227";
}
.glyphicon-yen:before {
  content: "\00a5";
}
.glyphicon-jpy:before {
  content: "\00a5";
}
.glyphicon-ruble:before {
  content: "\20bd";
}
.glyphicon-rub:before {
  content: "\20bd";
}
.glyphicon-scale:before {
  content: "\e230";
}
.glyphicon-ice-lolly:before {
  content: "\e231";
}
.glyphicon-ice-lolly-tasted:before {
  content: "\e232";
}
.glyphicon-education:before {
  content: "\e233";
}
.glyphicon-option-horizontal:before {
  content: "\e234";
}
.glyphicon-option-vertical:before {
  content: "\e235";
}
.glyphicon-menu-hamburger:before {
  content: "\e236";
}
.glyphicon-modal-window:before {
  content: "\e237";
}
.glyphicon-oil:before {
  content: "\e238";
}
.glyphicon-grain:before {
  content: "\e239";
}
.glyphicon-sunglasses:before {
  content: "\e240";
}
.glyphicon-text-size:before {
  content: "\e241";
}
.glyphicon-text-color:before {
  content: "\e242";
}
.glyphicon-text-background:before {
  content: "\e243";
}
.glyphicon-object-align-top:before {
  content: "\e244";
}
.glyphicon-object-align-bottom:before {
  content: "\e245";
}
.glyphicon-object-align-horizontal:before {
  content: "\e246";
}
.glyphicon-object-align-left:before {
  content: "\e247";
}
.glyphicon-object-align-vertical:before {
  content: "\e248";
}
.glyphicon-object-align-right:before {
  content: "\e249";
}
.glyphicon-triangle-right:before {
  content: "\e250";
}
.glyphicon-triangle-left:before {
  content: "\e251";
}
.glyphicon-triangle-bottom:before {
  content: "\e252";
}
.glyphicon-triangle-top:before {
  content: "\e253";
}
.glyphicon-console:before {
  content: "\e254";
}
.glyphicon-superscript:before {
  content: "\e255";
}
.glyphicon-subscript:before {
  content: "\e256";
}
.glyphicon-menu-left:before {
  content: "\e257";
}
.glyphicon-menu-right:before {
  content: "\e258";
}
.glyphicon-menu-down:before {
  content: "\e259";
}
.glyphicon-menu-up:before {
  content: "\e260";
}
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
*:before,
*:after {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
html {
  font-size: 10px;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  line-height: 1.42857143;
  color: #000;
  background-color: #fff;
}
input,
button,
select,
textarea {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
a {
  color: #337ab7;
  text-decoration: none;
}
a:hover,
a:focus {
  color: #23527c;
  text-decoration: underline;
}
a:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
figure {
  margin: 0;
}
img {
  vertical-align: middle;
}
.img-responsive,
.thumbnail > img,
.thumbnail a > img,
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  display: block;
  max-width: 100%;
  height: auto;
}
.img-rounded {
  border-radius: 3px;
}
.img-thumbnail {
  padding: 4px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
  display: inline-block;
  max-width: 100%;
  height: auto;
}
.img-circle {
  border-radius: 50%;
}
hr {
  margin-top: 18px;
  margin-bottom: 18px;
  border: 0;
  border-top: 1px solid #eeeeee;
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  padding: 0;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
[role="button"] {
  cursor: pointer;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  font-family: inherit;
  font-weight: 500;
  line-height: 1.1;
  color: inherit;
}
h1 small,
h2 small,
h3 small,
h4 small,
h5 small,
h6 small,
.h1 small,
.h2 small,
.h3 small,
.h4 small,
.h5 small,
.h6 small,
h1 .small,
h2 .small,
h3 .small,
h4 .small,
h5 .small,
h6 .small,
.h1 .small,
.h2 .small,
.h3 .small,
.h4 .small,
.h5 .small,
.h6 .small {
  font-weight: normal;
  line-height: 1;
  color: #777777;
}
h1,
.h1,
h2,
.h2,
h3,
.h3 {
  margin-top: 18px;
  margin-bottom: 9px;
}
h1 small,
.h1 small,
h2 small,
.h2 small,
h3 small,
.h3 small,
h1 .small,
.h1 .small,
h2 .small,
.h2 .small,
h3 .small,
.h3 .small {
  font-size: 65%;
}
h4,
.h4,
h5,
.h5,
h6,
.h6 {
  margin-top: 9px;
  margin-bottom: 9px;
}
h4 small,
.h4 small,
h5 small,
.h5 small,
h6 small,
.h6 small,
h4 .small,
.h4 .small,
h5 .small,
.h5 .small,
h6 .small,
.h6 .small {
  font-size: 75%;
}
h1,
.h1 {
  font-size: 33px;
}
h2,
.h2 {
  font-size: 27px;
}
h3,
.h3 {
  font-size: 23px;
}
h4,
.h4 {
  font-size: 17px;
}
h5,
.h5 {
  font-size: 13px;
}
h6,
.h6 {
  font-size: 12px;
}
p {
  margin: 0 0 9px;
}
.lead {
  margin-bottom: 18px;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.4;
}
@media (min-width: 768px) {
  .lead {
    font-size: 19.5px;
  }
}
small,
.small {
  font-size: 92%;
}
mark,
.mark {
  background-color: #fcf8e3;
  padding: .2em;
}
.text-left {
  text-align: left;
}
.text-right {
  text-align: right;
}
.text-center {
  text-align: center;
}
.text-justify {
  text-align: justify;
}
.text-nowrap {
  white-space: nowrap;
}
.text-lowercase {
  text-transform: lowercase;
}
.text-uppercase {
  text-transform: uppercase;
}
.text-capitalize {
  text-transform: capitalize;
}
.text-muted {
  color: #777777;
}
.text-primary {
  color: #337ab7;
}
a.text-primary:hover,
a.text-primary:focus {
  color: #286090;
}
.text-success {
  color: #3c763d;
}
a.text-success:hover,
a.text-success:focus {
  color: #2b542c;
}
.text-info {
  color: #31708f;
}
a.text-info:hover,
a.text-info:focus {
  color: #245269;
}
.text-warning {
  color: #8a6d3b;
}
a.text-warning:hover,
a.text-warning:focus {
  color: #66512c;
}
.text-danger {
  color: #a94442;
}
a.text-danger:hover,
a.text-danger:focus {
  color: #843534;
}
.bg-primary {
  color: #fff;
  background-color: #337ab7;
}
a.bg-primary:hover,
a.bg-primary:focus {
  background-color: #286090;
}
.bg-success {
  background-color: #dff0d8;
}
a.bg-success:hover,
a.bg-success:focus {
  background-color: #c1e2b3;
}
.bg-info {
  background-color: #d9edf7;
}
a.bg-info:hover,
a.bg-info:focus {
  background-color: #afd9ee;
}
.bg-warning {
  background-color: #fcf8e3;
}
a.bg-warning:hover,
a.bg-warning:focus {
  background-color: #f7ecb5;
}
.bg-danger {
  background-color: #f2dede;
}
a.bg-danger:hover,
a.bg-danger:focus {
  background-color: #e4b9b9;
}
.page-header {
  padding-bottom: 8px;
  margin: 36px 0 18px;
  border-bottom: 1px solid #eeeeee;
}
ul,
ol {
  margin-top: 0;
  margin-bottom: 9px;
}
ul ul,
ol ul,
ul ol,
ol ol {
  margin-bottom: 0;
}
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
.list-inline {
  padding-left: 0;
  list-style: none;
  margin-left: -5px;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
dl {
  margin-top: 0;
  margin-bottom: 18px;
}
dt,
dd {
  line-height: 1.42857143;
}
dt {
  font-weight: bold;
}
dd {
  margin-left: 0;
}
@media (min-width: 541px) {
  .dl-horizontal dt {
    float: left;
    width: 160px;
    clear: left;
    text-align: right;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .dl-horizontal dd {
    margin-left: 180px;
  }
}
abbr[title],
abbr[data-original-title] {
  cursor: help;
  border-bottom: 1px dotted #777777;
}
.initialism {
  font-size: 90%;
  text-transform: uppercase;
}
blockquote {
  padding: 9px 18px;
  margin: 0 0 18px;
  font-size: inherit;
  border-left: 5px solid #eeeeee;
}
blockquote p:last-child,
blockquote ul:last-child,
blockquote ol:last-child {
  margin-bottom: 0;
}
blockquote footer,
blockquote small,
blockquote .small {
  display: block;
  font-size: 80%;
  line-height: 1.42857143;
  color: #777777;
}
blockquote footer:before,
blockquote small:before,
blockquote .small:before {
  content: '\2014 \00A0';
}
.blockquote-reverse,
blockquote.pull-right {
  padding-right: 15px;
  padding-left: 0;
  border-right: 5px solid #eeeeee;
  border-left: 0;
  text-align: right;
}
.blockquote-reverse footer:before,
blockquote.pull-right footer:before,
.blockquote-reverse small:before,
blockquote.pull-right small:before,
.blockquote-reverse .small:before,
blockquote.pull-right .small:before {
  content: '';
}
.blockquote-reverse footer:after,
blockquote.pull-right footer:after,
.blockquote-reverse small:after,
blockquote.pull-right small:after,
.blockquote-reverse .small:after,
blockquote.pull-right .small:after {
  content: '\00A0 \2014';
}
address {
  margin-bottom: 18px;
  font-style: normal;
  line-height: 1.42857143;
}
code,
kbd,
pre,
samp {
  font-family: monospace;
}
code {
  padding: 2px 4px;
  font-size: 90%;
  color: #c7254e;
  background-color: #f9f2f4;
  border-radius: 2px;
}
kbd {
  padding: 2px 4px;
  font-size: 90%;
  color: #888;
  background-color: transparent;
  border-radius: 1px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
}
kbd kbd {
  padding: 0;
  font-size: 100%;
  font-weight: bold;
  box-shadow: none;
}
pre {
  display: block;
  padding: 8.5px;
  margin: 0 0 9px;
  font-size: 12px;
  line-height: 1.42857143;
  word-break: break-all;
  word-wrap: break-word;
  color: #333333;
  background-color: #f5f5f5;
  border: 1px solid #ccc;
  border-radius: 2px;
}
pre code {
  padding: 0;
  font-size: inherit;
  color: inherit;
  white-space: pre-wrap;
  background-color: transparent;
  border-radius: 0;
}
.pre-scrollable {
  max-height: 340px;
  overflow-y: scroll;
}
.container {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
@media (min-width: 768px) {
  .container {
    width: 768px;
  }
}
@media (min-width: 992px) {
  .container {
    width: 940px;
  }
}
@media (min-width: 1200px) {
  .container {
    width: 1140px;
  }
}
.container-fluid {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
.row {
  margin-left: 0px;
  margin-right: 0px;
}
.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
  position: relative;
  min-height: 1px;
  padding-left: 0px;
  padding-right: 0px;
}
.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 {
  float: left;
}
.col-xs-12 {
  width: 100%;
}
.col-xs-11 {
  width: 91.66666667%;
}
.col-xs-10 {
  width: 83.33333333%;
}
.col-xs-9 {
  width: 75%;
}
.col-xs-8 {
  width: 66.66666667%;
}
.col-xs-7 {
  width: 58.33333333%;
}
.col-xs-6 {
  width: 50%;
}
.col-xs-5 {
  width: 41.66666667%;
}
.col-xs-4 {
  width: 33.33333333%;
}
.col-xs-3 {
  width: 25%;
}
.col-xs-2 {
  width: 16.66666667%;
}
.col-xs-1 {
  width: 8.33333333%;
}
.col-xs-pull-12 {
  right: 100%;
}
.col-xs-pull-11 {
  right: 91.66666667%;
}
.col-xs-pull-10 {
  right: 83.33333333%;
}
.col-xs-pull-9 {
  right: 75%;
}
.col-xs-pull-8 {
  right: 66.66666667%;
}
.col-xs-pull-7 {
  right: 58.33333333%;
}
.col-xs-pull-6 {
  right: 50%;
}
.col-xs-pull-5 {
  right: 41.66666667%;
}
.col-xs-pull-4 {
  right: 33.33333333%;
}
.col-xs-pull-3 {
  right: 25%;
}
.col-xs-pull-2 {
  right: 16.66666667%;
}
.col-xs-pull-1 {
  right: 8.33333333%;
}
.col-xs-pull-0 {
  right: auto;
}
.col-xs-push-12 {
  left: 100%;
}
.col-xs-push-11 {
  left: 91.66666667%;
}
.col-xs-push-10 {
  left: 83.33333333%;
}
.col-xs-push-9 {
  left: 75%;
}
.col-xs-push-8 {
  left: 66.66666667%;
}
.col-xs-push-7 {
  left: 58.33333333%;
}
.col-xs-push-6 {
  left: 50%;
}
.col-xs-push-5 {
  left: 41.66666667%;
}
.col-xs-push-4 {
  left: 33.33333333%;
}
.col-xs-push-3 {
  left: 25%;
}
.col-xs-push-2 {
  left: 16.66666667%;
}
.col-xs-push-1 {
  left: 8.33333333%;
}
.col-xs-push-0 {
  left: auto;
}
.col-xs-offset-12 {
  margin-left: 100%;
}
.col-xs-offset-11 {
  margin-left: 91.66666667%;
}
.col-xs-offset-10 {
  margin-left: 83.33333333%;
}
.col-xs-offset-9 {
  margin-left: 75%;
}
.col-xs-offset-8 {
  margin-left: 66.66666667%;
}
.col-xs-offset-7 {
  margin-left: 58.33333333%;
}
.col-xs-offset-6 {
  margin-left: 50%;
}
.col-xs-offset-5 {
  margin-left: 41.66666667%;
}
.col-xs-offset-4 {
  margin-left: 33.33333333%;
}
.col-xs-offset-3 {
  margin-left: 25%;
}
.col-xs-offset-2 {
  margin-left: 16.66666667%;
}
.col-xs-offset-1 {
  margin-left: 8.33333333%;
}
.col-xs-offset-0 {
  margin-left: 0%;
}
@media (min-width: 768px) {
  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 {
    float: left;
  }
  .col-sm-12 {
    width: 100%;
  }
  .col-sm-11 {
    width: 91.66666667%;
  }
  .col-sm-10 {
    width: 83.33333333%;
  }
  .col-sm-9 {
    width: 75%;
  }
  .col-sm-8 {
    width: 66.66666667%;
  }
  .col-sm-7 {
    width: 58.33333333%;
  }
  .col-sm-6 {
    width: 50%;
  }
  .col-sm-5 {
    width: 41.66666667%;
  }
  .col-sm-4 {
    width: 33.33333333%;
  }
  .col-sm-3 {
    width: 25%;
  }
  .col-sm-2 {
    width: 16.66666667%;
  }
  .col-sm-1 {
    width: 8.33333333%;
  }
  .col-sm-pull-12 {
    right: 100%;
  }
  .col-sm-pull-11 {
    right: 91.66666667%;
  }
  .col-sm-pull-10 {
    right: 83.33333333%;
  }
  .col-sm-pull-9 {
    right: 75%;
  }
  .col-sm-pull-8 {
    right: 66.66666667%;
  }
  .col-sm-pull-7 {
    right: 58.33333333%;
  }
  .col-sm-pull-6 {
    right: 50%;
  }
  .col-sm-pull-5 {
    right: 41.66666667%;
  }
  .col-sm-pull-4 {
    right: 33.33333333%;
  }
  .col-sm-pull-3 {
    right: 25%;
  }
  .col-sm-pull-2 {
    right: 16.66666667%;
  }
  .col-sm-pull-1 {
    right: 8.33333333%;
  }
  .col-sm-pull-0 {
    right: auto;
  }
  .col-sm-push-12 {
    left: 100%;
  }
  .col-sm-push-11 {
    left: 91.66666667%;
  }
  .col-sm-push-10 {
    left: 83.33333333%;
  }
  .col-sm-push-9 {
    left: 75%;
  }
  .col-sm-push-8 {
    left: 66.66666667%;
  }
  .col-sm-push-7 {
    left: 58.33333333%;
  }
  .col-sm-push-6 {
    left: 50%;
  }
  .col-sm-push-5 {
    left: 41.66666667%;
  }
  .col-sm-push-4 {
    left: 33.33333333%;
  }
  .col-sm-push-3 {
    left: 25%;
  }
  .col-sm-push-2 {
    left: 16.66666667%;
  }
  .col-sm-push-1 {
    left: 8.33333333%;
  }
  .col-sm-push-0 {
    left: auto;
  }
  .col-sm-offset-12 {
    margin-left: 100%;
  }
  .col-sm-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-sm-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-sm-offset-9 {
    margin-left: 75%;
  }
  .col-sm-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-sm-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-sm-offset-6 {
    margin-left: 50%;
  }
  .col-sm-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-sm-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-sm-offset-3 {
    margin-left: 25%;
  }
  .col-sm-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-sm-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-sm-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 992px) {
  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
    float: left;
  }
  .col-md-12 {
    width: 100%;
  }
  .col-md-11 {
    width: 91.66666667%;
  }
  .col-md-10 {
    width: 83.33333333%;
  }
  .col-md-9 {
    width: 75%;
  }
  .col-md-8 {
    width: 66.66666667%;
  }
  .col-md-7 {
    width: 58.33333333%;
  }
  .col-md-6 {
    width: 50%;
  }
  .col-md-5 {
    width: 41.66666667%;
  }
  .col-md-4 {
    width: 33.33333333%;
  }
  .col-md-3 {
    width: 25%;
  }
  .col-md-2 {
    width: 16.66666667%;
  }
  .col-md-1 {
    width: 8.33333333%;
  }
  .col-md-pull-12 {
    right: 100%;
  }
  .col-md-pull-11 {
    right: 91.66666667%;
  }
  .col-md-pull-10 {
    right: 83.33333333%;
  }
  .col-md-pull-9 {
    right: 75%;
  }
  .col-md-pull-8 {
    right: 66.66666667%;
  }
  .col-md-pull-7 {
    right: 58.33333333%;
  }
  .col-md-pull-6 {
    right: 50%;
  }
  .col-md-pull-5 {
    right: 41.66666667%;
  }
  .col-md-pull-4 {
    right: 33.33333333%;
  }
  .col-md-pull-3 {
    right: 25%;
  }
  .col-md-pull-2 {
    right: 16.66666667%;
  }
  .col-md-pull-1 {
    right: 8.33333333%;
  }
  .col-md-pull-0 {
    right: auto;
  }
  .col-md-push-12 {
    left: 100%;
  }
  .col-md-push-11 {
    left: 91.66666667%;
  }
  .col-md-push-10 {
    left: 83.33333333%;
  }
  .col-md-push-9 {
    left: 75%;
  }
  .col-md-push-8 {
    left: 66.66666667%;
  }
  .col-md-push-7 {
    left: 58.33333333%;
  }
  .col-md-push-6 {
    left: 50%;
  }
  .col-md-push-5 {
    left: 41.66666667%;
  }
  .col-md-push-4 {
    left: 33.33333333%;
  }
  .col-md-push-3 {
    left: 25%;
  }
  .col-md-push-2 {
    left: 16.66666667%;
  }
  .col-md-push-1 {
    left: 8.33333333%;
  }
  .col-md-push-0 {
    left: auto;
  }
  .col-md-offset-12 {
    margin-left: 100%;
  }
  .col-md-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-md-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-md-offset-9 {
    margin-left: 75%;
  }
  .col-md-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-md-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-md-offset-6 {
    margin-left: 50%;
  }
  .col-md-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-md-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-md-offset-3 {
    margin-left: 25%;
  }
  .col-md-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-md-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-md-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 1200px) {
  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
    float: left;
  }
  .col-lg-12 {
    width: 100%;
  }
  .col-lg-11 {
    width: 91.66666667%;
  }
  .col-lg-10 {
    width: 83.33333333%;
  }
  .col-lg-9 {
    width: 75%;
  }
  .col-lg-8 {
    width: 66.66666667%;
  }
  .col-lg-7 {
    width: 58.33333333%;
  }
  .col-lg-6 {
    width: 50%;
  }
  .col-lg-5 {
    width: 41.66666667%;
  }
  .col-lg-4 {
    width: 33.33333333%;
  }
  .col-lg-3 {
    width: 25%;
  }
  .col-lg-2 {
    width: 16.66666667%;
  }
  .col-lg-1 {
    width: 8.33333333%;
  }
  .col-lg-pull-12 {
    right: 100%;
  }
  .col-lg-pull-11 {
    right: 91.66666667%;
  }
  .col-lg-pull-10 {
    right: 83.33333333%;
  }
  .col-lg-pull-9 {
    right: 75%;
  }
  .col-lg-pull-8 {
    right: 66.66666667%;
  }
  .col-lg-pull-7 {
    right: 58.33333333%;
  }
  .col-lg-pull-6 {
    right: 50%;
  }
  .col-lg-pull-5 {
    right: 41.66666667%;
  }
  .col-lg-pull-4 {
    right: 33.33333333%;
  }
  .col-lg-pull-3 {
    right: 25%;
  }
  .col-lg-pull-2 {
    right: 16.66666667%;
  }
  .col-lg-pull-1 {
    right: 8.33333333%;
  }
  .col-lg-pull-0 {
    right: auto;
  }
  .col-lg-push-12 {
    left: 100%;
  }
  .col-lg-push-11 {
    left: 91.66666667%;
  }
  .col-lg-push-10 {
    left: 83.33333333%;
  }
  .col-lg-push-9 {
    left: 75%;
  }
  .col-lg-push-8 {
    left: 66.66666667%;
  }
  .col-lg-push-7 {
    left: 58.33333333%;
  }
  .col-lg-push-6 {
    left: 50%;
  }
  .col-lg-push-5 {
    left: 41.66666667%;
  }
  .col-lg-push-4 {
    left: 33.33333333%;
  }
  .col-lg-push-3 {
    left: 25%;
  }
  .col-lg-push-2 {
    left: 16.66666667%;
  }
  .col-lg-push-1 {
    left: 8.33333333%;
  }
  .col-lg-push-0 {
    left: auto;
  }
  .col-lg-offset-12 {
    margin-left: 100%;
  }
  .col-lg-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-lg-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-lg-offset-9 {
    margin-left: 75%;
  }
  .col-lg-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-lg-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-lg-offset-6 {
    margin-left: 50%;
  }
  .col-lg-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-lg-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-lg-offset-3 {
    margin-left: 25%;
  }
  .col-lg-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-lg-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-lg-offset-0 {
    margin-left: 0%;
  }
}
table {
  background-color: transparent;
}
caption {
  padding-top: 8px;
  padding-bottom: 8px;
  color: #777777;
  text-align: left;
}
th {
  text-align: left;
}
.table {
  width: 100%;
  max-width: 100%;
  margin-bottom: 18px;
}
.table > thead > tr > th,
.table > tbody > tr > th,
.table > tfoot > tr > th,
.table > thead > tr > td,
.table > tbody > tr > td,
.table > tfoot > tr > td {
  padding: 8px;
  line-height: 1.42857143;
  vertical-align: top;
  border-top: 1px solid #ddd;
}
.table > thead > tr > th {
  vertical-align: bottom;
  border-bottom: 2px solid #ddd;
}
.table > caption + thead > tr:first-child > th,
.table > colgroup + thead > tr:first-child > th,
.table > thead:first-child > tr:first-child > th,
.table > caption + thead > tr:first-child > td,
.table > colgroup + thead > tr:first-child > td,
.table > thead:first-child > tr:first-child > td {
  border-top: 0;
}
.table > tbody + tbody {
  border-top: 2px solid #ddd;
}
.table .table {
  background-color: #fff;
}
.table-condensed > thead > tr > th,
.table-condensed > tbody > tr > th,
.table-condensed > tfoot > tr > th,
.table-condensed > thead > tr > td,
.table-condensed > tbody > tr > td,
.table-condensed > tfoot > tr > td {
  padding: 5px;
}
.table-bordered {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > tbody > tr > th,
.table-bordered > tfoot > tr > th,
.table-bordered > thead > tr > td,
.table-bordered > tbody > tr > td,
.table-bordered > tfoot > tr > td {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > thead > tr > td {
  border-bottom-width: 2px;
}
.table-striped > tbody > tr:nth-of-type(odd) {
  background-color: #f9f9f9;
}
.table-hover > tbody > tr:hover {
  background-color: #f5f5f5;
}
table col[class*="col-"] {
  position: static;
  float: none;
  display: table-column;
}
table td[class*="col-"],
table th[class*="col-"] {
  position: static;
  float: none;
  display: table-cell;
}
.table > thead > tr > td.active,
.table > tbody > tr > td.active,
.table > tfoot > tr > td.active,
.table > thead > tr > th.active,
.table > tbody > tr > th.active,
.table > tfoot > tr > th.active,
.table > thead > tr.active > td,
.table > tbody > tr.active > td,
.table > tfoot > tr.active > td,
.table > thead > tr.active > th,
.table > tbody > tr.active > th,
.table > tfoot > tr.active > th {
  background-color: #f5f5f5;
}
.table-hover > tbody > tr > td.active:hover,
.table-hover > tbody > tr > th.active:hover,
.table-hover > tbody > tr.active:hover > td,
.table-hover > tbody > tr:hover > .active,
.table-hover > tbody > tr.active:hover > th {
  background-color: #e8e8e8;
}
.table > thead > tr > td.success,
.table > tbody > tr > td.success,
.table > tfoot > tr > td.success,
.table > thead > tr > th.success,
.table > tbody > tr > th.success,
.table > tfoot > tr > th.success,
.table > thead > tr.success > td,
.table > tbody > tr.success > td,
.table > tfoot > tr.success > td,
.table > thead > tr.success > th,
.table > tbody > tr.success > th,
.table > tfoot > tr.success > th {
  background-color: #dff0d8;
}
.table-hover > tbody > tr > td.success:hover,
.table-hover > tbody > tr > th.success:hover,
.table-hover > tbody > tr.success:hover > td,
.table-hover > tbody > tr:hover > .success,
.table-hover > tbody > tr.success:hover > th {
  background-color: #d0e9c6;
}
.table > thead > tr > td.info,
.table > tbody > tr > td.info,
.table > tfoot > tr > td.info,
.table > thead > tr > th.info,
.table > tbody > tr > th.info,
.table > tfoot > tr > th.info,
.table > thead > tr.info > td,
.table > tbody > tr.info > td,
.table > tfoot > tr.info > td,
.table > thead > tr.info > th,
.table > tbody > tr.info > th,
.table > tfoot > tr.info > th {
  background-color: #d9edf7;
}
.table-hover > tbody > tr > td.info:hover,
.table-hover > tbody > tr > th.info:hover,
.table-hover > tbody > tr.info:hover > td,
.table-hover > tbody > tr:hover > .info,
.table-hover > tbody > tr.info:hover > th {
  background-color: #c4e3f3;
}
.table > thead > tr > td.warning,
.table > tbody > tr > td.warning,
.table > tfoot > tr > td.warning,
.table > thead > tr > th.warning,
.table > tbody > tr > th.warning,
.table > tfoot > tr > th.warning,
.table > thead > tr.warning > td,
.table > tbody > tr.warning > td,
.table > tfoot > tr.warning > td,
.table > thead > tr.warning > th,
.table > tbody > tr.warning > th,
.table > tfoot > tr.warning > th {
  background-color: #fcf8e3;
}
.table-hover > tbody > tr > td.warning:hover,
.table-hover > tbody > tr > th.warning:hover,
.table-hover > tbody > tr.warning:hover > td,
.table-hover > tbody > tr:hover > .warning,
.table-hover > tbody > tr.warning:hover > th {
  background-color: #faf2cc;
}
.table > thead > tr > td.danger,
.table > tbody > tr > td.danger,
.table > tfoot > tr > td.danger,
.table > thead > tr > th.danger,
.table > tbody > tr > th.danger,
.table > tfoot > tr > th.danger,
.table > thead > tr.danger > td,
.table > tbody > tr.danger > td,
.table > tfoot > tr.danger > td,
.table > thead > tr.danger > th,
.table > tbody > tr.danger > th,
.table > tfoot > tr.danger > th {
  background-color: #f2dede;
}
.table-hover > tbody > tr > td.danger:hover,
.table-hover > tbody > tr > th.danger:hover,
.table-hover > tbody > tr.danger:hover > td,
.table-hover > tbody > tr:hover > .danger,
.table-hover > tbody > tr.danger:hover > th {
  background-color: #ebcccc;
}
.table-responsive {
  overflow-x: auto;
  min-height: 0.01%;
}
@media screen and (max-width: 767px) {
  .table-responsive {
    width: 100%;
    margin-bottom: 13.5px;
    overflow-y: hidden;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    border: 1px solid #ddd;
  }
  .table-responsive > .table {
    margin-bottom: 0;
  }
  .table-responsive > .table > thead > tr > th,
  .table-responsive > .table > tbody > tr > th,
  .table-responsive > .table > tfoot > tr > th,
  .table-responsive > .table > thead > tr > td,
  .table-responsive > .table > tbody > tr > td,
  .table-responsive > .table > tfoot > tr > td {
    white-space: nowrap;
  }
  .table-responsive > .table-bordered {
    border: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:first-child,
  .table-responsive > .table-bordered > tbody > tr > th:first-child,
  .table-responsive > .table-bordered > tfoot > tr > th:first-child,
  .table-responsive > .table-bordered > thead > tr > td:first-child,
  .table-responsive > .table-bordered > tbody > tr > td:first-child,
  .table-responsive > .table-bordered > tfoot > tr > td:first-child {
    border-left: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:last-child,
  .table-responsive > .table-bordered > tbody > tr > th:last-child,
  .table-responsive > .table-bordered > tfoot > tr > th:last-child,
  .table-responsive > .table-bordered > thead > tr > td:last-child,
  .table-responsive > .table-bordered > tbody > tr > td:last-child,
  .table-responsive > .table-bordered > tfoot > tr > td:last-child {
    border-right: 0;
  }
  .table-responsive > .table-bordered > tbody > tr:last-child > th,
  .table-responsive > .table-bordered > tfoot > tr:last-child > th,
  .table-responsive > .table-bordered > tbody > tr:last-child > td,
  .table-responsive > .table-bordered > tfoot > tr:last-child > td {
    border-bottom: 0;
  }
}
fieldset {
  padding: 0;
  margin: 0;
  border: 0;
  min-width: 0;
}
legend {
  display: block;
  width: 100%;
  padding: 0;
  margin-bottom: 18px;
  font-size: 19.5px;
  line-height: inherit;
  color: #333333;
  border: 0;
  border-bottom: 1px solid #e5e5e5;
}
label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: bold;
}
input[type="search"] {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
input[type="radio"],
input[type="checkbox"] {
  margin: 4px 0 0;
  margin-top: 1px \9;
  line-height: normal;
}
input[type="file"] {
  display: block;
}
input[type="range"] {
  display: block;
  width: 100%;
}
select[multiple],
select[size] {
  height: auto;
}
input[type="file"]:focus,
input[type="radio"]:focus,
input[type="checkbox"]:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
output {
  display: block;
  padding-top: 7px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
}
.form-control {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
}
.form-control:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.form-control::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.form-control:-ms-input-placeholder {
  color: #999;
}
.form-control::-webkit-input-placeholder {
  color: #999;
}
.form-control::-ms-expand {
  border: 0;
  background-color: transparent;
}
.form-control[disabled],
.form-control[readonly],
fieldset[disabled] .form-control {
  background-color: #eeeeee;
  opacity: 1;
}
.form-control[disabled],
fieldset[disabled] .form-control {
  cursor: not-allowed;
}
textarea.form-control {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: none;
}
@media screen and (-webkit-min-device-pixel-ratio: 0) {
  input[type="date"].form-control,
  input[type="time"].form-control,
  input[type="datetime-local"].form-control,
  input[type="month"].form-control {
    line-height: 32px;
  }
  input[type="date"].input-sm,
  input[type="time"].input-sm,
  input[type="datetime-local"].input-sm,
  input[type="month"].input-sm,
  .input-group-sm input[type="date"],
  .input-group-sm input[type="time"],
  .input-group-sm input[type="datetime-local"],
  .input-group-sm input[type="month"] {
    line-height: 30px;
  }
  input[type="date"].input-lg,
  input[type="time"].input-lg,
  input[type="datetime-local"].input-lg,
  input[type="month"].input-lg,
  .input-group-lg input[type="date"],
  .input-group-lg input[type="time"],
  .input-group-lg input[type="datetime-local"],
  .input-group-lg input[type="month"] {
    line-height: 45px;
  }
}
.form-group {
  margin-bottom: 15px;
}
.radio,
.checkbox {
  position: relative;
  display: block;
  margin-top: 10px;
  margin-bottom: 10px;
}
.radio label,
.checkbox label {
  min-height: 18px;
  padding-left: 20px;
  margin-bottom: 0;
  font-weight: normal;
  cursor: pointer;
}
.radio input[type="radio"],
.radio-inline input[type="radio"],
.checkbox input[type="checkbox"],
.checkbox-inline input[type="checkbox"] {
  position: absolute;
  margin-left: -20px;
  margin-top: 4px \9;
}
.radio + .radio,
.checkbox + .checkbox {
  margin-top: -5px;
}
.radio-inline,
.checkbox-inline {
  position: relative;
  display: inline-block;
  padding-left: 20px;
  margin-bottom: 0;
  vertical-align: middle;
  font-weight: normal;
  cursor: pointer;
}
.radio-inline + .radio-inline,
.checkbox-inline + .checkbox-inline {
  margin-top: 0;
  margin-left: 10px;
}
input[type="radio"][disabled],
input[type="checkbox"][disabled],
input[type="radio"].disabled,
input[type="checkbox"].disabled,
fieldset[disabled] input[type="radio"],
fieldset[disabled] input[type="checkbox"] {
  cursor: not-allowed;
}
.radio-inline.disabled,
.checkbox-inline.disabled,
fieldset[disabled] .radio-inline,
fieldset[disabled] .checkbox-inline {
  cursor: not-allowed;
}
.radio.disabled label,
.checkbox.disabled label,
fieldset[disabled] .radio label,
fieldset[disabled] .checkbox label {
  cursor: not-allowed;
}
.form-control-static {
  padding-top: 7px;
  padding-bottom: 7px;
  margin-bottom: 0;
  min-height: 31px;
}
.form-control-static.input-lg,
.form-control-static.input-sm {
  padding-left: 0;
  padding-right: 0;
}
.input-sm {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-sm {
  height: 30px;
  line-height: 30px;
}
textarea.input-sm,
select[multiple].input-sm {
  height: auto;
}
.form-group-sm .form-control {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.form-group-sm select.form-control {
  height: 30px;
  line-height: 30px;
}
.form-group-sm textarea.form-control,
.form-group-sm select[multiple].form-control {
  height: auto;
}
.form-group-sm .form-control-static {
  height: 30px;
  min-height: 30px;
  padding: 6px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.input-lg {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-lg {
  height: 45px;
  line-height: 45px;
}
textarea.input-lg,
select[multiple].input-lg {
  height: auto;
}
.form-group-lg .form-control {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.form-group-lg select.form-control {
  height: 45px;
  line-height: 45px;
}
.form-group-lg textarea.form-control,
.form-group-lg select[multiple].form-control {
  height: auto;
}
.form-group-lg .form-control-static {
  height: 45px;
  min-height: 35px;
  padding: 11px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.has-feedback {
  position: relative;
}
.has-feedback .form-control {
  padding-right: 40px;
}
.form-control-feedback {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 2;
  display: block;
  width: 32px;
  height: 32px;
  line-height: 32px;
  text-align: center;
  pointer-events: none;
}
.input-lg + .form-control-feedback,
.input-group-lg + .form-control-feedback,
.form-group-lg .form-control + .form-control-feedback {
  width: 45px;
  height: 45px;
  line-height: 45px;
}
.input-sm + .form-control-feedback,
.input-group-sm + .form-control-feedback,
.form-group-sm .form-control + .form-control-feedback {
  width: 30px;
  height: 30px;
  line-height: 30px;
}
.has-success .help-block,
.has-success .control-label,
.has-success .radio,
.has-success .checkbox,
.has-success .radio-inline,
.has-success .checkbox-inline,
.has-success.radio label,
.has-success.checkbox label,
.has-success.radio-inline label,
.has-success.checkbox-inline label {
  color: #3c763d;
}
.has-success .form-control {
  border-color: #3c763d;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-success .form-control:focus {
  border-color: #2b542c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
}
.has-success .input-group-addon {
  color: #3c763d;
  border-color: #3c763d;
  background-color: #dff0d8;
}
.has-success .form-control-feedback {
  color: #3c763d;
}
.has-warning .help-block,
.has-warning .control-label,
.has-warning .radio,
.has-warning .checkbox,
.has-warning .radio-inline,
.has-warning .checkbox-inline,
.has-warning.radio label,
.has-warning.checkbox label,
.has-warning.radio-inline label,
.has-warning.checkbox-inline label {
  color: #8a6d3b;
}
.has-warning .form-control {
  border-color: #8a6d3b;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-warning .form-control:focus {
  border-color: #66512c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
}
.has-warning .input-group-addon {
  color: #8a6d3b;
  border-color: #8a6d3b;
  background-color: #fcf8e3;
}
.has-warning .form-control-feedback {
  color: #8a6d3b;
}
.has-error .help-block,
.has-error .control-label,
.has-error .radio,
.has-error .checkbox,
.has-error .radio-inline,
.has-error .checkbox-inline,
.has-error.radio label,
.has-error.checkbox label,
.has-error.radio-inline label,
.has-error.checkbox-inline label {
  color: #a94442;
}
.has-error .form-control {
  border-color: #a94442;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-error .form-control:focus {
  border-color: #843534;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
}
.has-error .input-group-addon {
  color: #a94442;
  border-color: #a94442;
  background-color: #f2dede;
}
.has-error .form-control-feedback {
  color: #a94442;
}
.has-feedback label ~ .form-control-feedback {
  top: 23px;
}
.has-feedback label.sr-only ~ .form-control-feedback {
  top: 0;
}
.help-block {
  display: block;
  margin-top: 5px;
  margin-bottom: 10px;
  color: #404040;
}
@media (min-width: 768px) {
  .form-inline .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .form-inline .form-control-static {
    display: inline-block;
  }
  .form-inline .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .form-inline .input-group .input-group-addon,
  .form-inline .input-group .input-group-btn,
  .form-inline .input-group .form-control {
    width: auto;
  }
  .form-inline .input-group > .form-control {
    width: 100%;
  }
  .form-inline .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio,
  .form-inline .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio label,
  .form-inline .checkbox label {
    padding-left: 0;
  }
  .form-inline .radio input[type="radio"],
  .form-inline .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .form-inline .has-feedback .form-control-feedback {
    top: 0;
  }
}
.form-horizontal .radio,
.form-horizontal .checkbox,
.form-horizontal .radio-inline,
.form-horizontal .checkbox-inline {
  margin-top: 0;
  margin-bottom: 0;
  padding-top: 7px;
}
.form-horizontal .radio,
.form-horizontal .checkbox {
  min-height: 25px;
}
.form-horizontal .form-group {
  margin-left: 0px;
  margin-right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .control-label {
    text-align: right;
    margin-bottom: 0;
    padding-top: 7px;
  }
}
.form-horizontal .has-feedback .form-control-feedback {
  right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .form-group-lg .control-label {
    padding-top: 11px;
    font-size: 17px;
  }
}
@media (min-width: 768px) {
  .form-horizontal .form-group-sm .control-label {
    padding-top: 6px;
    font-size: 12px;
  }
}
.btn {
  display: inline-block;
  margin-bottom: 0;
  font-weight: normal;
  text-align: center;
  vertical-align: middle;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  white-space: nowrap;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  border-radius: 2px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.btn:focus,
.btn:active:focus,
.btn.active:focus,
.btn.focus,
.btn:active.focus,
.btn.active.focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.btn:hover,
.btn:focus,
.btn.focus {
  color: #333;
  text-decoration: none;
}
.btn:active,
.btn.active {
  outline: 0;
  background-image: none;
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn.disabled,
.btn[disabled],
fieldset[disabled] .btn {
  cursor: not-allowed;
  opacity: 0.65;
  filter: alpha(opacity=65);
  -webkit-box-shadow: none;
  box-shadow: none;
}
a.btn.disabled,
fieldset[disabled] a.btn {
  pointer-events: none;
}
.btn-default {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.btn-default:focus,
.btn-default.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.btn-default:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active:hover,
.btn-default.active:hover,
.open > .dropdown-toggle.btn-default:hover,
.btn-default:active:focus,
.btn-default.active:focus,
.open > .dropdown-toggle.btn-default:focus,
.btn-default:active.focus,
.btn-default.active.focus,
.open > .dropdown-toggle.btn-default.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  background-image: none;
}
.btn-default.disabled:hover,
.btn-default[disabled]:hover,
fieldset[disabled] .btn-default:hover,
.btn-default.disabled:focus,
.btn-default[disabled]:focus,
fieldset[disabled] .btn-default:focus,
.btn-default.disabled.focus,
.btn-default[disabled].focus,
fieldset[disabled] .btn-default.focus {
  background-color: #fff;
  border-color: #ccc;
}
.btn-default .badge {
  color: #fff;
  background-color: #333;
}
.btn-primary {
  color: #fff;
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary:focus,
.btn-primary.focus {
  color: #fff;
  background-color: #286090;
  border-color: #122b40;
}
.btn-primary:hover {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active:hover,
.btn-primary.active:hover,
.open > .dropdown-toggle.btn-primary:hover,
.btn-primary:active:focus,
.btn-primary.active:focus,
.open > .dropdown-toggle.btn-primary:focus,
.btn-primary:active.focus,
.btn-primary.active.focus,
.open > .dropdown-toggle.btn-primary.focus {
  color: #fff;
  background-color: #204d74;
  border-color: #122b40;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  background-image: none;
}
.btn-primary.disabled:hover,
.btn-primary[disabled]:hover,
fieldset[disabled] .btn-primary:hover,
.btn-primary.disabled:focus,
.btn-primary[disabled]:focus,
fieldset[disabled] .btn-primary:focus,
.btn-primary.disabled.focus,
.btn-primary[disabled].focus,
fieldset[disabled] .btn-primary.focus {
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary .badge {
  color: #337ab7;
  background-color: #fff;
}
.btn-success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success:focus,
.btn-success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.btn-success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active:hover,
.btn-success.active:hover,
.open > .dropdown-toggle.btn-success:hover,
.btn-success:active:focus,
.btn-success.active:focus,
.open > .dropdown-toggle.btn-success:focus,
.btn-success:active.focus,
.btn-success.active.focus,
.open > .dropdown-toggle.btn-success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  background-image: none;
}
.btn-success.disabled:hover,
.btn-success[disabled]:hover,
fieldset[disabled] .btn-success:hover,
.btn-success.disabled:focus,
.btn-success[disabled]:focus,
fieldset[disabled] .btn-success:focus,
.btn-success.disabled.focus,
.btn-success[disabled].focus,
fieldset[disabled] .btn-success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.btn-info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info:focus,
.btn-info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.btn-info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active:hover,
.btn-info.active:hover,
.open > .dropdown-toggle.btn-info:hover,
.btn-info:active:focus,
.btn-info.active:focus,
.open > .dropdown-toggle.btn-info:focus,
.btn-info:active.focus,
.btn-info.active.focus,
.open > .dropdown-toggle.btn-info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  background-image: none;
}
.btn-info.disabled:hover,
.btn-info[disabled]:hover,
fieldset[disabled] .btn-info:hover,
.btn-info.disabled:focus,
.btn-info[disabled]:focus,
fieldset[disabled] .btn-info:focus,
.btn-info.disabled.focus,
.btn-info[disabled].focus,
fieldset[disabled] .btn-info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.btn-warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning:focus,
.btn-warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.btn-warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active:hover,
.btn-warning.active:hover,
.open > .dropdown-toggle.btn-warning:hover,
.btn-warning:active:focus,
.btn-warning.active:focus,
.open > .dropdown-toggle.btn-warning:focus,
.btn-warning:active.focus,
.btn-warning.active.focus,
.open > .dropdown-toggle.btn-warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  background-image: none;
}
.btn-warning.disabled:hover,
.btn-warning[disabled]:hover,
fieldset[disabled] .btn-warning:hover,
.btn-warning.disabled:focus,
.btn-warning[disabled]:focus,
fieldset[disabled] .btn-warning:focus,
.btn-warning.disabled.focus,
.btn-warning[disabled].focus,
fieldset[disabled] .btn-warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.btn-danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger:focus,
.btn-danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.btn-danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active:hover,
.btn-danger.active:hover,
.open > .dropdown-toggle.btn-danger:hover,
.btn-danger:active:focus,
.btn-danger.active:focus,
.open > .dropdown-toggle.btn-danger:focus,
.btn-danger:active.focus,
.btn-danger.active.focus,
.open > .dropdown-toggle.btn-danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  background-image: none;
}
.btn-danger.disabled:hover,
.btn-danger[disabled]:hover,
fieldset[disabled] .btn-danger:hover,
.btn-danger.disabled:focus,
.btn-danger[disabled]:focus,
fieldset[disabled] .btn-danger:focus,
.btn-danger.disabled.focus,
.btn-danger[disabled].focus,
fieldset[disabled] .btn-danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger .badge {
  color: #d9534f;
  background-color: #fff;
}
.btn-link {
  color: #337ab7;
  font-weight: normal;
  border-radius: 0;
}
.btn-link,
.btn-link:active,
.btn-link.active,
.btn-link[disabled],
fieldset[disabled] .btn-link {
  background-color: transparent;
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn-link,
.btn-link:hover,
.btn-link:focus,
.btn-link:active {
  border-color: transparent;
}
.btn-link:hover,
.btn-link:focus {
  color: #23527c;
  text-decoration: underline;
  background-color: transparent;
}
.btn-link[disabled]:hover,
fieldset[disabled] .btn-link:hover,
.btn-link[disabled]:focus,
fieldset[disabled] .btn-link:focus {
  color: #777777;
  text-decoration: none;
}
.btn-lg,
.btn-group-lg > .btn {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.btn-sm,
.btn-group-sm > .btn {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-xs,
.btn-group-xs > .btn {
  padding: 1px 5px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-block {
  display: block;
  width: 100%;
}
.btn-block + .btn-block {
  margin-top: 5px;
}
input[type="submit"].btn-block,
input[type="reset"].btn-block,
input[type="button"].btn-block {
  width: 100%;
}
.fade {
  opacity: 0;
  -webkit-transition: opacity 0.15s linear;
  -o-transition: opacity 0.15s linear;
  transition: opacity 0.15s linear;
}
.fade.in {
  opacity: 1;
}
.collapse {
  display: none;
}
.collapse.in {
  display: block;
}
tr.collapse.in {
  display: table-row;
}
tbody.collapse.in {
  display: table-row-group;
}
.collapsing {
  position: relative;
  height: 0;
  overflow: hidden;
  -webkit-transition-property: height, visibility;
  transition-property: height, visibility;
  -webkit-transition-duration: 0.35s;
  transition-duration: 0.35s;
  -webkit-transition-timing-function: ease;
  transition-timing-function: ease;
}
.caret {
  display: inline-block;
  width: 0;
  height: 0;
  margin-left: 2px;
  vertical-align: middle;
  border-top: 4px dashed;
  border-top: 4px solid \9;
  border-right: 4px solid transparent;
  border-left: 4px solid transparent;
}
.dropup,
.dropdown {
  position: relative;
}
.dropdown-toggle:focus {
  outline: 0;
}
.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 160px;
  padding: 5px 0;
  margin: 2px 0 0;
  list-style: none;
  font-size: 13px;
  text-align: left;
  background-color: #fff;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 2px;
  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  background-clip: padding-box;
}
.dropdown-menu.pull-right {
  right: 0;
  left: auto;
}
.dropdown-menu .divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.dropdown-menu > li > a {
  display: block;
  padding: 3px 20px;
  clear: both;
  font-weight: normal;
  line-height: 1.42857143;
  color: #333333;
  white-space: nowrap;
}
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
  text-decoration: none;
  color: #262626;
  background-color: #f5f5f5;
}
.dropdown-menu > .active > a,
.dropdown-menu > .active > a:hover,
.dropdown-menu > .active > a:focus {
  color: #fff;
  text-decoration: none;
  outline: 0;
  background-color: #337ab7;
}
.dropdown-menu > .disabled > a,
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  color: #777777;
}
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  text-decoration: none;
  background-color: transparent;
  background-image: none;
  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
  cursor: not-allowed;
}
.open > .dropdown-menu {
  display: block;
}
.open > a {
  outline: 0;
}
.dropdown-menu-right {
  left: auto;
  right: 0;
}
.dropdown-menu-left {
  left: 0;
  right: auto;
}
.dropdown-header {
  display: block;
  padding: 3px 20px;
  font-size: 12px;
  line-height: 1.42857143;
  color: #777777;
  white-space: nowrap;
}
.dropdown-backdrop {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  z-index: 990;
}
.pull-right > .dropdown-menu {
  right: 0;
  left: auto;
}
.dropup .caret,
.navbar-fixed-bottom .dropdown .caret {
  border-top: 0;
  border-bottom: 4px dashed;
  border-bottom: 4px solid \9;
  content: "";
}
.dropup .dropdown-menu,
.navbar-fixed-bottom .dropdown .dropdown-menu {
  top: auto;
  bottom: 100%;
  margin-bottom: 2px;
}
@media (min-width: 541px) {
  .navbar-right .dropdown-menu {
    left: auto;
    right: 0;
  }
  .navbar-right .dropdown-menu-left {
    left: 0;
    right: auto;
  }
}
.btn-group,
.btn-group-vertical {
  position: relative;
  display: inline-block;
  vertical-align: middle;
}
.btn-group > .btn,
.btn-group-vertical > .btn {
  position: relative;
  float: left;
}
.btn-group > .btn:hover,
.btn-group-vertical > .btn:hover,
.btn-group > .btn:focus,
.btn-group-vertical > .btn:focus,
.btn-group > .btn:active,
.btn-group-vertical > .btn:active,
.btn-group > .btn.active,
.btn-group-vertical > .btn.active {
  z-index: 2;
}
.btn-group .btn + .btn,
.btn-group .btn + .btn-group,
.btn-group .btn-group + .btn,
.btn-group .btn-group + .btn-group {
  margin-left: -1px;
}
.btn-toolbar {
  margin-left: -5px;
}
.btn-toolbar .btn,
.btn-toolbar .btn-group,
.btn-toolbar .input-group {
  float: left;
}
.btn-toolbar > .btn,
.btn-toolbar > .btn-group,
.btn-toolbar > .input-group {
  margin-left: 5px;
}
.btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) {
  border-radius: 0;
}
.btn-group > .btn:first-child {
  margin-left: 0;
}
.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn:last-child:not(:first-child),
.btn-group > .dropdown-toggle:not(:first-child) {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group > .btn-group {
  float: left;
}
.btn-group > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group .dropdown-toggle:active,
.btn-group.open .dropdown-toggle {
  outline: 0;
}
.btn-group > .btn + .dropdown-toggle {
  padding-left: 8px;
  padding-right: 8px;
}
.btn-group > .btn-lg + .dropdown-toggle {
  padding-left: 12px;
  padding-right: 12px;
}
.btn-group.open .dropdown-toggle {
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn-group.open .dropdown-toggle.btn-link {
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn .caret {
  margin-left: 0;
}
.btn-lg .caret {
  border-width: 5px 5px 0;
  border-bottom-width: 0;
}
.dropup .btn-lg .caret {
  border-width: 0 5px 5px;
}
.btn-group-vertical > .btn,
.btn-group-vertical > .btn-group,
.btn-group-vertical > .btn-group > .btn {
  display: block;
  float: none;
  width: 100%;
  max-width: 100%;
}
.btn-group-vertical > .btn-group > .btn {
  float: none;
}
.btn-group-vertical > .btn + .btn,
.btn-group-vertical > .btn + .btn-group,
.btn-group-vertical > .btn-group + .btn,
.btn-group-vertical > .btn-group + .btn-group {
  margin-top: -1px;
  margin-left: 0;
}
.btn-group-vertical > .btn:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.btn-group-vertical > .btn:first-child:not(:last-child) {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn:last-child:not(:first-child) {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
.btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.btn-group-justified {
  display: table;
  width: 100%;
  table-layout: fixed;
  border-collapse: separate;
}
.btn-group-justified > .btn,
.btn-group-justified > .btn-group {
  float: none;
  display: table-cell;
  width: 1%;
}
.btn-group-justified > .btn-group .btn {
  width: 100%;
}
.btn-group-justified > .btn-group .dropdown-menu {
  left: auto;
}
[data-toggle="buttons"] > .btn input[type="radio"],
[data-toggle="buttons"] > .btn-group > .btn input[type="radio"],
[data-toggle="buttons"] > .btn input[type="checkbox"],
[data-toggle="buttons"] > .btn-group > .btn input[type="checkbox"] {
  position: absolute;
  clip: rect(0, 0, 0, 0);
  pointer-events: none;
}
.input-group {
  position: relative;
  display: table;
  border-collapse: separate;
}
.input-group[class*="col-"] {
  float: none;
  padding-left: 0;
  padding-right: 0;
}
.input-group .form-control {
  position: relative;
  z-index: 2;
  float: left;
  width: 100%;
  margin-bottom: 0;
}
.input-group .form-control:focus {
  z-index: 3;
}
.input-group-lg > .form-control,
.input-group-lg > .input-group-addon,
.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-group-lg > .form-control,
select.input-group-lg > .input-group-addon,
select.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  line-height: 45px;
}
textarea.input-group-lg > .form-control,
textarea.input-group-lg > .input-group-addon,
textarea.input-group-lg > .input-group-btn > .btn,
select[multiple].input-group-lg > .form-control,
select[multiple].input-group-lg > .input-group-addon,
select[multiple].input-group-lg > .input-group-btn > .btn {
  height: auto;
}
.input-group-sm > .form-control,
.input-group-sm > .input-group-addon,
.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-group-sm > .form-control,
select.input-group-sm > .input-group-addon,
select.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  line-height: 30px;
}
textarea.input-group-sm > .form-control,
textarea.input-group-sm > .input-group-addon,
textarea.input-group-sm > .input-group-btn > .btn,
select[multiple].input-group-sm > .form-control,
select[multiple].input-group-sm > .input-group-addon,
select[multiple].input-group-sm > .input-group-btn > .btn {
  height: auto;
}
.input-group-addon,
.input-group-btn,
.input-group .form-control {
  display: table-cell;
}
.input-group-addon:not(:first-child):not(:last-child),
.input-group-btn:not(:first-child):not(:last-child),
.input-group .form-control:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.input-group-addon,
.input-group-btn {
  width: 1%;
  white-space: nowrap;
  vertical-align: middle;
}
.input-group-addon {
  padding: 6px 12px;
  font-size: 13px;
  font-weight: normal;
  line-height: 1;
  color: #555555;
  text-align: center;
  background-color: #eeeeee;
  border: 1px solid #ccc;
  border-radius: 2px;
}
.input-group-addon.input-sm {
  padding: 5px 10px;
  font-size: 12px;
  border-radius: 1px;
}
.input-group-addon.input-lg {
  padding: 10px 16px;
  font-size: 17px;
  border-radius: 3px;
}
.input-group-addon input[type="radio"],
.input-group-addon input[type="checkbox"] {
  margin-top: 0;
}
.input-group .form-control:first-child,
.input-group-addon:first-child,
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group > .btn,
.input-group-btn:first-child > .dropdown-toggle,
.input-group-btn:last-child > .btn:not(:last-child):not(.dropdown-toggle),
.input-group-btn:last-child > .btn-group:not(:last-child) > .btn {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.input-group-addon:first-child {
  border-right: 0;
}
.input-group .form-control:last-child,
.input-group-addon:last-child,
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group > .btn,
.input-group-btn:last-child > .dropdown-toggle,
.input-group-btn:first-child > .btn:not(:first-child),
.input-group-btn:first-child > .btn-group:not(:first-child) > .btn {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.input-group-addon:last-child {
  border-left: 0;
}
.input-group-btn {
  position: relative;
  font-size: 0;
  white-space: nowrap;
}
.input-group-btn > .btn {
  position: relative;
}
.input-group-btn > .btn + .btn {
  margin-left: -1px;
}
.input-group-btn > .btn:hover,
.input-group-btn > .btn:focus,
.input-group-btn > .btn:active {
  z-index: 2;
}
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group {
  margin-right: -1px;
}
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group {
  z-index: 2;
  margin-left: -1px;
}
.nav {
  margin-bottom: 0;
  padding-left: 0;
  list-style: none;
}
.nav > li {
  position: relative;
  display: block;
}
.nav > li > a {
  position: relative;
  display: block;
  padding: 10px 15px;
}
.nav > li > a:hover,
.nav > li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.nav > li.disabled > a {
  color: #777777;
}
.nav > li.disabled > a:hover,
.nav > li.disabled > a:focus {
  color: #777777;
  text-decoration: none;
  background-color: transparent;
  cursor: not-allowed;
}
.nav .open > a,
.nav .open > a:hover,
.nav .open > a:focus {
  background-color: #eeeeee;
  border-color: #337ab7;
}
.nav .nav-divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.nav > li > a > img {
  max-width: none;
}
.nav-tabs {
  border-bottom: 1px solid #ddd;
}
.nav-tabs > li {
  float: left;
  margin-bottom: -1px;
}
.nav-tabs > li > a {
  margin-right: 2px;
  line-height: 1.42857143;
  border: 1px solid transparent;
  border-radius: 2px 2px 0 0;
}
.nav-tabs > li > a:hover {
  border-color: #eeeeee #eeeeee #ddd;
}
.nav-tabs > li.active > a,
.nav-tabs > li.active > a:hover,
.nav-tabs > li.active > a:focus {
  color: #555555;
  background-color: #fff;
  border: 1px solid #ddd;
  border-bottom-color: transparent;
  cursor: default;
}
.nav-tabs.nav-justified {
  width: 100%;
  border-bottom: 0;
}
.nav-tabs.nav-justified > li {
  float: none;
}
.nav-tabs.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-tabs.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-tabs.nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs.nav-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs.nav-justified > .active > a,
.nav-tabs.nav-justified > .active > a:hover,
.nav-tabs.nav-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs.nav-justified > .active > a,
  .nav-tabs.nav-justified > .active > a:hover,
  .nav-tabs.nav-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.nav-pills > li {
  float: left;
}
.nav-pills > li > a {
  border-radius: 2px;
}
.nav-pills > li + li {
  margin-left: 2px;
}
.nav-pills > li.active > a,
.nav-pills > li.active > a:hover,
.nav-pills > li.active > a:focus {
  color: #fff;
  background-color: #337ab7;
}
.nav-stacked > li {
  float: none;
}
.nav-stacked > li + li {
  margin-top: 2px;
  margin-left: 0;
}
.nav-justified {
  width: 100%;
}
.nav-justified > li {
  float: none;
}
.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs-justified {
  border-bottom: 0;
}
.nav-tabs-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs-justified > .active > a,
.nav-tabs-justified > .active > a:hover,
.nav-tabs-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs-justified > .active > a,
  .nav-tabs-justified > .active > a:hover,
  .nav-tabs-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.tab-content > .tab-pane {
  display: none;
}
.tab-content > .active {
  display: block;
}
.nav-tabs .dropdown-menu {
  margin-top: -1px;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar {
  position: relative;
  min-height: 30px;
  margin-bottom: 18px;
  border: 1px solid transparent;
}
@media (min-width: 541px) {
  .navbar {
    border-radius: 2px;
  }
}
@media (min-width: 541px) {
  .navbar-header {
    float: left;
  }
}
.navbar-collapse {
  overflow-x: visible;
  padding-right: 0px;
  padding-left: 0px;
  border-top: 1px solid transparent;
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
  -webkit-overflow-scrolling: touch;
}
.navbar-collapse.in {
  overflow-y: auto;
}
@media (min-width: 541px) {
  .navbar-collapse {
    width: auto;
    border-top: 0;
    box-shadow: none;
  }
  .navbar-collapse.collapse {
    display: block !important;
    height: auto !important;
    padding-bottom: 0;
    overflow: visible !important;
  }
  .navbar-collapse.in {
    overflow-y: visible;
  }
  .navbar-fixed-top .navbar-collapse,
  .navbar-static-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    padding-left: 0;
    padding-right: 0;
  }
}
.navbar-fixed-top .navbar-collapse,
.navbar-fixed-bottom .navbar-collapse {
  max-height: 340px;
}
@media (max-device-width: 540px) and (orientation: landscape) {
  .navbar-fixed-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    max-height: 200px;
  }
}
.container > .navbar-header,
.container-fluid > .navbar-header,
.container > .navbar-collapse,
.container-fluid > .navbar-collapse {
  margin-right: 0px;
  margin-left: 0px;
}
@media (min-width: 541px) {
  .container > .navbar-header,
  .container-fluid > .navbar-header,
  .container > .navbar-collapse,
  .container-fluid > .navbar-collapse {
    margin-right: 0;
    margin-left: 0;
  }
}
.navbar-static-top {
  z-index: 1000;
  border-width: 0 0 1px;
}
@media (min-width: 541px) {
  .navbar-static-top {
    border-radius: 0;
  }
}
.navbar-fixed-top,
.navbar-fixed-bottom {
  position: fixed;
  right: 0;
  left: 0;
  z-index: 1030;
}
@media (min-width: 541px) {
  .navbar-fixed-top,
  .navbar-fixed-bottom {
    border-radius: 0;
  }
}
.navbar-fixed-top {
  top: 0;
  border-width: 0 0 1px;
}
.navbar-fixed-bottom {
  bottom: 0;
  margin-bottom: 0;
  border-width: 1px 0 0;
}
.navbar-brand {
  float: left;
  padding: 6px 0px;
  font-size: 17px;
  line-height: 18px;
  height: 30px;
}
.navbar-brand:hover,
.navbar-brand:focus {
  text-decoration: none;
}
.navbar-brand > img {
  display: block;
}
@media (min-width: 541px) {
  .navbar > .container .navbar-brand,
  .navbar > .container-fluid .navbar-brand {
    margin-left: 0px;
  }
}
.navbar-toggle {
  position: relative;
  float: right;
  margin-right: 0px;
  padding: 9px 10px;
  margin-top: -2px;
  margin-bottom: -2px;
  background-color: transparent;
  background-image: none;
  border: 1px solid transparent;
  border-radius: 2px;
}
.navbar-toggle:focus {
  outline: 0;
}
.navbar-toggle .icon-bar {
  display: block;
  width: 22px;
  height: 2px;
  border-radius: 1px;
}
.navbar-toggle .icon-bar + .icon-bar {
  margin-top: 4px;
}
@media (min-width: 541px) {
  .navbar-toggle {
    display: none;
  }
}
.navbar-nav {
  margin: 3px 0px;
}
.navbar-nav > li > a {
  padding-top: 10px;
  padding-bottom: 10px;
  line-height: 18px;
}
@media (max-width: 540px) {
  .navbar-nav .open .dropdown-menu {
    position: static;
    float: none;
    width: auto;
    margin-top: 0;
    background-color: transparent;
    border: 0;
    box-shadow: none;
  }
  .navbar-nav .open .dropdown-menu > li > a,
  .navbar-nav .open .dropdown-menu .dropdown-header {
    padding: 5px 15px 5px 25px;
  }
  .navbar-nav .open .dropdown-menu > li > a {
    line-height: 18px;
  }
  .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-nav .open .dropdown-menu > li > a:focus {
    background-image: none;
  }
}
@media (min-width: 541px) {
  .navbar-nav {
    float: left;
    margin: 0;
  }
  .navbar-nav > li {
    float: left;
  }
  .navbar-nav > li > a {
    padding-top: 6px;
    padding-bottom: 6px;
  }
}
.navbar-form {
  margin-left: 0px;
  margin-right: 0px;
  padding: 10px 0px;
  border-top: 1px solid transparent;
  border-bottom: 1px solid transparent;
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  margin-top: -1px;
  margin-bottom: -1px;
}
@media (min-width: 768px) {
  .navbar-form .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .navbar-form .form-control-static {
    display: inline-block;
  }
  .navbar-form .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .navbar-form .input-group .input-group-addon,
  .navbar-form .input-group .input-group-btn,
  .navbar-form .input-group .form-control {
    width: auto;
  }
  .navbar-form .input-group > .form-control {
    width: 100%;
  }
  .navbar-form .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio,
  .navbar-form .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio label,
  .navbar-form .checkbox label {
    padding-left: 0;
  }
  .navbar-form .radio input[type="radio"],
  .navbar-form .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .navbar-form .has-feedback .form-control-feedback {
    top: 0;
  }
}
@media (max-width: 540px) {
  .navbar-form .form-group {
    margin-bottom: 5px;
  }
  .navbar-form .form-group:last-child {
    margin-bottom: 0;
  }
}
@media (min-width: 541px) {
  .navbar-form {
    width: auto;
    border: 0;
    margin-left: 0;
    margin-right: 0;
    padding-top: 0;
    padding-bottom: 0;
    -webkit-box-shadow: none;
    box-shadow: none;
  }
}
.navbar-nav > li > .dropdown-menu {
  margin-top: 0;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar-fixed-bottom .navbar-nav > li > .dropdown-menu {
  margin-bottom: 0;
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.navbar-btn {
  margin-top: -1px;
  margin-bottom: -1px;
}
.navbar-btn.btn-sm {
  margin-top: 0px;
  margin-bottom: 0px;
}
.navbar-btn.btn-xs {
  margin-top: 4px;
  margin-bottom: 4px;
}
.navbar-text {
  margin-top: 6px;
  margin-bottom: 6px;
}
@media (min-width: 541px) {
  .navbar-text {
    float: left;
    margin-left: 0px;
    margin-right: 0px;
  }
}
@media (min-width: 541px) {
  .navbar-left {
    float: left !important;
    float: left;
  }
  .navbar-right {
    float: right !important;
    float: right;
    margin-right: 0px;
  }
  .navbar-right ~ .navbar-right {
    margin-right: 0;
  }
}
.navbar-default {
  background-color: #f8f8f8;
  border-color: #e7e7e7;
}
.navbar-default .navbar-brand {
  color: #777;
}
.navbar-default .navbar-brand:hover,
.navbar-default .navbar-brand:focus {
  color: #5e5e5e;
  background-color: transparent;
}
.navbar-default .navbar-text {
  color: #777;
}
.navbar-default .navbar-nav > li > a {
  color: #777;
}
.navbar-default .navbar-nav > li > a:hover,
.navbar-default .navbar-nav > li > a:focus {
  color: #333;
  background-color: transparent;
}
.navbar-default .navbar-nav > .active > a,
.navbar-default .navbar-nav > .active > a:hover,
.navbar-default .navbar-nav > .active > a:focus {
  color: #555;
  background-color: #e7e7e7;
}
.navbar-default .navbar-nav > .disabled > a,
.navbar-default .navbar-nav > .disabled > a:hover,
.navbar-default .navbar-nav > .disabled > a:focus {
  color: #ccc;
  background-color: transparent;
}
.navbar-default .navbar-toggle {
  border-color: #ddd;
}
.navbar-default .navbar-toggle:hover,
.navbar-default .navbar-toggle:focus {
  background-color: #ddd;
}
.navbar-default .navbar-toggle .icon-bar {
  background-color: #888;
}
.navbar-default .navbar-collapse,
.navbar-default .navbar-form {
  border-color: #e7e7e7;
}
.navbar-default .navbar-nav > .open > a,
.navbar-default .navbar-nav > .open > a:hover,
.navbar-default .navbar-nav > .open > a:focus {
  background-color: #e7e7e7;
  color: #555;
}
@media (max-width: 540px) {
  .navbar-default .navbar-nav .open .dropdown-menu > li > a {
    color: #777;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #333;
    background-color: transparent;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #555;
    background-color: #e7e7e7;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #ccc;
    background-color: transparent;
  }
}
.navbar-default .navbar-link {
  color: #777;
}
.navbar-default .navbar-link:hover {
  color: #333;
}
.navbar-default .btn-link {
  color: #777;
}
.navbar-default .btn-link:hover,
.navbar-default .btn-link:focus {
  color: #333;
}
.navbar-default .btn-link[disabled]:hover,
fieldset[disabled] .navbar-default .btn-link:hover,
.navbar-default .btn-link[disabled]:focus,
fieldset[disabled] .navbar-default .btn-link:focus {
  color: #ccc;
}
.navbar-inverse {
  background-color: #222;
  border-color: #080808;
}
.navbar-inverse .navbar-brand {
  color: #9d9d9d;
}
.navbar-inverse .navbar-brand:hover,
.navbar-inverse .navbar-brand:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-text {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a:hover,
.navbar-inverse .navbar-nav > li > a:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-nav > .active > a,
.navbar-inverse .navbar-nav > .active > a:hover,
.navbar-inverse .navbar-nav > .active > a:focus {
  color: #fff;
  background-color: #080808;
}
.navbar-inverse .navbar-nav > .disabled > a,
.navbar-inverse .navbar-nav > .disabled > a:hover,
.navbar-inverse .navbar-nav > .disabled > a:focus {
  color: #444;
  background-color: transparent;
}
.navbar-inverse .navbar-toggle {
  border-color: #333;
}
.navbar-inverse .navbar-toggle:hover,
.navbar-inverse .navbar-toggle:focus {
  background-color: #333;
}
.navbar-inverse .navbar-toggle .icon-bar {
  background-color: #fff;
}
.navbar-inverse .navbar-collapse,
.navbar-inverse .navbar-form {
  border-color: #101010;
}
.navbar-inverse .navbar-nav > .open > a,
.navbar-inverse .navbar-nav > .open > a:hover,
.navbar-inverse .navbar-nav > .open > a:focus {
  background-color: #080808;
  color: #fff;
}
@media (max-width: 540px) {
  .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header {
    border-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu .divider {
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a {
    color: #9d9d9d;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #fff;
    background-color: transparent;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #fff;
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #444;
    background-color: transparent;
  }
}
.navbar-inverse .navbar-link {
  color: #9d9d9d;
}
.navbar-inverse .navbar-link:hover {
  color: #fff;
}
.navbar-inverse .btn-link {
  color: #9d9d9d;
}
.navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link:focus {
  color: #fff;
}
.navbar-inverse .btn-link[disabled]:hover,
fieldset[disabled] .navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link[disabled]:focus,
fieldset[disabled] .navbar-inverse .btn-link:focus {
  color: #444;
}
.breadcrumb {
  padding: 8px 15px;
  margin-bottom: 18px;
  list-style: none;
  background-color: #f5f5f5;
  border-radius: 2px;
}
.breadcrumb > li {
  display: inline-block;
}
.breadcrumb > li + li:before {
  content: "/\00a0";
  padding: 0 5px;
  color: #5e5e5e;
}
.breadcrumb > .active {
  color: #777777;
}
.pagination {
  display: inline-block;
  padding-left: 0;
  margin: 18px 0;
  border-radius: 2px;
}
.pagination > li {
  display: inline;
}
.pagination > li > a,
.pagination > li > span {
  position: relative;
  float: left;
  padding: 6px 12px;
  line-height: 1.42857143;
  text-decoration: none;
  color: #337ab7;
  background-color: #fff;
  border: 1px solid #ddd;
  margin-left: -1px;
}
.pagination > li:first-child > a,
.pagination > li:first-child > span {
  margin-left: 0;
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.pagination > li:last-child > a,
.pagination > li:last-child > span {
  border-bottom-right-radius: 2px;
  border-top-right-radius: 2px;
}
.pagination > li > a:hover,
.pagination > li > span:hover,
.pagination > li > a:focus,
.pagination > li > span:focus {
  z-index: 2;
  color: #23527c;
  background-color: #eeeeee;
  border-color: #ddd;
}
.pagination > .active > a,
.pagination > .active > span,
.pagination > .active > a:hover,
.pagination > .active > span:hover,
.pagination > .active > a:focus,
.pagination > .active > span:focus {
  z-index: 3;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
  cursor: default;
}
.pagination > .disabled > span,
.pagination > .disabled > span:hover,
.pagination > .disabled > span:focus,
.pagination > .disabled > a,
.pagination > .disabled > a:hover,
.pagination > .disabled > a:focus {
  color: #777777;
  background-color: #fff;
  border-color: #ddd;
  cursor: not-allowed;
}
.pagination-lg > li > a,
.pagination-lg > li > span {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.pagination-lg > li:first-child > a,
.pagination-lg > li:first-child > span {
  border-bottom-left-radius: 3px;
  border-top-left-radius: 3px;
}
.pagination-lg > li:last-child > a,
.pagination-lg > li:last-child > span {
  border-bottom-right-radius: 3px;
  border-top-right-radius: 3px;
}
.pagination-sm > li > a,
.pagination-sm > li > span {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.pagination-sm > li:first-child > a,
.pagination-sm > li:first-child > span {
  border-bottom-left-radius: 1px;
  border-top-left-radius: 1px;
}
.pagination-sm > li:last-child > a,
.pagination-sm > li:last-child > span {
  border-bottom-right-radius: 1px;
  border-top-right-radius: 1px;
}
.pager {
  padding-left: 0;
  margin: 18px 0;
  list-style: none;
  text-align: center;
}
.pager li {
  display: inline;
}
.pager li > a,
.pager li > span {
  display: inline-block;
  padding: 5px 14px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 15px;
}
.pager li > a:hover,
.pager li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.pager .next > a,
.pager .next > span {
  float: right;
}
.pager .previous > a,
.pager .previous > span {
  float: left;
}
.pager .disabled > a,
.pager .disabled > a:hover,
.pager .disabled > a:focus,
.pager .disabled > span {
  color: #777777;
  background-color: #fff;
  cursor: not-allowed;
}
.label {
  display: inline;
  padding: .2em .6em .3em;
  font-size: 75%;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-align: center;
  white-space: nowrap;
  vertical-align: baseline;
  border-radius: .25em;
}
a.label:hover,
a.label:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.label:empty {
  display: none;
}
.btn .label {
  position: relative;
  top: -1px;
}
.label-default {
  background-color: #777777;
}
.label-default[href]:hover,
.label-default[href]:focus {
  background-color: #5e5e5e;
}
.label-primary {
  background-color: #337ab7;
}
.label-primary[href]:hover,
.label-primary[href]:focus {
  background-color: #286090;
}
.label-success {
  background-color: #5cb85c;
}
.label-success[href]:hover,
.label-success[href]:focus {
  background-color: #449d44;
}
.label-info {
  background-color: #5bc0de;
}
.label-info[href]:hover,
.label-info[href]:focus {
  background-color: #31b0d5;
}
.label-warning {
  background-color: #f0ad4e;
}
.label-warning[href]:hover,
.label-warning[href]:focus {
  background-color: #ec971f;
}
.label-danger {
  background-color: #d9534f;
}
.label-danger[href]:hover,
.label-danger[href]:focus {
  background-color: #c9302c;
}
.badge {
  display: inline-block;
  min-width: 10px;
  padding: 3px 7px;
  font-size: 12px;
  font-weight: bold;
  color: #fff;
  line-height: 1;
  vertical-align: middle;
  white-space: nowrap;
  text-align: center;
  background-color: #777777;
  border-radius: 10px;
}
.badge:empty {
  display: none;
}
.btn .badge {
  position: relative;
  top: -1px;
}
.btn-xs .badge,
.btn-group-xs > .btn .badge {
  top: 0;
  padding: 1px 5px;
}
a.badge:hover,
a.badge:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.list-group-item.active > .badge,
.nav-pills > .active > a > .badge {
  color: #337ab7;
  background-color: #fff;
}
.list-group-item > .badge {
  float: right;
}
.list-group-item > .badge + .badge {
  margin-right: 5px;
}
.nav-pills > li > a > .badge {
  margin-left: 3px;
}
.jumbotron {
  padding-top: 30px;
  padding-bottom: 30px;
  margin-bottom: 30px;
  color: inherit;
  background-color: #eeeeee;
}
.jumbotron h1,
.jumbotron .h1 {
  color: inherit;
}
.jumbotron p {
  margin-bottom: 15px;
  font-size: 20px;
  font-weight: 200;
}
.jumbotron > hr {
  border-top-color: #d5d5d5;
}
.container .jumbotron,
.container-fluid .jumbotron {
  border-radius: 3px;
  padding-left: 0px;
  padding-right: 0px;
}
.jumbotron .container {
  max-width: 100%;
}
@media screen and (min-width: 768px) {
  .jumbotron {
    padding-top: 48px;
    padding-bottom: 48px;
  }
  .container .jumbotron,
  .container-fluid .jumbotron {
    padding-left: 60px;
    padding-right: 60px;
  }
  .jumbotron h1,
  .jumbotron .h1 {
    font-size: 59px;
  }
}
.thumbnail {
  display: block;
  padding: 4px;
  margin-bottom: 18px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: border 0.2s ease-in-out;
  -o-transition: border 0.2s ease-in-out;
  transition: border 0.2s ease-in-out;
}
.thumbnail > img,
.thumbnail a > img {
  margin-left: auto;
  margin-right: auto;
}
a.thumbnail:hover,
a.thumbnail:focus,
a.thumbnail.active {
  border-color: #337ab7;
}
.thumbnail .caption {
  padding: 9px;
  color: #000;
}
.alert {
  padding: 15px;
  margin-bottom: 18px;
  border: 1px solid transparent;
  border-radius: 2px;
}
.alert h4 {
  margin-top: 0;
  color: inherit;
}
.alert .alert-link {
  font-weight: bold;
}
.alert > p,
.alert > ul {
  margin-bottom: 0;
}
.alert > p + p {
  margin-top: 5px;
}
.alert-dismissable,
.alert-dismissible {
  padding-right: 35px;
}
.alert-dismissable .close,
.alert-dismissible .close {
  position: relative;
  top: -2px;
  right: -21px;
  color: inherit;
}
.alert-success {
  background-color: #dff0d8;
  border-color: #d6e9c6;
  color: #3c763d;
}
.alert-success hr {
  border-top-color: #c9e2b3;
}
.alert-success .alert-link {
  color: #2b542c;
}
.alert-info {
  background-color: #d9edf7;
  border-color: #bce8f1;
  color: #31708f;
}
.alert-info hr {
  border-top-color: #a6e1ec;
}
.alert-info .alert-link {
  color: #245269;
}
.alert-warning {
  background-color: #fcf8e3;
  border-color: #faebcc;
  color: #8a6d3b;
}
.alert-warning hr {
  border-top-color: #f7e1b5;
}
.alert-warning .alert-link {
  color: #66512c;
}
.alert-danger {
  background-color: #f2dede;
  border-color: #ebccd1;
  color: #a94442;
}
.alert-danger hr {
  border-top-color: #e4b9c0;
}
.alert-danger .alert-link {
  color: #843534;
}
@-webkit-keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
@keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
.progress {
  overflow: hidden;
  height: 18px;
  margin-bottom: 18px;
  background-color: #f5f5f5;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
}
.progress-bar {
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 18px;
  color: #fff;
  text-align: center;
  background-color: #337ab7;
  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  -webkit-transition: width 0.6s ease;
  -o-transition: width 0.6s ease;
  transition: width 0.6s ease;
}
.progress-striped .progress-bar,
.progress-bar-striped {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-size: 40px 40px;
}
.progress.active .progress-bar,
.progress-bar.active {
  -webkit-animation: progress-bar-stripes 2s linear infinite;
  -o-animation: progress-bar-stripes 2s linear infinite;
  animation: progress-bar-stripes 2s linear infinite;
}
.progress-bar-success {
  background-color: #5cb85c;
}
.progress-striped .progress-bar-success {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-info {
  background-color: #5bc0de;
}
.progress-striped .progress-bar-info {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-warning {
  background-color: #f0ad4e;
}
.progress-striped .progress-bar-warning {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-danger {
  background-color: #d9534f;
}
.progress-striped .progress-bar-danger {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.media {
  margin-top: 15px;
}
.media:first-child {
  margin-top: 0;
}
.media,
.media-body {
  zoom: 1;
  overflow: hidden;
}
.media-body {
  width: 10000px;
}
.media-object {
  display: block;
}
.media-object.img-thumbnail {
  max-width: none;
}
.media-right,
.media > .pull-right {
  padding-left: 10px;
}
.media-left,
.media > .pull-left {
  padding-right: 10px;
}
.media-left,
.media-right,
.media-body {
  display: table-cell;
  vertical-align: top;
}
.media-middle {
  vertical-align: middle;
}
.media-bottom {
  vertical-align: bottom;
}
.media-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.media-list {
  padding-left: 0;
  list-style: none;
}
.list-group {
  margin-bottom: 20px;
  padding-left: 0;
}
.list-group-item {
  position: relative;
  display: block;
  padding: 10px 15px;
  margin-bottom: -1px;
  background-color: #fff;
  border: 1px solid #ddd;
}
.list-group-item:first-child {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
}
.list-group-item:last-child {
  margin-bottom: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
a.list-group-item,
button.list-group-item {
  color: #555;
}
a.list-group-item .list-group-item-heading,
button.list-group-item .list-group-item-heading {
  color: #333;
}
a.list-group-item:hover,
button.list-group-item:hover,
a.list-group-item:focus,
button.list-group-item:focus {
  text-decoration: none;
  color: #555;
  background-color: #f5f5f5;
}
button.list-group-item {
  width: 100%;
  text-align: left;
}
.list-group-item.disabled,
.list-group-item.disabled:hover,
.list-group-item.disabled:focus {
  background-color: #eeeeee;
  color: #777777;
  cursor: not-allowed;
}
.list-group-item.disabled .list-group-item-heading,
.list-group-item.disabled:hover .list-group-item-heading,
.list-group-item.disabled:focus .list-group-item-heading {
  color: inherit;
}
.list-group-item.disabled .list-group-item-text,
.list-group-item.disabled:hover .list-group-item-text,
.list-group-item.disabled:focus .list-group-item-text {
  color: #777777;
}
.list-group-item.active,
.list-group-item.active:hover,
.list-group-item.active:focus {
  z-index: 2;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.list-group-item.active .list-group-item-heading,
.list-group-item.active:hover .list-group-item-heading,
.list-group-item.active:focus .list-group-item-heading,
.list-group-item.active .list-group-item-heading > small,
.list-group-item.active:hover .list-group-item-heading > small,
.list-group-item.active:focus .list-group-item-heading > small,
.list-group-item.active .list-group-item-heading > .small,
.list-group-item.active:hover .list-group-item-heading > .small,
.list-group-item.active:focus .list-group-item-heading > .small {
  color: inherit;
}
.list-group-item.active .list-group-item-text,
.list-group-item.active:hover .list-group-item-text,
.list-group-item.active:focus .list-group-item-text {
  color: #c7ddef;
}
.list-group-item-success {
  color: #3c763d;
  background-color: #dff0d8;
}
a.list-group-item-success,
button.list-group-item-success {
  color: #3c763d;
}
a.list-group-item-success .list-group-item-heading,
button.list-group-item-success .list-group-item-heading {
  color: inherit;
}
a.list-group-item-success:hover,
button.list-group-item-success:hover,
a.list-group-item-success:focus,
button.list-group-item-success:focus {
  color: #3c763d;
  background-color: #d0e9c6;
}
a.list-group-item-success.active,
button.list-group-item-success.active,
a.list-group-item-success.active:hover,
button.list-group-item-success.active:hover,
a.list-group-item-success.active:focus,
button.list-group-item-success.active:focus {
  color: #fff;
  background-color: #3c763d;
  border-color: #3c763d;
}
.list-group-item-info {
  color: #31708f;
  background-color: #d9edf7;
}
a.list-group-item-info,
button.list-group-item-info {
  color: #31708f;
}
a.list-group-item-info .list-group-item-heading,
button.list-group-item-info .list-group-item-heading {
  color: inherit;
}
a.list-group-item-info:hover,
button.list-group-item-info:hover,
a.list-group-item-info:focus,
button.list-group-item-info:focus {
  color: #31708f;
  background-color: #c4e3f3;
}
a.list-group-item-info.active,
button.list-group-item-info.active,
a.list-group-item-info.active:hover,
button.list-group-item-info.active:hover,
a.list-group-item-info.active:focus,
button.list-group-item-info.active:focus {
  color: #fff;
  background-color: #31708f;
  border-color: #31708f;
}
.list-group-item-warning {
  color: #8a6d3b;
  background-color: #fcf8e3;
}
a.list-group-item-warning,
button.list-group-item-warning {
  color: #8a6d3b;
}
a.list-group-item-warning .list-group-item-heading,
button.list-group-item-warning .list-group-item-heading {
  color: inherit;
}
a.list-group-item-warning:hover,
button.list-group-item-warning:hover,
a.list-group-item-warning:focus,
button.list-group-item-warning:focus {
  color: #8a6d3b;
  background-color: #faf2cc;
}
a.list-group-item-warning.active,
button.list-group-item-warning.active,
a.list-group-item-warning.active:hover,
button.list-group-item-warning.active:hover,
a.list-group-item-warning.active:focus,
button.list-group-item-warning.active:focus {
  color: #fff;
  background-color: #8a6d3b;
  border-color: #8a6d3b;
}
.list-group-item-danger {
  color: #a94442;
  background-color: #f2dede;
}
a.list-group-item-danger,
button.list-group-item-danger {
  color: #a94442;
}
a.list-group-item-danger .list-group-item-heading,
button.list-group-item-danger .list-group-item-heading {
  color: inherit;
}
a.list-group-item-danger:hover,
button.list-group-item-danger:hover,
a.list-group-item-danger:focus,
button.list-group-item-danger:focus {
  color: #a94442;
  background-color: #ebcccc;
}
a.list-group-item-danger.active,
button.list-group-item-danger.active,
a.list-group-item-danger.active:hover,
button.list-group-item-danger.active:hover,
a.list-group-item-danger.active:focus,
button.list-group-item-danger.active:focus {
  color: #fff;
  background-color: #a94442;
  border-color: #a94442;
}
.list-group-item-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.list-group-item-text {
  margin-bottom: 0;
  line-height: 1.3;
}
.panel {
  margin-bottom: 18px;
  background-color: #fff;
  border: 1px solid transparent;
  border-radius: 2px;
  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
}
.panel-body {
  padding: 15px;
}
.panel-heading {
  padding: 10px 15px;
  border-bottom: 1px solid transparent;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel-heading > .dropdown .dropdown-toggle {
  color: inherit;
}
.panel-title {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 15px;
  color: inherit;
}
.panel-title > a,
.panel-title > small,
.panel-title > .small,
.panel-title > small > a,
.panel-title > .small > a {
  color: inherit;
}
.panel-footer {
  padding: 10px 15px;
  background-color: #f5f5f5;
  border-top: 1px solid #ddd;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .list-group,
.panel > .panel-collapse > .list-group {
  margin-bottom: 0;
}
.panel > .list-group .list-group-item,
.panel > .panel-collapse > .list-group .list-group-item {
  border-width: 1px 0;
  border-radius: 0;
}
.panel > .list-group:first-child .list-group-item:first-child,
.panel > .panel-collapse > .list-group:first-child .list-group-item:first-child {
  border-top: 0;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .list-group:last-child .list-group-item:last-child,
.panel > .panel-collapse > .list-group:last-child .list-group-item:last-child {
  border-bottom: 0;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.panel-heading + .list-group .list-group-item:first-child {
  border-top-width: 0;
}
.list-group + .panel-footer {
  border-top-width: 0;
}
.panel > .table,
.panel > .table-responsive > .table,
.panel > .panel-collapse > .table {
  margin-bottom: 0;
}
.panel > .table caption,
.panel > .table-responsive > .table caption,
.panel > .panel-collapse > .table caption {
  padding-left: 15px;
  padding-right: 15px;
}
.panel > .table:first-child,
.panel > .table-responsive:first-child > .table:first-child {
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child {
  border-top-left-radius: 1px;
  border-top-right-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:first-child {
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:last-child {
  border-top-right-radius: 1px;
}
.panel > .table:last-child,
.panel > .table-responsive:last-child > .table:last-child {
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child {
  border-bottom-left-radius: 1px;
  border-bottom-right-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:first-child {
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:last-child {
  border-bottom-right-radius: 1px;
}
.panel > .panel-body + .table,
.panel > .panel-body + .table-responsive,
.panel > .table + .panel-body,
.panel > .table-responsive + .panel-body {
  border-top: 1px solid #ddd;
}
.panel > .table > tbody:first-child > tr:first-child th,
.panel > .table > tbody:first-child > tr:first-child td {
  border-top: 0;
}
.panel > .table-bordered,
.panel > .table-responsive > .table-bordered {
  border: 0;
}
.panel > .table-bordered > thead > tr > th:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:first-child,
.panel > .table-bordered > tbody > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:first-child,
.panel > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-bordered > thead > tr > td:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:first-child,
.panel > .table-bordered > tbody > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:first-child,
.panel > .table-bordered > tfoot > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:first-child {
  border-left: 0;
}
.panel > .table-bordered > thead > tr > th:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:last-child,
.panel > .table-bordered > tbody > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:last-child,
.panel > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-bordered > thead > tr > td:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:last-child,
.panel > .table-bordered > tbody > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:last-child,
.panel > .table-bordered > tfoot > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:last-child {
  border-right: 0;
}
.panel > .table-bordered > thead > tr:first-child > td,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > td,
.panel > .table-bordered > tbody > tr:first-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > td,
.panel > .table-bordered > thead > tr:first-child > th,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > th,
.panel > .table-bordered > tbody > tr:first-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > th {
  border-bottom: 0;
}
.panel > .table-bordered > tbody > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > td,
.panel > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-bordered > tbody > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > th,
.panel > .table-bordered > tfoot > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > th {
  border-bottom: 0;
}
.panel > .table-responsive {
  border: 0;
  margin-bottom: 0;
}
.panel-group {
  margin-bottom: 18px;
}
.panel-group .panel {
  margin-bottom: 0;
  border-radius: 2px;
}
.panel-group .panel + .panel {
  margin-top: 5px;
}
.panel-group .panel-heading {
  border-bottom: 0;
}
.panel-group .panel-heading + .panel-collapse > .panel-body,
.panel-group .panel-heading + .panel-collapse > .list-group {
  border-top: 1px solid #ddd;
}
.panel-group .panel-footer {
  border-top: 0;
}
.panel-group .panel-footer + .panel-collapse .panel-body {
  border-bottom: 1px solid #ddd;
}
.panel-default {
  border-color: #ddd;
}
.panel-default > .panel-heading {
  color: #333333;
  background-color: #f5f5f5;
  border-color: #ddd;
}
.panel-default > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ddd;
}
.panel-default > .panel-heading .badge {
  color: #f5f5f5;
  background-color: #333333;
}
.panel-default > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ddd;
}
.panel-primary {
  border-color: #337ab7;
}
.panel-primary > .panel-heading {
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.panel-primary > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #337ab7;
}
.panel-primary > .panel-heading .badge {
  color: #337ab7;
  background-color: #fff;
}
.panel-primary > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #337ab7;
}
.panel-success {
  border-color: #d6e9c6;
}
.panel-success > .panel-heading {
  color: #3c763d;
  background-color: #dff0d8;
  border-color: #d6e9c6;
}
.panel-success > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #d6e9c6;
}
.panel-success > .panel-heading .badge {
  color: #dff0d8;
  background-color: #3c763d;
}
.panel-success > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #d6e9c6;
}
.panel-info {
  border-color: #bce8f1;
}
.panel-info > .panel-heading {
  color: #31708f;
  background-color: #d9edf7;
  border-color: #bce8f1;
}
.panel-info > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #bce8f1;
}
.panel-info > .panel-heading .badge {
  color: #d9edf7;
  background-color: #31708f;
}
.panel-info > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #bce8f1;
}
.panel-warning {
  border-color: #faebcc;
}
.panel-warning > .panel-heading {
  color: #8a6d3b;
  background-color: #fcf8e3;
  border-color: #faebcc;
}
.panel-warning > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #faebcc;
}
.panel-warning > .panel-heading .badge {
  color: #fcf8e3;
  background-color: #8a6d3b;
}
.panel-warning > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #faebcc;
}
.panel-danger {
  border-color: #ebccd1;
}
.panel-danger > .panel-heading {
  color: #a94442;
  background-color: #f2dede;
  border-color: #ebccd1;
}
.panel-danger > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ebccd1;
}
.panel-danger > .panel-heading .badge {
  color: #f2dede;
  background-color: #a94442;
}
.panel-danger > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ebccd1;
}
.embed-responsive {
  position: relative;
  display: block;
  height: 0;
  padding: 0;
  overflow: hidden;
}
.embed-responsive .embed-responsive-item,
.embed-responsive iframe,
.embed-responsive embed,
.embed-responsive object,
.embed-responsive video {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  border: 0;
}
.embed-responsive-16by9 {
  padding-bottom: 56.25%;
}
.embed-responsive-4by3 {
  padding-bottom: 75%;
}
.well {
  min-height: 20px;
  padding: 19px;
  margin-bottom: 20px;
  background-color: #f5f5f5;
  border: 1px solid #e3e3e3;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
}
.well blockquote {
  border-color: #ddd;
  border-color: rgba(0, 0, 0, 0.15);
}
.well-lg {
  padding: 24px;
  border-radius: 3px;
}
.well-sm {
  padding: 9px;
  border-radius: 1px;
}
.close {
  float: right;
  font-size: 19.5px;
  font-weight: bold;
  line-height: 1;
  color: #000;
  text-shadow: 0 1px 0 #fff;
  opacity: 0.2;
  filter: alpha(opacity=20);
}
.close:hover,
.close:focus {
  color: #000;
  text-decoration: none;
  cursor: pointer;
  opacity: 0.5;
  filter: alpha(opacity=50);
}
button.close {
  padding: 0;
  cursor: pointer;
  background: transparent;
  border: 0;
  -webkit-appearance: none;
}
.modal-open {
  overflow: hidden;
}
.modal {
  display: none;
  overflow: hidden;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1050;
  -webkit-overflow-scrolling: touch;
  outline: 0;
}
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, -25%);
  -ms-transform: translate(0, -25%);
  -o-transform: translate(0, -25%);
  transform: translate(0, -25%);
  -webkit-transition: -webkit-transform 0.3s ease-out;
  -moz-transition: -moz-transform 0.3s ease-out;
  -o-transition: -o-transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
}
.modal.in .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
.modal-open .modal {
  overflow-x: hidden;
  overflow-y: auto;
}
.modal-dialog {
  position: relative;
  width: auto;
  margin: 10px;
}
.modal-content {
  position: relative;
  background-color: #fff;
  border: 1px solid #999;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  background-clip: padding-box;
  outline: 0;
}
.modal-backdrop {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1040;
  background-color: #000;
}
.modal-backdrop.fade {
  opacity: 0;
  filter: alpha(opacity=0);
}
.modal-backdrop.in {
  opacity: 0.5;
  filter: alpha(opacity=50);
}
.modal-header {
  padding: 15px;
  border-bottom: 1px solid #e5e5e5;
}
.modal-header .close {
  margin-top: -2px;
}
.modal-title {
  margin: 0;
  line-height: 1.42857143;
}
.modal-body {
  position: relative;
  padding: 15px;
}
.modal-footer {
  padding: 15px;
  text-align: right;
  border-top: 1px solid #e5e5e5;
}
.modal-footer .btn + .btn {
  margin-left: 5px;
  margin-bottom: 0;
}
.modal-footer .btn-group .btn + .btn {
  margin-left: -1px;
}
.modal-footer .btn-block + .btn-block {
  margin-left: 0;
}
.modal-scrollbar-measure {
  position: absolute;
  top: -9999px;
  width: 50px;
  height: 50px;
  overflow: scroll;
}
@media (min-width: 768px) {
  .modal-dialog {
    width: 600px;
    margin: 30px auto;
  }
  .modal-content {
    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
  }
  .modal-sm {
    width: 300px;
  }
}
@media (min-width: 992px) {
  .modal-lg {
    width: 900px;
  }
}
.tooltip {
  position: absolute;
  z-index: 1070;
  display: block;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 12px;
  opacity: 0;
  filter: alpha(opacity=0);
}
.tooltip.in {
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.tooltip.top {
  margin-top: -3px;
  padding: 5px 0;
}
.tooltip.right {
  margin-left: 3px;
  padding: 0 5px;
}
.tooltip.bottom {
  margin-top: 3px;
  padding: 5px 0;
}
.tooltip.left {
  margin-left: -3px;
  padding: 0 5px;
}
.tooltip-inner {
  max-width: 200px;
  padding: 3px 8px;
  color: #fff;
  text-align: center;
  background-color: #000;
  border-radius: 2px;
}
.tooltip-arrow {
  position: absolute;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.tooltip.top .tooltip-arrow {
  bottom: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-left .tooltip-arrow {
  bottom: 0;
  right: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-right .tooltip-arrow {
  bottom: 0;
  left: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.right .tooltip-arrow {
  top: 50%;
  left: 0;
  margin-top: -5px;
  border-width: 5px 5px 5px 0;
  border-right-color: #000;
}
.tooltip.left .tooltip-arrow {
  top: 50%;
  right: 0;
  margin-top: -5px;
  border-width: 5px 0 5px 5px;
  border-left-color: #000;
}
.tooltip.bottom .tooltip-arrow {
  top: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-left .tooltip-arrow {
  top: 0;
  right: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-right .tooltip-arrow {
  top: 0;
  left: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.popover {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1060;
  display: none;
  max-width: 276px;
  padding: 1px;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 13px;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
.popover.top {
  margin-top: -10px;
}
.popover.right {
  margin-left: 10px;
}
.popover.bottom {
  margin-top: 10px;
}
.popover.left {
  margin-left: -10px;
}
.popover-title {
  margin: 0;
  padding: 8px 14px;
  font-size: 13px;
  background-color: #f7f7f7;
  border-bottom: 1px solid #ebebeb;
  border-radius: 2px 2px 0 0;
}
.popover-content {
  padding: 9px 14px;
}
.popover > .arrow,
.popover > .arrow:after {
  position: absolute;
  display: block;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.popover > .arrow {
  border-width: 11px;
}
.popover > .arrow:after {
  border-width: 10px;
  content: "";
}
.popover.top > .arrow {
  left: 50%;
  margin-left: -11px;
  border-bottom-width: 0;
  border-top-color: #999999;
  border-top-color: rgba(0, 0, 0, 0.25);
  bottom: -11px;
}
.popover.top > .arrow:after {
  content: " ";
  bottom: 1px;
  margin-left: -10px;
  border-bottom-width: 0;
  border-top-color: #fff;
}
.popover.right > .arrow {
  top: 50%;
  left: -11px;
  margin-top: -11px;
  border-left-width: 0;
  border-right-color: #999999;
  border-right-color: rgba(0, 0, 0, 0.25);
}
.popover.right > .arrow:after {
  content: " ";
  left: 1px;
  bottom: -10px;
  border-left-width: 0;
  border-right-color: #fff;
}
.popover.bottom > .arrow {
  left: 50%;
  margin-left: -11px;
  border-top-width: 0;
  border-bottom-color: #999999;
  border-bottom-color: rgba(0, 0, 0, 0.25);
  top: -11px;
}
.popover.bottom > .arrow:after {
  content: " ";
  top: 1px;
  margin-left: -10px;
  border-top-width: 0;
  border-bottom-color: #fff;
}
.popover.left > .arrow {
  top: 50%;
  right: -11px;
  margin-top: -11px;
  border-right-width: 0;
  border-left-color: #999999;
  border-left-color: rgba(0, 0, 0, 0.25);
}
.popover.left > .arrow:after {
  content: " ";
  right: 1px;
  border-right-width: 0;
  border-left-color: #fff;
  bottom: -10px;
}
.carousel {
  position: relative;
}
.carousel-inner {
  position: relative;
  overflow: hidden;
  width: 100%;
}
.carousel-inner > .item {
  display: none;
  position: relative;
  -webkit-transition: 0.6s ease-in-out left;
  -o-transition: 0.6s ease-in-out left;
  transition: 0.6s ease-in-out left;
}
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  line-height: 1;
}
@media all and (transform-3d), (-webkit-transform-3d) {
  .carousel-inner > .item {
    -webkit-transition: -webkit-transform 0.6s ease-in-out;
    -moz-transition: -moz-transform 0.6s ease-in-out;
    -o-transition: -o-transform 0.6s ease-in-out;
    transition: transform 0.6s ease-in-out;
    -webkit-backface-visibility: hidden;
    -moz-backface-visibility: hidden;
    backface-visibility: hidden;
    -webkit-perspective: 1000px;
    -moz-perspective: 1000px;
    perspective: 1000px;
  }
  .carousel-inner > .item.next,
  .carousel-inner > .item.active.right {
    -webkit-transform: translate3d(100%, 0, 0);
    transform: translate3d(100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.prev,
  .carousel-inner > .item.active.left {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.next.left,
  .carousel-inner > .item.prev.right,
  .carousel-inner > .item.active {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    left: 0;
  }
}
.carousel-inner > .active,
.carousel-inner > .next,
.carousel-inner > .prev {
  display: block;
}
.carousel-inner > .active {
  left: 0;
}
.carousel-inner > .next,
.carousel-inner > .prev {
  position: absolute;
  top: 0;
  width: 100%;
}
.carousel-inner > .next {
  left: 100%;
}
.carousel-inner > .prev {
  left: -100%;
}
.carousel-inner > .next.left,
.carousel-inner > .prev.right {
  left: 0;
}
.carousel-inner > .active.left {
  left: -100%;
}
.carousel-inner > .active.right {
  left: 100%;
}
.carousel-control {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  width: 15%;
  opacity: 0.5;
  filter: alpha(opacity=50);
  font-size: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
  background-color: rgba(0, 0, 0, 0);
}
.carousel-control.left {
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);
}
.carousel-control.right {
  left: auto;
  right: 0;
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);
}
.carousel-control:hover,
.carousel-control:focus {
  outline: 0;
  color: #fff;
  text-decoration: none;
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.carousel-control .icon-prev,
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-left,
.carousel-control .glyphicon-chevron-right {
  position: absolute;
  top: 50%;
  margin-top: -10px;
  z-index: 5;
  display: inline-block;
}
.carousel-control .icon-prev,
.carousel-control .glyphicon-chevron-left {
  left: 50%;
  margin-left: -10px;
}
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-right {
  right: 50%;
  margin-right: -10px;
}
.carousel-control .icon-prev,
.carousel-control .icon-next {
  width: 20px;
  height: 20px;
  line-height: 1;
  font-family: serif;
}
.carousel-control .icon-prev:before {
  content: '\2039';
}
.carousel-control .icon-next:before {
  content: '\203a';
}
.carousel-indicators {
  position: absolute;
  bottom: 10px;
  left: 50%;
  z-index: 15;
  width: 60%;
  margin-left: -30%;
  padding-left: 0;
  list-style: none;
  text-align: center;
}
.carousel-indicators li {
  display: inline-block;
  width: 10px;
  height: 10px;
  margin: 1px;
  text-indent: -999px;
  border: 1px solid #fff;
  border-radius: 10px;
  cursor: pointer;
  background-color: #000 \9;
  background-color: rgba(0, 0, 0, 0);
}
.carousel-indicators .active {
  margin: 0;
  width: 12px;
  height: 12px;
  background-color: #fff;
}
.carousel-caption {
  position: absolute;
  left: 15%;
  right: 15%;
  bottom: 20px;
  z-index: 10;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
}
.carousel-caption .btn {
  text-shadow: none;
}
@media screen and (min-width: 768px) {
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-prev,
  .carousel-control .icon-next {
    width: 30px;
    height: 30px;
    margin-top: -10px;
    font-size: 30px;
  }
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .icon-prev {
    margin-left: -10px;
  }
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-next {
    margin-right: -10px;
  }
  .carousel-caption {
    left: 20%;
    right: 20%;
    padding-bottom: 30px;
  }
  .carousel-indicators {
    bottom: 20px;
  }
}
.clearfix:before,
.clearfix:after,
.dl-horizontal dd:before,
.dl-horizontal dd:after,
.container:before,
.container:after,
.container-fluid:before,
.container-fluid:after,
.row:before,
.row:after,
.form-horizontal .form-group:before,
.form-horizontal .form-group:after,
.btn-toolbar:before,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:before,
.btn-group-vertical > .btn-group:after,
.nav:before,
.nav:after,
.navbar:before,
.navbar:after,
.navbar-header:before,
.navbar-header:after,
.navbar-collapse:before,
.navbar-collapse:after,
.pager:before,
.pager:after,
.panel-body:before,
.panel-body:after,
.modal-header:before,
.modal-header:after,
.modal-footer:before,
.modal-footer:after,
.item_buttons:before,
.item_buttons:after {
  content: " ";
  display: table;
}
.clearfix:after,
.dl-horizontal dd:after,
.container:after,
.container-fluid:after,
.row:after,
.form-horizontal .form-group:after,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:after,
.nav:after,
.navbar:after,
.navbar-header:after,
.navbar-collapse:after,
.pager:after,
.panel-body:after,
.modal-header:after,
.modal-footer:after,
.item_buttons:after {
  clear: both;
}
.center-block {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.pull-right {
  float: right !important;
}
.pull-left {
  float: left !important;
}
.hide {
  display: none !important;
}
.show {
  display: block !important;
}
.invisible {
  visibility: hidden;
}
.text-hide {
  font: 0/0 a;
  color: transparent;
  text-shadow: none;
  background-color: transparent;
  border: 0;
}
.hidden {
  display: none !important;
}
.affix {
  position: fixed;
}
@-ms-viewport {
  width: device-width;
}
.visible-xs,
.visible-sm,
.visible-md,
.visible-lg {
  display: none !important;
}
.visible-xs-block,
.visible-xs-inline,
.visible-xs-inline-block,
.visible-sm-block,
.visible-sm-inline,
.visible-sm-inline-block,
.visible-md-block,
.visible-md-inline,
.visible-md-inline-block,
.visible-lg-block,
.visible-lg-inline,
.visible-lg-inline-block {
  display: none !important;
}
@media (max-width: 767px) {
  .visible-xs {
    display: block !important;
  }
  table.visible-xs {
    display: table !important;
  }
  tr.visible-xs {
    display: table-row !important;
  }
  th.visible-xs,
  td.visible-xs {
    display: table-cell !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-block {
    display: block !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline {
    display: inline !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm {
    display: block !important;
  }
  table.visible-sm {
    display: table !important;
  }
  tr.visible-sm {
    display: table-row !important;
  }
  th.visible-sm,
  td.visible-sm {
    display: table-cell !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-block {
    display: block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline {
    display: inline !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md {
    display: block !important;
  }
  table.visible-md {
    display: table !important;
  }
  tr.visible-md {
    display: table-row !important;
  }
  th.visible-md,
  td.visible-md {
    display: table-cell !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-block {
    display: block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline {
    display: inline !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg {
    display: block !important;
  }
  table.visible-lg {
    display: table !important;
  }
  tr.visible-lg {
    display: table-row !important;
  }
  th.visible-lg,
  td.visible-lg {
    display: table-cell !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-block {
    display: block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline {
    display: inline !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline-block {
    display: inline-block !important;
  }
}
@media (max-width: 767px) {
  .hidden-xs {
    display: none !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .hidden-sm {
    display: none !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .hidden-md {
    display: none !important;
  }
}
@media (min-width: 1200px) {
  .hidden-lg {
    display: none !important;
  }
}
.visible-print {
  display: none !important;
}
@media print {
  .visible-print {
    display: block !important;
  }
  table.visible-print {
    display: table !important;
  }
  tr.visible-print {
    display: table-row !important;
  }
  th.visible-print,
  td.visible-print {
    display: table-cell !important;
  }
}
.visible-print-block {
  display: none !important;
}
@media print {
  .visible-print-block {
    display: block !important;
  }
}
.visible-print-inline {
  display: none !important;
}
@media print {
  .visible-print-inline {
    display: inline !important;
  }
}
.visible-print-inline-block {
  display: none !important;
}
@media print {
  .visible-print-inline-block {
    display: inline-block !important;
  }
}
@media print {
  .hidden-print {
    display: none !important;
  }
}
/*!
*
* Font Awesome
*
*/
/*!
 *  Font Awesome 4.7.0 by @davegandy - http://fontawesome.io - @fontawesome
 *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
 */
/* FONT PATH
 * -------------------------- */
@font-face {
  font-family: 'FontAwesome';
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?v=4.7.0');
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?#iefix&v=4.7.0') format('embedded-opentype'), url('../components/font-awesome/fonts/fontawesome-webfont.woff2?v=4.7.0') format('woff2'), url('../components/font-awesome/fonts/fontawesome-webfont.woff?v=4.7.0') format('woff'), url('../components/font-awesome/fonts/fontawesome-webfont.ttf?v=4.7.0') format('truetype'), url('../components/font-awesome/fonts/fontawesome-webfont.svg?v=4.7.0#fontawesomeregular') format('svg');
  font-weight: normal;
  font-style: normal;
}
.fa {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
/* makes the font 33% larger relative to the icon container */
.fa-lg {
  font-size: 1.33333333em;
  line-height: 0.75em;
  vertical-align: -15%;
}
.fa-2x {
  font-size: 2em;
}
.fa-3x {
  font-size: 3em;
}
.fa-4x {
  font-size: 4em;
}
.fa-5x {
  font-size: 5em;
}
.fa-fw {
  width: 1.28571429em;
  text-align: center;
}
.fa-ul {
  padding-left: 0;
  margin-left: 2.14285714em;
  list-style-type: none;
}
.fa-ul > li {
  position: relative;
}
.fa-li {
  position: absolute;
  left: -2.14285714em;
  width: 2.14285714em;
  top: 0.14285714em;
  text-align: center;
}
.fa-li.fa-lg {
  left: -1.85714286em;
}
.fa-border {
  padding: .2em .25em .15em;
  border: solid 0.08em #eee;
  border-radius: .1em;
}
.fa-pull-left {
  float: left;
}
.fa-pull-right {
  float: right;
}
.fa.fa-pull-left {
  margin-right: .3em;
}
.fa.fa-pull-right {
  margin-left: .3em;
}
/* Deprecated as of 4.4.0 */
.pull-right {
  float: right;
}
.pull-left {
  float: left;
}
.fa.pull-left {
  margin-right: .3em;
}
.fa.pull-right {
  margin-left: .3em;
}
.fa-spin {
  -webkit-animation: fa-spin 2s infinite linear;
  animation: fa-spin 2s infinite linear;
}
.fa-pulse {
  -webkit-animation: fa-spin 1s infinite steps(8);
  animation: fa-spin 1s infinite steps(8);
}
@-webkit-keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
@keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
.fa-rotate-90 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=1)";
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
}
.fa-rotate-180 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=2)";
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
.fa-rotate-270 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=3)";
  -webkit-transform: rotate(270deg);
  -ms-transform: rotate(270deg);
  transform: rotate(270deg);
}
.fa-flip-horizontal {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1)";
  -webkit-transform: scale(-1, 1);
  -ms-transform: scale(-1, 1);
  transform: scale(-1, 1);
}
.fa-flip-vertical {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1)";
  -webkit-transform: scale(1, -1);
  -ms-transform: scale(1, -1);
  transform: scale(1, -1);
}
:root .fa-rotate-90,
:root .fa-rotate-180,
:root .fa-rotate-270,
:root .fa-flip-horizontal,
:root .fa-flip-vertical {
  filter: none;
}
.fa-stack {
  position: relative;
  display: inline-block;
  width: 2em;
  height: 2em;
  line-height: 2em;
  vertical-align: middle;
}
.fa-stack-1x,
.fa-stack-2x {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}
.fa-stack-1x {
  line-height: inherit;
}
.fa-stack-2x {
  font-size: 2em;
}
.fa-inverse {
  color: #fff;
}
/* Font Awesome uses the Unicode Private Use Area (PUA) to ensure screen
   readers do not read off random characters that represent icons */
.fa-glass:before {
  content: "\f000";
}
.fa-music:before {
  content: "\f001";
}
.fa-search:before {
  content: "\f002";
}
.fa-envelope-o:before {
  content: "\f003";
}
.fa-heart:before {
  content: "\f004";
}
.fa-star:before {
  content: "\f005";
}
.fa-star-o:before {
  content: "\f006";
}
.fa-user:before {
  content: "\f007";
}
.fa-film:before {
  content: "\f008";
}
.fa-th-large:before {
  content: "\f009";
}
.fa-th:before {
  content: "\f00a";
}
.fa-th-list:before {
  content: "\f00b";
}
.fa-check:before {
  content: "\f00c";
}
.fa-remove:before,
.fa-close:before,
.fa-times:before {
  content: "\f00d";
}
.fa-search-plus:before {
  content: "\f00e";
}
.fa-search-minus:before {
  content: "\f010";
}
.fa-power-off:before {
  content: "\f011";
}
.fa-signal:before {
  content: "\f012";
}
.fa-gear:before,
.fa-cog:before {
  content: "\f013";
}
.fa-trash-o:before {
  content: "\f014";
}
.fa-home:before {
  content: "\f015";
}
.fa-file-o:before {
  content: "\f016";
}
.fa-clock-o:before {
  content: "\f017";
}
.fa-road:before {
  content: "\f018";
}
.fa-download:before {
  content: "\f019";
}
.fa-arrow-circle-o-down:before {
  content: "\f01a";
}
.fa-arrow-circle-o-up:before {
  content: "\f01b";
}
.fa-inbox:before {
  content: "\f01c";
}
.fa-play-circle-o:before {
  content: "\f01d";
}
.fa-rotate-right:before,
.fa-repeat:before {
  content: "\f01e";
}
.fa-refresh:before {
  content: "\f021";
}
.fa-list-alt:before {
  content: "\f022";
}
.fa-lock:before {
  content: "\f023";
}
.fa-flag:before {
  content: "\f024";
}
.fa-headphones:before {
  content: "\f025";
}
.fa-volume-off:before {
  content: "\f026";
}
.fa-volume-down:before {
  content: "\f027";
}
.fa-volume-up:before {
  content: "\f028";
}
.fa-qrcode:before {
  content: "\f029";
}
.fa-barcode:before {
  content: "\f02a";
}
.fa-tag:before {
  content: "\f02b";
}
.fa-tags:before {
  content: "\f02c";
}
.fa-book:before {
  content: "\f02d";
}
.fa-bookmark:before {
  content: "\f02e";
}
.fa-print:before {
  content: "\f02f";
}
.fa-camera:before {
  content: "\f030";
}
.fa-font:before {
  content: "\f031";
}
.fa-bold:before {
  content: "\f032";
}
.fa-italic:before {
  content: "\f033";
}
.fa-text-height:before {
  content: "\f034";
}
.fa-text-width:before {
  content: "\f035";
}
.fa-align-left:before {
  content: "\f036";
}
.fa-align-center:before {
  content: "\f037";
}
.fa-align-right:before {
  content: "\f038";
}
.fa-align-justify:before {
  content: "\f039";
}
.fa-list:before {
  content: "\f03a";
}
.fa-dedent:before,
.fa-outdent:before {
  content: "\f03b";
}
.fa-indent:before {
  content: "\f03c";
}
.fa-video-camera:before {
  content: "\f03d";
}
.fa-photo:before,
.fa-image:before,
.fa-picture-o:before {
  content: "\f03e";
}
.fa-pencil:before {
  content: "\f040";
}
.fa-map-marker:before {
  content: "\f041";
}
.fa-adjust:before {
  content: "\f042";
}
.fa-tint:before {
  content: "\f043";
}
.fa-edit:before,
.fa-pencil-square-o:before {
  content: "\f044";
}
.fa-share-square-o:before {
  content: "\f045";
}
.fa-check-square-o:before {
  content: "\f046";
}
.fa-arrows:before {
  content: "\f047";
}
.fa-step-backward:before {
  content: "\f048";
}
.fa-fast-backward:before {
  content: "\f049";
}
.fa-backward:before {
  content: "\f04a";
}
.fa-play:before {
  content: "\f04b";
}
.fa-pause:before {
  content: "\f04c";
}
.fa-stop:before {
  content: "\f04d";
}
.fa-forward:before {
  content: "\f04e";
}
.fa-fast-forward:before {
  content: "\f050";
}
.fa-step-forward:before {
  content: "\f051";
}
.fa-eject:before {
  content: "\f052";
}
.fa-chevron-left:before {
  content: "\f053";
}
.fa-chevron-right:before {
  content: "\f054";
}
.fa-plus-circle:before {
  content: "\f055";
}
.fa-minus-circle:before {
  content: "\f056";
}
.fa-times-circle:before {
  content: "\f057";
}
.fa-check-circle:before {
  content: "\f058";
}
.fa-question-circle:before {
  content: "\f059";
}
.fa-info-circle:before {
  content: "\f05a";
}
.fa-crosshairs:before {
  content: "\f05b";
}
.fa-times-circle-o:before {
  content: "\f05c";
}
.fa-check-circle-o:before {
  content: "\f05d";
}
.fa-ban:before {
  content: "\f05e";
}
.fa-arrow-left:before {
  content: "\f060";
}
.fa-arrow-right:before {
  content: "\f061";
}
.fa-arrow-up:before {
  content: "\f062";
}
.fa-arrow-down:before {
  content: "\f063";
}
.fa-mail-forward:before,
.fa-share:before {
  content: "\f064";
}
.fa-expand:before {
  content: "\f065";
}
.fa-compress:before {
  content: "\f066";
}
.fa-plus:before {
  content: "\f067";
}
.fa-minus:before {
  content: "\f068";
}
.fa-asterisk:before {
  content: "\f069";
}
.fa-exclamation-circle:before {
  content: "\f06a";
}
.fa-gift:before {
  content: "\f06b";
}
.fa-leaf:before {
  content: "\f06c";
}
.fa-fire:before {
  content: "\f06d";
}
.fa-eye:before {
  content: "\f06e";
}
.fa-eye-slash:before {
  content: "\f070";
}
.fa-warning:before,
.fa-exclamation-triangle:before {
  content: "\f071";
}
.fa-plane:before {
  content: "\f072";
}
.fa-calendar:before {
  content: "\f073";
}
.fa-random:before {
  content: "\f074";
}
.fa-comment:before {
  content: "\f075";
}
.fa-magnet:before {
  content: "\f076";
}
.fa-chevron-up:before {
  content: "\f077";
}
.fa-chevron-down:before {
  content: "\f078";
}
.fa-retweet:before {
  content: "\f079";
}
.fa-shopping-cart:before {
  content: "\f07a";
}
.fa-folder:before {
  content: "\f07b";
}
.fa-folder-open:before {
  content: "\f07c";
}
.fa-arrows-v:before {
  content: "\f07d";
}
.fa-arrows-h:before {
  content: "\f07e";
}
.fa-bar-chart-o:before,
.fa-bar-chart:before {
  content: "\f080";
}
.fa-twitter-square:before {
  content: "\f081";
}
.fa-facebook-square:before {
  content: "\f082";
}
.fa-camera-retro:before {
  content: "\f083";
}
.fa-key:before {
  content: "\f084";
}
.fa-gears:before,
.fa-cogs:before {
  content: "\f085";
}
.fa-comments:before {
  content: "\f086";
}
.fa-thumbs-o-up:before {
  content: "\f087";
}
.fa-thumbs-o-down:before {
  content: "\f088";
}
.fa-star-half:before {
  content: "\f089";
}
.fa-heart-o:before {
  content: "\f08a";
}
.fa-sign-out:before {
  content: "\f08b";
}
.fa-linkedin-square:before {
  content: "\f08c";
}
.fa-thumb-tack:before {
  content: "\f08d";
}
.fa-external-link:before {
  content: "\f08e";
}
.fa-sign-in:before {
  content: "\f090";
}
.fa-trophy:before {
  content: "\f091";
}
.fa-github-square:before {
  content: "\f092";
}
.fa-upload:before {
  content: "\f093";
}
.fa-lemon-o:before {
  content: "\f094";
}
.fa-phone:before {
  content: "\f095";
}
.fa-square-o:before {
  content: "\f096";
}
.fa-bookmark-o:before {
  content: "\f097";
}
.fa-phone-square:before {
  content: "\f098";
}
.fa-twitter:before {
  content: "\f099";
}
.fa-facebook-f:before,
.fa-facebook:before {
  content: "\f09a";
}
.fa-github:before {
  content: "\f09b";
}
.fa-unlock:before {
  content: "\f09c";
}
.fa-credit-card:before {
  content: "\f09d";
}
.fa-feed:before,
.fa-rss:before {
  content: "\f09e";
}
.fa-hdd-o:before {
  content: "\f0a0";
}
.fa-bullhorn:before {
  content: "\f0a1";
}
.fa-bell:before {
  content: "\f0f3";
}
.fa-certificate:before {
  content: "\f0a3";
}
.fa-hand-o-right:before {
  content: "\f0a4";
}
.fa-hand-o-left:before {
  content: "\f0a5";
}
.fa-hand-o-up:before {
  content: "\f0a6";
}
.fa-hand-o-down:before {
  content: "\f0a7";
}
.fa-arrow-circle-left:before {
  content: "\f0a8";
}
.fa-arrow-circle-right:before {
  content: "\f0a9";
}
.fa-arrow-circle-up:before {
  content: "\f0aa";
}
.fa-arrow-circle-down:before {
  content: "\f0ab";
}
.fa-globe:before {
  content: "\f0ac";
}
.fa-wrench:before {
  content: "\f0ad";
}
.fa-tasks:before {
  content: "\f0ae";
}
.fa-filter:before {
  content: "\f0b0";
}
.fa-briefcase:before {
  content: "\f0b1";
}
.fa-arrows-alt:before {
  content: "\f0b2";
}
.fa-group:before,
.fa-users:before {
  content: "\f0c0";
}
.fa-chain:before,
.fa-link:before {
  content: "\f0c1";
}
.fa-cloud:before {
  content: "\f0c2";
}
.fa-flask:before {
  content: "\f0c3";
}
.fa-cut:before,
.fa-scissors:before {
  content: "\f0c4";
}
.fa-copy:before,
.fa-files-o:before {
  content: "\f0c5";
}
.fa-paperclip:before {
  content: "\f0c6";
}
.fa-save:before,
.fa-floppy-o:before {
  content: "\f0c7";
}
.fa-square:before {
  content: "\f0c8";
}
.fa-navicon:before,
.fa-reorder:before,
.fa-bars:before {
  content: "\f0c9";
}
.fa-list-ul:before {
  content: "\f0ca";
}
.fa-list-ol:before {
  content: "\f0cb";
}
.fa-strikethrough:before {
  content: "\f0cc";
}
.fa-underline:before {
  content: "\f0cd";
}
.fa-table:before {
  content: "\f0ce";
}
.fa-magic:before {
  content: "\f0d0";
}
.fa-truck:before {
  content: "\f0d1";
}
.fa-pinterest:before {
  content: "\f0d2";
}
.fa-pinterest-square:before {
  content: "\f0d3";
}
.fa-google-plus-square:before {
  content: "\f0d4";
}
.fa-google-plus:before {
  content: "\f0d5";
}
.fa-money:before {
  content: "\f0d6";
}
.fa-caret-down:before {
  content: "\f0d7";
}
.fa-caret-up:before {
  content: "\f0d8";
}
.fa-caret-left:before {
  content: "\f0d9";
}
.fa-caret-right:before {
  content: "\f0da";
}
.fa-columns:before {
  content: "\f0db";
}
.fa-unsorted:before,
.fa-sort:before {
  content: "\f0dc";
}
.fa-sort-down:before,
.fa-sort-desc:before {
  content: "\f0dd";
}
.fa-sort-up:before,
.fa-sort-asc:before {
  content: "\f0de";
}
.fa-envelope:before {
  content: "\f0e0";
}
.fa-linkedin:before {
  content: "\f0e1";
}
.fa-rotate-left:before,
.fa-undo:before {
  content: "\f0e2";
}
.fa-legal:before,
.fa-gavel:before {
  content: "\f0e3";
}
.fa-dashboard:before,
.fa-tachometer:before {
  content: "\f0e4";
}
.fa-comment-o:before {
  content: "\f0e5";
}
.fa-comments-o:before {
  content: "\f0e6";
}
.fa-flash:before,
.fa-bolt:before {
  content: "\f0e7";
}
.fa-sitemap:before {
  content: "\f0e8";
}
.fa-umbrella:before {
  content: "\f0e9";
}
.fa-paste:before,
.fa-clipboard:before {
  content: "\f0ea";
}
.fa-lightbulb-o:before {
  content: "\f0eb";
}
.fa-exchange:before {
  content: "\f0ec";
}
.fa-cloud-download:before {
  content: "\f0ed";
}
.fa-cloud-upload:before {
  content: "\f0ee";
}
.fa-user-md:before {
  content: "\f0f0";
}
.fa-stethoscope:before {
  content: "\f0f1";
}
.fa-suitcase:before {
  content: "\f0f2";
}
.fa-bell-o:before {
  content: "\f0a2";
}
.fa-coffee:before {
  content: "\f0f4";
}
.fa-cutlery:before {
  content: "\f0f5";
}
.fa-file-text-o:before {
  content: "\f0f6";
}
.fa-building-o:before {
  content: "\f0f7";
}
.fa-hospital-o:before {
  content: "\f0f8";
}
.fa-ambulance:before {
  content: "\f0f9";
}
.fa-medkit:before {
  content: "\f0fa";
}
.fa-fighter-jet:before {
  content: "\f0fb";
}
.fa-beer:before {
  content: "\f0fc";
}
.fa-h-square:before {
  content: "\f0fd";
}
.fa-plus-square:before {
  content: "\f0fe";
}
.fa-angle-double-left:before {
  content: "\f100";
}
.fa-angle-double-right:before {
  content: "\f101";
}
.fa-angle-double-up:before {
  content: "\f102";
}
.fa-angle-double-down:before {
  content: "\f103";
}
.fa-angle-left:before {
  content: "\f104";
}
.fa-angle-right:before {
  content: "\f105";
}
.fa-angle-up:before {
  content: "\f106";
}
.fa-angle-down:before {
  content: "\f107";
}
.fa-desktop:before {
  content: "\f108";
}
.fa-laptop:before {
  content: "\f109";
}
.fa-tablet:before {
  content: "\f10a";
}
.fa-mobile-phone:before,
.fa-mobile:before {
  content: "\f10b";
}
.fa-circle-o:before {
  content: "\f10c";
}
.fa-quote-left:before {
  content: "\f10d";
}
.fa-quote-right:before {
  content: "\f10e";
}
.fa-spinner:before {
  content: "\f110";
}
.fa-circle:before {
  content: "\f111";
}
.fa-mail-reply:before,
.fa-reply:before {
  content: "\f112";
}
.fa-github-alt:before {
  content: "\f113";
}
.fa-folder-o:before {
  content: "\f114";
}
.fa-folder-open-o:before {
  content: "\f115";
}
.fa-smile-o:before {
  content: "\f118";
}
.fa-frown-o:before {
  content: "\f119";
}
.fa-meh-o:before {
  content: "\f11a";
}
.fa-gamepad:before {
  content: "\f11b";
}
.fa-keyboard-o:before {
  content: "\f11c";
}
.fa-flag-o:before {
  content: "\f11d";
}
.fa-flag-checkered:before {
  content: "\f11e";
}
.fa-terminal:before {
  content: "\f120";
}
.fa-code:before {
  content: "\f121";
}
.fa-mail-reply-all:before,
.fa-reply-all:before {
  content: "\f122";
}
.fa-star-half-empty:before,
.fa-star-half-full:before,
.fa-star-half-o:before {
  content: "\f123";
}
.fa-location-arrow:before {
  content: "\f124";
}
.fa-crop:before {
  content: "\f125";
}
.fa-code-fork:before {
  content: "\f126";
}
.fa-unlink:before,
.fa-chain-broken:before {
  content: "\f127";
}
.fa-question:before {
  content: "\f128";
}
.fa-info:before {
  content: "\f129";
}
.fa-exclamation:before {
  content: "\f12a";
}
.fa-superscript:before {
  content: "\f12b";
}
.fa-subscript:before {
  content: "\f12c";
}
.fa-eraser:before {
  content: "\f12d";
}
.fa-puzzle-piece:before {
  content: "\f12e";
}
.fa-microphone:before {
  content: "\f130";
}
.fa-microphone-slash:before {
  content: "\f131";
}
.fa-shield:before {
  content: "\f132";
}
.fa-calendar-o:before {
  content: "\f133";
}
.fa-fire-extinguisher:before {
  content: "\f134";
}
.fa-rocket:before {
  content: "\f135";
}
.fa-maxcdn:before {
  content: "\f136";
}
.fa-chevron-circle-left:before {
  content: "\f137";
}
.fa-chevron-circle-right:before {
  content: "\f138";
}
.fa-chevron-circle-up:before {
  content: "\f139";
}
.fa-chevron-circle-down:before {
  content: "\f13a";
}
.fa-html5:before {
  content: "\f13b";
}
.fa-css3:before {
  content: "\f13c";
}
.fa-anchor:before {
  content: "\f13d";
}
.fa-unlock-alt:before {
  content: "\f13e";
}
.fa-bullseye:before {
  content: "\f140";
}
.fa-ellipsis-h:before {
  content: "\f141";
}
.fa-ellipsis-v:before {
  content: "\f142";
}
.fa-rss-square:before {
  content: "\f143";
}
.fa-play-circle:before {
  content: "\f144";
}
.fa-ticket:before {
  content: "\f145";
}
.fa-minus-square:before {
  content: "\f146";
}
.fa-minus-square-o:before {
  content: "\f147";
}
.fa-level-up:before {
  content: "\f148";
}
.fa-level-down:before {
  content: "\f149";
}
.fa-check-square:before {
  content: "\f14a";
}
.fa-pencil-square:before {
  content: "\f14b";
}
.fa-external-link-square:before {
  content: "\f14c";
}
.fa-share-square:before {
  content: "\f14d";
}
.fa-compass:before {
  content: "\f14e";
}
.fa-toggle-down:before,
.fa-caret-square-o-down:before {
  content: "\f150";
}
.fa-toggle-up:before,
.fa-caret-square-o-up:before {
  content: "\f151";
}
.fa-toggle-right:before,
.fa-caret-square-o-right:before {
  content: "\f152";
}
.fa-euro:before,
.fa-eur:before {
  content: "\f153";
}
.fa-gbp:before {
  content: "\f154";
}
.fa-dollar:before,
.fa-usd:before {
  content: "\f155";
}
.fa-rupee:before,
.fa-inr:before {
  content: "\f156";
}
.fa-cny:before,
.fa-rmb:before,
.fa-yen:before,
.fa-jpy:before {
  content: "\f157";
}
.fa-ruble:before,
.fa-rouble:before,
.fa-rub:before {
  content: "\f158";
}
.fa-won:before,
.fa-krw:before {
  content: "\f159";
}
.fa-bitcoin:before,
.fa-btc:before {
  content: "\f15a";
}
.fa-file:before {
  content: "\f15b";
}
.fa-file-text:before {
  content: "\f15c";
}
.fa-sort-alpha-asc:before {
  content: "\f15d";
}
.fa-sort-alpha-desc:before {
  content: "\f15e";
}
.fa-sort-amount-asc:before {
  content: "\f160";
}
.fa-sort-amount-desc:before {
  content: "\f161";
}
.fa-sort-numeric-asc:before {
  content: "\f162";
}
.fa-sort-numeric-desc:before {
  content: "\f163";
}
.fa-thumbs-up:before {
  content: "\f164";
}
.fa-thumbs-down:before {
  content: "\f165";
}
.fa-youtube-square:before {
  content: "\f166";
}
.fa-youtube:before {
  content: "\f167";
}
.fa-xing:before {
  content: "\f168";
}
.fa-xing-square:before {
  content: "\f169";
}
.fa-youtube-play:before {
  content: "\f16a";
}
.fa-dropbox:before {
  content: "\f16b";
}
.fa-stack-overflow:before {
  content: "\f16c";
}
.fa-instagram:before {
  content: "\f16d";
}
.fa-flickr:before {
  content: "\f16e";
}
.fa-adn:before {
  content: "\f170";
}
.fa-bitbucket:before {
  content: "\f171";
}
.fa-bitbucket-square:before {
  content: "\f172";
}
.fa-tumblr:before {
  content: "\f173";
}
.fa-tumblr-square:before {
  content: "\f174";
}
.fa-long-arrow-down:before {
  content: "\f175";
}
.fa-long-arrow-up:before {
  content: "\f176";
}
.fa-long-arrow-left:before {
  content: "\f177";
}
.fa-long-arrow-right:before {
  content: "\f178";
}
.fa-apple:before {
  content: "\f179";
}
.fa-windows:before {
  content: "\f17a";
}
.fa-android:before {
  content: "\f17b";
}
.fa-linux:before {
  content: "\f17c";
}
.fa-dribbble:before {
  content: "\f17d";
}
.fa-skype:before {
  content: "\f17e";
}
.fa-foursquare:before {
  content: "\f180";
}
.fa-trello:before {
  content: "\f181";
}
.fa-female:before {
  content: "\f182";
}
.fa-male:before {
  content: "\f183";
}
.fa-gittip:before,
.fa-gratipay:before {
  content: "\f184";
}
.fa-sun-o:before {
  content: "\f185";
}
.fa-moon-o:before {
  content: "\f186";
}
.fa-archive:before {
  content: "\f187";
}
.fa-bug:before {
  content: "\f188";
}
.fa-vk:before {
  content: "\f189";
}
.fa-weibo:before {
  content: "\f18a";
}
.fa-renren:before {
  content: "\f18b";
}
.fa-pagelines:before {
  content: "\f18c";
}
.fa-stack-exchange:before {
  content: "\f18d";
}
.fa-arrow-circle-o-right:before {
  content: "\f18e";
}
.fa-arrow-circle-o-left:before {
  content: "\f190";
}
.fa-toggle-left:before,
.fa-caret-square-o-left:before {
  content: "\f191";
}
.fa-dot-circle-o:before {
  content: "\f192";
}
.fa-wheelchair:before {
  content: "\f193";
}
.fa-vimeo-square:before {
  content: "\f194";
}
.fa-turkish-lira:before,
.fa-try:before {
  content: "\f195";
}
.fa-plus-square-o:before {
  content: "\f196";
}
.fa-space-shuttle:before {
  content: "\f197";
}
.fa-slack:before {
  content: "\f198";
}
.fa-envelope-square:before {
  content: "\f199";
}
.fa-wordpress:before {
  content: "\f19a";
}
.fa-openid:before {
  content: "\f19b";
}
.fa-institution:before,
.fa-bank:before,
.fa-university:before {
  content: "\f19c";
}
.fa-mortar-board:before,
.fa-graduation-cap:before {
  content: "\f19d";
}
.fa-yahoo:before {
  content: "\f19e";
}
.fa-google:before {
  content: "\f1a0";
}
.fa-reddit:before {
  content: "\f1a1";
}
.fa-reddit-square:before {
  content: "\f1a2";
}
.fa-stumbleupon-circle:before {
  content: "\f1a3";
}
.fa-stumbleupon:before {
  content: "\f1a4";
}
.fa-delicious:before {
  content: "\f1a5";
}
.fa-digg:before {
  content: "\f1a6";
}
.fa-pied-piper-pp:before {
  content: "\f1a7";
}
.fa-pied-piper-alt:before {
  content: "\f1a8";
}
.fa-drupal:before {
  content: "\f1a9";
}
.fa-joomla:before {
  content: "\f1aa";
}
.fa-language:before {
  content: "\f1ab";
}
.fa-fax:before {
  content: "\f1ac";
}
.fa-building:before {
  content: "\f1ad";
}
.fa-child:before {
  content: "\f1ae";
}
.fa-paw:before {
  content: "\f1b0";
}
.fa-spoon:before {
  content: "\f1b1";
}
.fa-cube:before {
  content: "\f1b2";
}
.fa-cubes:before {
  content: "\f1b3";
}
.fa-behance:before {
  content: "\f1b4";
}
.fa-behance-square:before {
  content: "\f1b5";
}
.fa-steam:before {
  content: "\f1b6";
}
.fa-steam-square:before {
  content: "\f1b7";
}
.fa-recycle:before {
  content: "\f1b8";
}
.fa-automobile:before,
.fa-car:before {
  content: "\f1b9";
}
.fa-cab:before,
.fa-taxi:before {
  content: "\f1ba";
}
.fa-tree:before {
  content: "\f1bb";
}
.fa-spotify:before {
  content: "\f1bc";
}
.fa-deviantart:before {
  content: "\f1bd";
}
.fa-soundcloud:before {
  content: "\f1be";
}
.fa-database:before {
  content: "\f1c0";
}
.fa-file-pdf-o:before {
  content: "\f1c1";
}
.fa-file-word-o:before {
  content: "\f1c2";
}
.fa-file-excel-o:before {
  content: "\f1c3";
}
.fa-file-powerpoint-o:before {
  content: "\f1c4";
}
.fa-file-photo-o:before,
.fa-file-picture-o:before,
.fa-file-image-o:before {
  content: "\f1c5";
}
.fa-file-zip-o:before,
.fa-file-archive-o:before {
  content: "\f1c6";
}
.fa-file-sound-o:before,
.fa-file-audio-o:before {
  content: "\f1c7";
}
.fa-file-movie-o:before,
.fa-file-video-o:before {
  content: "\f1c8";
}
.fa-file-code-o:before {
  content: "\f1c9";
}
.fa-vine:before {
  content: "\f1ca";
}
.fa-codepen:before {
  content: "\f1cb";
}
.fa-jsfiddle:before {
  content: "\f1cc";
}
.fa-life-bouy:before,
.fa-life-buoy:before,
.fa-life-saver:before,
.fa-support:before,
.fa-life-ring:before {
  content: "\f1cd";
}
.fa-circle-o-notch:before {
  content: "\f1ce";
}
.fa-ra:before,
.fa-resistance:before,
.fa-rebel:before {
  content: "\f1d0";
}
.fa-ge:before,
.fa-empire:before {
  content: "\f1d1";
}
.fa-git-square:before {
  content: "\f1d2";
}
.fa-git:before {
  content: "\f1d3";
}
.fa-y-combinator-square:before,
.fa-yc-square:before,
.fa-hacker-news:before {
  content: "\f1d4";
}
.fa-tencent-weibo:before {
  content: "\f1d5";
}
.fa-qq:before {
  content: "\f1d6";
}
.fa-wechat:before,
.fa-weixin:before {
  content: "\f1d7";
}
.fa-send:before,
.fa-paper-plane:before {
  content: "\f1d8";
}
.fa-send-o:before,
.fa-paper-plane-o:before {
  content: "\f1d9";
}
.fa-history:before {
  content: "\f1da";
}
.fa-circle-thin:before {
  content: "\f1db";
}
.fa-header:before {
  content: "\f1dc";
}
.fa-paragraph:before {
  content: "\f1dd";
}
.fa-sliders:before {
  content: "\f1de";
}
.fa-share-alt:before {
  content: "\f1e0";
}
.fa-share-alt-square:before {
  content: "\f1e1";
}
.fa-bomb:before {
  content: "\f1e2";
}
.fa-soccer-ball-o:before,
.fa-futbol-o:before {
  content: "\f1e3";
}
.fa-tty:before {
  content: "\f1e4";
}
.fa-binoculars:before {
  content: "\f1e5";
}
.fa-plug:before {
  content: "\f1e6";
}
.fa-slideshare:before {
  content: "\f1e7";
}
.fa-twitch:before {
  content: "\f1e8";
}
.fa-yelp:before {
  content: "\f1e9";
}
.fa-newspaper-o:before {
  content: "\f1ea";
}
.fa-wifi:before {
  content: "\f1eb";
}
.fa-calculator:before {
  content: "\f1ec";
}
.fa-paypal:before {
  content: "\f1ed";
}
.fa-google-wallet:before {
  content: "\f1ee";
}
.fa-cc-visa:before {
  content: "\f1f0";
}
.fa-cc-mastercard:before {
  content: "\f1f1";
}
.fa-cc-discover:before {
  content: "\f1f2";
}
.fa-cc-amex:before {
  content: "\f1f3";
}
.fa-cc-paypal:before {
  content: "\f1f4";
}
.fa-cc-stripe:before {
  content: "\f1f5";
}
.fa-bell-slash:before {
  content: "\f1f6";
}
.fa-bell-slash-o:before {
  content: "\f1f7";
}
.fa-trash:before {
  content: "\f1f8";
}
.fa-copyright:before {
  content: "\f1f9";
}
.fa-at:before {
  content: "\f1fa";
}
.fa-eyedropper:before {
  content: "\f1fb";
}
.fa-paint-brush:before {
  content: "\f1fc";
}
.fa-birthday-cake:before {
  content: "\f1fd";
}
.fa-area-chart:before {
  content: "\f1fe";
}
.fa-pie-chart:before {
  content: "\f200";
}
.fa-line-chart:before {
  content: "\f201";
}
.fa-lastfm:before {
  content: "\f202";
}
.fa-lastfm-square:before {
  content: "\f203";
}
.fa-toggle-off:before {
  content: "\f204";
}
.fa-toggle-on:before {
  content: "\f205";
}
.fa-bicycle:before {
  content: "\f206";
}
.fa-bus:before {
  content: "\f207";
}
.fa-ioxhost:before {
  content: "\f208";
}
.fa-angellist:before {
  content: "\f209";
}
.fa-cc:before {
  content: "\f20a";
}
.fa-shekel:before,
.fa-sheqel:before,
.fa-ils:before {
  content: "\f20b";
}
.fa-meanpath:before {
  content: "\f20c";
}
.fa-buysellads:before {
  content: "\f20d";
}
.fa-connectdevelop:before {
  content: "\f20e";
}
.fa-dashcube:before {
  content: "\f210";
}
.fa-forumbee:before {
  content: "\f211";
}
.fa-leanpub:before {
  content: "\f212";
}
.fa-sellsy:before {
  content: "\f213";
}
.fa-shirtsinbulk:before {
  content: "\f214";
}
.fa-simplybuilt:before {
  content: "\f215";
}
.fa-skyatlas:before {
  content: "\f216";
}
.fa-cart-plus:before {
  content: "\f217";
}
.fa-cart-arrow-down:before {
  content: "\f218";
}
.fa-diamond:before {
  content: "\f219";
}
.fa-ship:before {
  content: "\f21a";
}
.fa-user-secret:before {
  content: "\f21b";
}
.fa-motorcycle:before {
  content: "\f21c";
}
.fa-street-view:before {
  content: "\f21d";
}
.fa-heartbeat:before {
  content: "\f21e";
}
.fa-venus:before {
  content: "\f221";
}
.fa-mars:before {
  content: "\f222";
}
.fa-mercury:before {
  content: "\f223";
}
.fa-intersex:before,
.fa-transgender:before {
  content: "\f224";
}
.fa-transgender-alt:before {
  content: "\f225";
}
.fa-venus-double:before {
  content: "\f226";
}
.fa-mars-double:before {
  content: "\f227";
}
.fa-venus-mars:before {
  content: "\f228";
}
.fa-mars-stroke:before {
  content: "\f229";
}
.fa-mars-stroke-v:before {
  content: "\f22a";
}
.fa-mars-stroke-h:before {
  content: "\f22b";
}
.fa-neuter:before {
  content: "\f22c";
}
.fa-genderless:before {
  content: "\f22d";
}
.fa-facebook-official:before {
  content: "\f230";
}
.fa-pinterest-p:before {
  content: "\f231";
}
.fa-whatsapp:before {
  content: "\f232";
}
.fa-server:before {
  content: "\f233";
}
.fa-user-plus:before {
  content: "\f234";
}
.fa-user-times:before {
  content: "\f235";
}
.fa-hotel:before,
.fa-bed:before {
  content: "\f236";
}
.fa-viacoin:before {
  content: "\f237";
}
.fa-train:before {
  content: "\f238";
}
.fa-subway:before {
  content: "\f239";
}
.fa-medium:before {
  content: "\f23a";
}
.fa-yc:before,
.fa-y-combinator:before {
  content: "\f23b";
}
.fa-optin-monster:before {
  content: "\f23c";
}
.fa-opencart:before {
  content: "\f23d";
}
.fa-expeditedssl:before {
  content: "\f23e";
}
.fa-battery-4:before,
.fa-battery:before,
.fa-battery-full:before {
  content: "\f240";
}
.fa-battery-3:before,
.fa-battery-three-quarters:before {
  content: "\f241";
}
.fa-battery-2:before,
.fa-battery-half:before {
  content: "\f242";
}
.fa-battery-1:before,
.fa-battery-quarter:before {
  content: "\f243";
}
.fa-battery-0:before,
.fa-battery-empty:before {
  content: "\f244";
}
.fa-mouse-pointer:before {
  content: "\f245";
}
.fa-i-cursor:before {
  content: "\f246";
}
.fa-object-group:before {
  content: "\f247";
}
.fa-object-ungroup:before {
  content: "\f248";
}
.fa-sticky-note:before {
  content: "\f249";
}
.fa-sticky-note-o:before {
  content: "\f24a";
}
.fa-cc-jcb:before {
  content: "\f24b";
}
.fa-cc-diners-club:before {
  content: "\f24c";
}
.fa-clone:before {
  content: "\f24d";
}
.fa-balance-scale:before {
  content: "\f24e";
}
.fa-hourglass-o:before {
  content: "\f250";
}
.fa-hourglass-1:before,
.fa-hourglass-start:before {
  content: "\f251";
}
.fa-hourglass-2:before,
.fa-hourglass-half:before {
  content: "\f252";
}
.fa-hourglass-3:before,
.fa-hourglass-end:before {
  content: "\f253";
}
.fa-hourglass:before {
  content: "\f254";
}
.fa-hand-grab-o:before,
.fa-hand-rock-o:before {
  content: "\f255";
}
.fa-hand-stop-o:before,
.fa-hand-paper-o:before {
  content: "\f256";
}
.fa-hand-scissors-o:before {
  content: "\f257";
}
.fa-hand-lizard-o:before {
  content: "\f258";
}
.fa-hand-spock-o:before {
  content: "\f259";
}
.fa-hand-pointer-o:before {
  content: "\f25a";
}
.fa-hand-peace-o:before {
  content: "\f25b";
}
.fa-trademark:before {
  content: "\f25c";
}
.fa-registered:before {
  content: "\f25d";
}
.fa-creative-commons:before {
  content: "\f25e";
}
.fa-gg:before {
  content: "\f260";
}
.fa-gg-circle:before {
  content: "\f261";
}
.fa-tripadvisor:before {
  content: "\f262";
}
.fa-odnoklassniki:before {
  content: "\f263";
}
.fa-odnoklassniki-square:before {
  content: "\f264";
}
.fa-get-pocket:before {
  content: "\f265";
}
.fa-wikipedia-w:before {
  content: "\f266";
}
.fa-safari:before {
  content: "\f267";
}
.fa-chrome:before {
  content: "\f268";
}
.fa-firefox:before {
  content: "\f269";
}
.fa-opera:before {
  content: "\f26a";
}
.fa-internet-explorer:before {
  content: "\f26b";
}
.fa-tv:before,
.fa-television:before {
  content: "\f26c";
}
.fa-contao:before {
  content: "\f26d";
}
.fa-500px:before {
  content: "\f26e";
}
.fa-amazon:before {
  content: "\f270";
}
.fa-calendar-plus-o:before {
  content: "\f271";
}
.fa-calendar-minus-o:before {
  content: "\f272";
}
.fa-calendar-times-o:before {
  content: "\f273";
}
.fa-calendar-check-o:before {
  content: "\f274";
}
.fa-industry:before {
  content: "\f275";
}
.fa-map-pin:before {
  content: "\f276";
}
.fa-map-signs:before {
  content: "\f277";
}
.fa-map-o:before {
  content: "\f278";
}
.fa-map:before {
  content: "\f279";
}
.fa-commenting:before {
  content: "\f27a";
}
.fa-commenting-o:before {
  content: "\f27b";
}
.fa-houzz:before {
  content: "\f27c";
}
.fa-vimeo:before {
  content: "\f27d";
}
.fa-black-tie:before {
  content: "\f27e";
}
.fa-fonticons:before {
  content: "\f280";
}
.fa-reddit-alien:before {
  content: "\f281";
}
.fa-edge:before {
  content: "\f282";
}
.fa-credit-card-alt:before {
  content: "\f283";
}
.fa-codiepie:before {
  content: "\f284";
}
.fa-modx:before {
  content: "\f285";
}
.fa-fort-awesome:before {
  content: "\f286";
}
.fa-usb:before {
  content: "\f287";
}
.fa-product-hunt:before {
  content: "\f288";
}
.fa-mixcloud:before {
  content: "\f289";
}
.fa-scribd:before {
  content: "\f28a";
}
.fa-pause-circle:before {
  content: "\f28b";
}
.fa-pause-circle-o:before {
  content: "\f28c";
}
.fa-stop-circle:before {
  content: "\f28d";
}
.fa-stop-circle-o:before {
  content: "\f28e";
}
.fa-shopping-bag:before {
  content: "\f290";
}
.fa-shopping-basket:before {
  content: "\f291";
}
.fa-hashtag:before {
  content: "\f292";
}
.fa-bluetooth:before {
  content: "\f293";
}
.fa-bluetooth-b:before {
  content: "\f294";
}
.fa-percent:before {
  content: "\f295";
}
.fa-gitlab:before {
  content: "\f296";
}
.fa-wpbeginner:before {
  content: "\f297";
}
.fa-wpforms:before {
  content: "\f298";
}
.fa-envira:before {
  content: "\f299";
}
.fa-universal-access:before {
  content: "\f29a";
}
.fa-wheelchair-alt:before {
  content: "\f29b";
}
.fa-question-circle-o:before {
  content: "\f29c";
}
.fa-blind:before {
  content: "\f29d";
}
.fa-audio-description:before {
  content: "\f29e";
}
.fa-volume-control-phone:before {
  content: "\f2a0";
}
.fa-braille:before {
  content: "\f2a1";
}
.fa-assistive-listening-systems:before {
  content: "\f2a2";
}
.fa-asl-interpreting:before,
.fa-american-sign-language-interpreting:before {
  content: "\f2a3";
}
.fa-deafness:before,
.fa-hard-of-hearing:before,
.fa-deaf:before {
  content: "\f2a4";
}
.fa-glide:before {
  content: "\f2a5";
}
.fa-glide-g:before {
  content: "\f2a6";
}
.fa-signing:before,
.fa-sign-language:before {
  content: "\f2a7";
}
.fa-low-vision:before {
  content: "\f2a8";
}
.fa-viadeo:before {
  content: "\f2a9";
}
.fa-viadeo-square:before {
  content: "\f2aa";
}
.fa-snapchat:before {
  content: "\f2ab";
}
.fa-snapchat-ghost:before {
  content: "\f2ac";
}
.fa-snapchat-square:before {
  content: "\f2ad";
}
.fa-pied-piper:before {
  content: "\f2ae";
}
.fa-first-order:before {
  content: "\f2b0";
}
.fa-yoast:before {
  content: "\f2b1";
}
.fa-themeisle:before {
  content: "\f2b2";
}
.fa-google-plus-circle:before,
.fa-google-plus-official:before {
  content: "\f2b3";
}
.fa-fa:before,
.fa-font-awesome:before {
  content: "\f2b4";
}
.fa-handshake-o:before {
  content: "\f2b5";
}
.fa-envelope-open:before {
  content: "\f2b6";
}
.fa-envelope-open-o:before {
  content: "\f2b7";
}
.fa-linode:before {
  content: "\f2b8";
}
.fa-address-book:before {
  content: "\f2b9";
}
.fa-address-book-o:before {
  content: "\f2ba";
}
.fa-vcard:before,
.fa-address-card:before {
  content: "\f2bb";
}
.fa-vcard-o:before,
.fa-address-card-o:before {
  content: "\f2bc";
}
.fa-user-circle:before {
  content: "\f2bd";
}
.fa-user-circle-o:before {
  content: "\f2be";
}
.fa-user-o:before {
  content: "\f2c0";
}
.fa-id-badge:before {
  content: "\f2c1";
}
.fa-drivers-license:before,
.fa-id-card:before {
  content: "\f2c2";
}
.fa-drivers-license-o:before,
.fa-id-card-o:before {
  content: "\f2c3";
}
.fa-quora:before {
  content: "\f2c4";
}
.fa-free-code-camp:before {
  content: "\f2c5";
}
.fa-telegram:before {
  content: "\f2c6";
}
.fa-thermometer-4:before,
.fa-thermometer:before,
.fa-thermometer-full:before {
  content: "\f2c7";
}
.fa-thermometer-3:before,
.fa-thermometer-three-quarters:before {
  content: "\f2c8";
}
.fa-thermometer-2:before,
.fa-thermometer-half:before {
  content: "\f2c9";
}
.fa-thermometer-1:before,
.fa-thermometer-quarter:before {
  content: "\f2ca";
}
.fa-thermometer-0:before,
.fa-thermometer-empty:before {
  content: "\f2cb";
}
.fa-shower:before {
  content: "\f2cc";
}
.fa-bathtub:before,
.fa-s15:before,
.fa-bath:before {
  content: "\f2cd";
}
.fa-podcast:before {
  content: "\f2ce";
}
.fa-window-maximize:before {
  content: "\f2d0";
}
.fa-window-minimize:before {
  content: "\f2d1";
}
.fa-window-restore:before {
  content: "\f2d2";
}
.fa-times-rectangle:before,
.fa-window-close:before {
  content: "\f2d3";
}
.fa-times-rectangle-o:before,
.fa-window-close-o:before {
  content: "\f2d4";
}
.fa-bandcamp:before {
  content: "\f2d5";
}
.fa-grav:before {
  content: "\f2d6";
}
.fa-etsy:before {
  content: "\f2d7";
}
.fa-imdb:before {
  content: "\f2d8";
}
.fa-ravelry:before {
  content: "\f2d9";
}
.fa-eercast:before {
  content: "\f2da";
}
.fa-microchip:before {
  content: "\f2db";
}
.fa-snowflake-o:before {
  content: "\f2dc";
}
.fa-superpowers:before {
  content: "\f2dd";
}
.fa-wpexplorer:before {
  content: "\f2de";
}
.fa-meetup:before {
  content: "\f2e0";
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
/*!
*
* IPython base
*
*/
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
code {
  color: #000;
}
pre {
  font-size: inherit;
  line-height: inherit;
}
label {
  font-weight: normal;
}
/* Make the page background atleast 100% the height of the view port */
/* Make the page itself atleast 70% the height of the view port */
.border-box-sizing {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.corner-all {
  border-radius: 2px;
}
.no-padding {
  padding: 0px;
}
/* Flexible box model classes */
/* Taken from Alex Russell http://infrequently.org/2009/08/css-3-progress/ */
/* This file is a compatability layer.  It allows the usage of flexible box 
model layouts accross multiple browsers, including older browsers.  The newest,
universal implementation of the flexible box model is used when available (see
`Modern browsers` comments below).  Browsers that are known to implement this 
new spec completely include:

    Firefox 28.0+
    Chrome 29.0+
    Internet Explorer 11+ 
    Opera 17.0+

Browsers not listed, including Safari, are supported via the styling under the
`Old browsers` comments below.
*/
.hbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
.hbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.vbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
.vbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.hbox.reverse,
.vbox.reverse,
.reverse {
  /* Old browsers */
  -webkit-box-direction: reverse;
  -moz-box-direction: reverse;
  box-direction: reverse;
  /* Modern browsers */
  flex-direction: row-reverse;
}
.hbox.box-flex0,
.vbox.box-flex0,
.box-flex0 {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
  width: auto;
}
.hbox.box-flex1,
.vbox.box-flex1,
.box-flex1 {
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex,
.vbox.box-flex,
.box-flex {
  /* Old browsers */
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex2,
.vbox.box-flex2,
.box-flex2 {
  /* Old browsers */
  -webkit-box-flex: 2;
  -moz-box-flex: 2;
  box-flex: 2;
  /* Modern browsers */
  flex: 2;
}
.box-group1 {
  /*  Deprecated */
  -webkit-box-flex-group: 1;
  -moz-box-flex-group: 1;
  box-flex-group: 1;
}
.box-group2 {
  /* Deprecated */
  -webkit-box-flex-group: 2;
  -moz-box-flex-group: 2;
  box-flex-group: 2;
}
.hbox.start,
.vbox.start,
.start {
  /* Old browsers */
  -webkit-box-pack: start;
  -moz-box-pack: start;
  box-pack: start;
  /* Modern browsers */
  justify-content: flex-start;
}
.hbox.end,
.vbox.end,
.end {
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
}
.hbox.center,
.vbox.center,
.center {
  /* Old browsers */
  -webkit-box-pack: center;
  -moz-box-pack: center;
  box-pack: center;
  /* Modern browsers */
  justify-content: center;
}
.hbox.baseline,
.vbox.baseline,
.baseline {
  /* Old browsers */
  -webkit-box-pack: baseline;
  -moz-box-pack: baseline;
  box-pack: baseline;
  /* Modern browsers */
  justify-content: baseline;
}
.hbox.stretch,
.vbox.stretch,
.stretch {
  /* Old browsers */
  -webkit-box-pack: stretch;
  -moz-box-pack: stretch;
  box-pack: stretch;
  /* Modern browsers */
  justify-content: stretch;
}
.hbox.align-start,
.vbox.align-start,
.align-start {
  /* Old browsers */
  -webkit-box-align: start;
  -moz-box-align: start;
  box-align: start;
  /* Modern browsers */
  align-items: flex-start;
}
.hbox.align-end,
.vbox.align-end,
.align-end {
  /* Old browsers */
  -webkit-box-align: end;
  -moz-box-align: end;
  box-align: end;
  /* Modern browsers */
  align-items: flex-end;
}
.hbox.align-center,
.vbox.align-center,
.align-center {
  /* Old browsers */
  -webkit-box-align: center;
  -moz-box-align: center;
  box-align: center;
  /* Modern browsers */
  align-items: center;
}
.hbox.align-baseline,
.vbox.align-baseline,
.align-baseline {
  /* Old browsers */
  -webkit-box-align: baseline;
  -moz-box-align: baseline;
  box-align: baseline;
  /* Modern browsers */
  align-items: baseline;
}
.hbox.align-stretch,
.vbox.align-stretch,
.align-stretch {
  /* Old browsers */
  -webkit-box-align: stretch;
  -moz-box-align: stretch;
  box-align: stretch;
  /* Modern browsers */
  align-items: stretch;
}
div.error {
  margin: 2em;
  text-align: center;
}
div.error > h1 {
  font-size: 500%;
  line-height: normal;
}
div.error > p {
  font-size: 200%;
  line-height: normal;
}
div.traceback-wrapper {
  text-align: left;
  max-width: 800px;
  margin: auto;
}
div.traceback-wrapper pre.traceback {
  max-height: 600px;
  overflow: auto;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
body {
  background-color: #fff;
  /* This makes sure that the body covers the entire window and needs to
       be in a different element than the display: box in wrapper below */
  position: absolute;
  left: 0px;
  right: 0px;
  top: 0px;
  bottom: 0px;
  overflow: visible;
}
body > #header {
  /* Initially hidden to prevent FLOUC */
  display: none;
  background-color: #fff;
  /* Display over codemirror */
  position: relative;
  z-index: 100;
}
body > #header #header-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 5px;
  padding-bottom: 5px;
  padding-top: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
body > #header .header-bar {
  width: 100%;
  height: 1px;
  background: #e7e7e7;
  margin-bottom: -1px;
}
@media print {
  body > #header {
    display: none !important;
  }
}
#header-spacer {
  width: 100%;
  visibility: hidden;
}
@media print {
  #header-spacer {
    display: none;
  }
}
#ipython_notebook {
  padding-left: 0px;
  padding-top: 1px;
  padding-bottom: 1px;
}
[dir="rtl"] #ipython_notebook {
  margin-right: 10px;
  margin-left: 0;
}
[dir="rtl"] #ipython_notebook.pull-left {
  float: right !important;
  float: right;
}
.flex-spacer {
  flex: 1;
}
#noscript {
  width: auto;
  padding-top: 16px;
  padding-bottom: 16px;
  text-align: center;
  font-size: 22px;
  color: red;
  font-weight: bold;
}
#ipython_notebook img {
  height: 28px;
}
#site {
  width: 100%;
  display: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  overflow: auto;
}
@media print {
  #site {
    height: auto !important;
  }
}
/* Smaller buttons */
.ui-button .ui-button-text {
  padding: 0.2em 0.8em;
  font-size: 77%;
}
input.ui-button {
  padding: 0.3em 0.9em;
}
span#kernel_logo_widget {
  margin: 0 10px;
}
span#login_widget {
  float: right;
}
[dir="rtl"] span#login_widget {
  float: left;
}
span#login_widget > .button,
#logout {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button:focus,
#logout:focus,
span#login_widget > .button.focus,
#logout.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
span#login_widget > .button:hover,
#logout:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active:hover,
#logout:active:hover,
span#login_widget > .button.active:hover,
#logout.active:hover,
.open > .dropdown-togglespan#login_widget > .button:hover,
.open > .dropdown-toggle#logout:hover,
span#login_widget > .button:active:focus,
#logout:active:focus,
span#login_widget > .button.active:focus,
#logout.active:focus,
.open > .dropdown-togglespan#login_widget > .button:focus,
.open > .dropdown-toggle#logout:focus,
span#login_widget > .button:active.focus,
#logout:active.focus,
span#login_widget > .button.active.focus,
#logout.active.focus,
.open > .dropdown-togglespan#login_widget > .button.focus,
.open > .dropdown-toggle#logout.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  background-image: none;
}
span#login_widget > .button.disabled:hover,
#logout.disabled:hover,
span#login_widget > .button[disabled]:hover,
#logout[disabled]:hover,
fieldset[disabled] span#login_widget > .button:hover,
fieldset[disabled] #logout:hover,
span#login_widget > .button.disabled:focus,
#logout.disabled:focus,
span#login_widget > .button[disabled]:focus,
#logout[disabled]:focus,
fieldset[disabled] span#login_widget > .button:focus,
fieldset[disabled] #logout:focus,
span#login_widget > .button.disabled.focus,
#logout.disabled.focus,
span#login_widget > .button[disabled].focus,
#logout[disabled].focus,
fieldset[disabled] span#login_widget > .button.focus,
fieldset[disabled] #logout.focus {
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button .badge,
#logout .badge {
  color: #fff;
  background-color: #333;
}
.nav-header {
  text-transform: none;
}
#header > span {
  margin-top: 10px;
}
.modal_stretch .modal-dialog {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 80vh;
}
.modal_stretch .modal-dialog .modal-body {
  max-height: calc(100vh - 200px);
  overflow: auto;
  flex: 1;
}
.modal-header {
  cursor: move;
}
@media (min-width: 768px) {
  .modal .modal-dialog {
    width: 700px;
  }
}
@media (min-width: 768px) {
  select.form-control {
    margin-left: 12px;
    margin-right: 12px;
  }
}
/*!
*
* IPython auth
*
*/
.center-nav {
  display: inline-block;
  margin-bottom: -4px;
}
[dir="rtl"] .center-nav form.pull-left {
  float: right !important;
  float: right;
}
[dir="rtl"] .center-nav .navbar-text {
  float: right;
}
[dir="rtl"] .navbar-inner {
  text-align: right;
}
[dir="rtl"] div.text-left {
  text-align: right;
}
/*!
*
* IPython tree view
*
*/
/* We need an invisible input field on top of the sentense*/
/* "Drag file onto the list ..." */
.alternate_upload {
  background-color: none;
  display: inline;
}
.alternate_upload.form {
  padding: 0;
  margin: 0;
}
.alternate_upload input.fileinput {
  position: absolute;
  display: block;
  width: 100%;
  height: 100%;
  overflow: hidden;
  cursor: pointer;
  opacity: 0;
  z-index: 2;
}
.alternate_upload .btn-xs > input.fileinput {
  margin: -1px -5px;
}
.alternate_upload .btn-upload {
  position: relative;
  height: 22px;
}
::-webkit-file-upload-button {
  cursor: pointer;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
ul#tabs {
  margin-bottom: 4px;
}
ul#tabs a {
  padding-top: 6px;
  padding-bottom: 4px;
}
[dir="rtl"] ul#tabs.nav-tabs > li {
  float: right;
}
[dir="rtl"] ul#tabs.nav.nav-tabs {
  padding-right: 0;
}
ul.breadcrumb a:focus,
ul.breadcrumb a:hover {
  text-decoration: none;
}
ul.breadcrumb i.icon-home {
  font-size: 16px;
  margin-right: 4px;
}
ul.breadcrumb span {
  color: #5e5e5e;
}
.list_toolbar {
  padding: 4px 0 4px 0;
  vertical-align: middle;
}
.list_toolbar .tree-buttons {
  padding-top: 1px;
}
[dir="rtl"] .list_toolbar .tree-buttons .pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .list_toolbar .col-sm-4,
[dir="rtl"] .list_toolbar .col-sm-8 {
  float: right;
}
.dynamic-buttons {
  padding-top: 3px;
  display: inline-block;
}
.list_toolbar [class*="span"] {
  min-height: 24px;
}
.list_header {
  font-weight: bold;
  background-color: #EEE;
}
.list_placeholder {
  font-weight: bold;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
}
.list_container {
  margin-top: 4px;
  margin-bottom: 20px;
  border: 1px solid #ddd;
  border-radius: 2px;
}
.list_container > div {
  border-bottom: 1px solid #ddd;
}
.list_container > div:hover .list-item {
  background-color: red;
}
.list_container > div:last-child {
  border: none;
}
.list_item:hover .list_item {
  background-color: #ddd;
}
.list_item a {
  text-decoration: none;
}
.list_item:hover {
  background-color: #fafafa;
}
.list_header > div,
.list_item > div {
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
.list_header > div input,
.list_item > div input {
  margin-right: 7px;
  margin-left: 14px;
  vertical-align: text-bottom;
  line-height: 22px;
  position: relative;
  top: -1px;
}
.list_header > div .item_link,
.list_item > div .item_link {
  margin-left: -1px;
  vertical-align: baseline;
  line-height: 22px;
}
[dir="rtl"] .list_item > div input {
  margin-right: 0;
}
.new-file input[type=checkbox] {
  visibility: hidden;
}
.item_name {
  line-height: 22px;
  height: 24px;
}
.item_icon {
  font-size: 14px;
  color: #5e5e5e;
  margin-right: 7px;
  margin-left: 7px;
  line-height: 22px;
  vertical-align: baseline;
}
.item_modified {
  margin-right: 7px;
  margin-left: 7px;
}
[dir="rtl"] .item_modified.pull-right {
  float: left !important;
  float: left;
}
.item_buttons {
  line-height: 1em;
  margin-left: -5px;
}
.item_buttons .btn,
.item_buttons .btn-group,
.item_buttons .input-group {
  float: left;
}
.item_buttons > .btn,
.item_buttons > .btn-group,
.item_buttons > .input-group {
  margin-left: 5px;
}
.item_buttons .btn {
  min-width: 13ex;
}
.item_buttons .running-indicator {
  padding-top: 4px;
  color: #5cb85c;
}
.item_buttons .kernel-name {
  padding-top: 4px;
  color: #5bc0de;
  margin-right: 7px;
  float: left;
}
[dir="rtl"] .item_buttons.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .item_buttons .kernel-name {
  margin-left: 7px;
  float: right;
}
.toolbar_info {
  height: 24px;
  line-height: 24px;
}
.list_item input:not([type=checkbox]) {
  padding-top: 3px;
  padding-bottom: 3px;
  height: 22px;
  line-height: 14px;
  margin: 0px;
}
.highlight_text {
  color: blue;
}
#project_name {
  display: inline-block;
  padding-left: 7px;
  margin-left: -2px;
}
#project_name > .breadcrumb {
  padding: 0px;
  margin-bottom: 0px;
  background-color: transparent;
  font-weight: bold;
}
.sort_button {
  display: inline-block;
  padding-left: 7px;
}
[dir="rtl"] .sort_button.pull-right {
  float: left !important;
  float: left;
}
#tree-selector {
  padding-right: 0px;
}
#button-select-all {
  min-width: 50px;
}
[dir="rtl"] #button-select-all.btn {
  float: right ;
}
#select-all {
  margin-left: 7px;
  margin-right: 2px;
  margin-top: 2px;
  height: 16px;
}
[dir="rtl"] #select-all.pull-left {
  float: right !important;
  float: right;
}
.menu_icon {
  margin-right: 2px;
}
.tab-content .row {
  margin-left: 0px;
  margin-right: 0px;
}
.folder_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f114";
}
.folder_icon:before.fa-pull-left {
  margin-right: .3em;
}
.folder_icon:before.fa-pull-right {
  margin-left: .3em;
}
.folder_icon:before.pull-left {
  margin-right: .3em;
}
.folder_icon:before.pull-right {
  margin-left: .3em;
}
.notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
}
.notebook_icon:before.fa-pull-left {
  margin-right: .3em;
}
.notebook_icon:before.fa-pull-right {
  margin-left: .3em;
}
.notebook_icon:before.pull-left {
  margin-right: .3em;
}
.notebook_icon:before.pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
  color: #5cb85c;
}
.running_notebook_icon:before.fa-pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.fa-pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before.pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.pull-right {
  margin-left: .3em;
}
.file_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f016";
  position: relative;
  top: -2px;
}
.file_icon:before.fa-pull-left {
  margin-right: .3em;
}
.file_icon:before.fa-pull-right {
  margin-left: .3em;
}
.file_icon:before.pull-left {
  margin-right: .3em;
}
.file_icon:before.pull-right {
  margin-left: .3em;
}
#notebook_toolbar .pull-right {
  padding-top: 0px;
  margin-right: -1px;
}
ul#new-menu {
  left: auto;
  right: 0;
}
#new-menu .dropdown-header {
  font-size: 10px;
  border-bottom: 1px solid #e5e5e5;
  padding: 0 0 3px;
  margin: -3px 20px 0;
}
.kernel-menu-icon {
  padding-right: 12px;
  width: 24px;
  content: "\f096";
}
.kernel-menu-icon:before {
  content: "\f096";
}
.kernel-menu-icon-current:before {
  content: "\f00c";
}
#tab_content {
  padding-top: 20px;
}
#running .panel-group .panel {
  margin-top: 3px;
  margin-bottom: 1em;
}
#running .panel-group .panel .panel-heading {
  background-color: #EEE;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
#running .panel-group .panel .panel-heading a:focus,
#running .panel-group .panel .panel-heading a:hover {
  text-decoration: none;
}
#running .panel-group .panel .panel-body {
  padding: 0px;
}
#running .panel-group .panel .panel-body .list_container {
  margin-top: 0px;
  margin-bottom: 0px;
  border: 0px;
  border-radius: 0px;
}
#running .panel-group .panel .panel-body .list_container .list_item {
  border-bottom: 1px solid #ddd;
}
#running .panel-group .panel .panel-body .list_container .list_item:last-child {
  border-bottom: 0px;
}
.delete-button {
  display: none;
}
.duplicate-button {
  display: none;
}
.rename-button {
  display: none;
}
.move-button {
  display: none;
}
.download-button {
  display: none;
}
.shutdown-button {
  display: none;
}
.dynamic-instructions {
  display: inline-block;
  padding-top: 4px;
}
/*!
*
* IPython text editor webapp
*
*/
.selected-keymap i.fa {
  padding: 0px 5px;
}
.selected-keymap i.fa:before {
  content: "\f00c";
}
#mode-menu {
  overflow: auto;
  max-height: 20em;
}
.edit_app #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.edit_app #menubar .navbar {
  /* Use a negative 1 bottom margin, so the border overlaps the border of the
    header */
  margin-bottom: -1px;
}
.dirty-indicator {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator.pull-left {
  margin-right: .3em;
}
.dirty-indicator.pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-dirty.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty.pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-clean.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f00c";
}
.dirty-indicator-clean:before.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.pull-right {
  margin-left: .3em;
}
#filename {
  font-size: 16pt;
  display: table;
  padding: 0px 5px;
}
#current-mode {
  padding-left: 5px;
  padding-right: 5px;
}
#texteditor-backdrop {
  padding-top: 20px;
  padding-bottom: 20px;
}
@media not print {
  #texteditor-backdrop {
    background-color: #EEE;
  }
}
@media print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container {
    padding: 0px;
    background-color: #fff;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
.CodeMirror-dialog {
  background-color: #fff;
}
/*!
*
* IPython notebook
*
*/
/* CSS font colors for translated ANSI escape sequences */
/* The color values are a mix of
   http://www.xcolors.net/dl/baskerville-ivorylight and
   http://www.xcolors.net/dl/euphrasia */
.ansi-black-fg {
  color: #3E424D;
}
.ansi-black-bg {
  background-color: #3E424D;
}
.ansi-black-intense-fg {
  color: #282C36;
}
.ansi-black-intense-bg {
  background-color: #282C36;
}
.ansi-red-fg {
  color: #E75C58;
}
.ansi-red-bg {
  background-color: #E75C58;
}
.ansi-red-intense-fg {
  color: #B22B31;
}
.ansi-red-intense-bg {
  background-color: #B22B31;
}
.ansi-green-fg {
  color: #00A250;
}
.ansi-green-bg {
  background-color: #00A250;
}
.ansi-green-intense-fg {
  color: #007427;
}
.ansi-green-intense-bg {
  background-color: #007427;
}
.ansi-yellow-fg {
  color: #DDB62B;
}
.ansi-yellow-bg {
  background-color: #DDB62B;
}
.ansi-yellow-intense-fg {
  color: #B27D12;
}
.ansi-yellow-intense-bg {
  background-color: #B27D12;
}
.ansi-blue-fg {
  color: #208FFB;
}
.ansi-blue-bg {
  background-color: #208FFB;
}
.ansi-blue-intense-fg {
  color: #0065CA;
}
.ansi-blue-intense-bg {
  background-color: #0065CA;
}
.ansi-magenta-fg {
  color: #D160C4;
}
.ansi-magenta-bg {
  background-color: #D160C4;
}
.ansi-magenta-intense-fg {
  color: #A03196;
}
.ansi-magenta-intense-bg {
  background-color: #A03196;
}
.ansi-cyan-fg {
  color: #60C6C8;
}
.ansi-cyan-bg {
  background-color: #60C6C8;
}
.ansi-cyan-intense-fg {
  color: #258F8F;
}
.ansi-cyan-intense-bg {
  background-color: #258F8F;
}
.ansi-white-fg {
  color: #C5C1B4;
}
.ansi-white-bg {
  background-color: #C5C1B4;
}
.ansi-white-intense-fg {
  color: #A1A6B2;
}
.ansi-white-intense-bg {
  background-color: #A1A6B2;
}
.ansi-default-inverse-fg {
  color: #FFFFFF;
}
.ansi-default-inverse-bg {
  background-color: #000000;
}
.ansi-bold {
  font-weight: bold;
}
.ansi-underline {
  text-decoration: underline;
}
/* The following styles are deprecated an will be removed in a future version */
.ansibold {
  font-weight: bold;
}
.ansi-inverse {
  outline: 0.5px dotted;
}
/* use dark versions for foreground, to improve visibility */
.ansiblack {
  color: black;
}
.ansired {
  color: darkred;
}
.ansigreen {
  color: darkgreen;
}
.ansiyellow {
  color: #c4a000;
}
.ansiblue {
  color: darkblue;
}
.ansipurple {
  color: darkviolet;
}
.ansicyan {
  color: steelblue;
}
.ansigray {
  color: gray;
}
/* and light for background, for the same reason */
.ansibgblack {
  background-color: black;
}
.ansibgred {
  background-color: red;
}
.ansibggreen {
  background-color: green;
}
.ansibgyellow {
  background-color: yellow;
}
.ansibgblue {
  background-color: blue;
}
.ansibgpurple {
  background-color: magenta;
}
.ansibgcyan {
  background-color: cyan;
}
.ansibggray {
  background-color: gray;
}
div.cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-radius: 2px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  border-width: 1px;
  border-style: solid;
  border-color: transparent;
  width: 100%;
  padding: 5px;
  /* This acts as a spacer between cells, that is outside the border */
  margin: 0px;
  outline: none;
  position: relative;
  overflow: visible;
}
div.cell:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: transparent;
}
div.cell.jupyter-soft-selected {
  border-left-color: #E3F2FD;
  border-left-width: 1px;
  padding-left: 5px;
  border-right-color: #E3F2FD;
  border-right-width: 1px;
  background: #E3F2FD;
}
@media print {
  div.cell.jupyter-soft-selected {
    border-color: transparent;
  }
}
div.cell.selected,
div.cell.selected.jupyter-soft-selected {
  border-color: #ababab;
}
div.cell.selected:before,
div.cell.selected.jupyter-soft-selected:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: #42A5F5;
}
@media print {
  div.cell.selected,
  div.cell.selected.jupyter-soft-selected {
    border-color: transparent;
  }
}
.edit_mode div.cell.selected {
  border-color: #66BB6A;
}
.edit_mode div.cell.selected:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: #66BB6A;
}
@media print {
  .edit_mode div.cell.selected {
    border-color: transparent;
  }
}
.prompt {
  /* This needs to be wide enough for 3 digit prompt numbers: In[100]: */
  min-width: 14ex;
  /* This padding is tuned to match the padding on the CodeMirror editor. */
  padding: 0.4em;
  margin: 0px;
  font-family: monospace;
  text-align: right;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
  /* Don't highlight prompt number selection */
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  /* Use default cursor */
  cursor: default;
}
@media (max-width: 540px) {
  .prompt {
    text-align: left;
  }
}
div.inner_cell {
  min-width: 0;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_area {
  border: 1px solid #cfcfcf;
  border-radius: 2px;
  background: #f7f7f7;
  line-height: 1.21429em;
}
/* This is needed so that empty prompt areas can collapse to zero height when there
   is no content in the output_subarea and the prompt. The main purpose of this is
   to make sure that empty JavaScript output_subareas have no height. */
div.prompt:empty {
  padding-top: 0;
  padding-bottom: 0;
}
div.unrecognized_cell {
  padding: 5px 5px 5px 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.unrecognized_cell .inner_cell {
  border-radius: 2px;
  padding: 5px;
  font-weight: bold;
  color: red;
  border: 1px solid #cfcfcf;
  background: #eaeaea;
}
div.unrecognized_cell .inner_cell a {
  color: inherit;
  text-decoration: none;
}
div.unrecognized_cell .inner_cell a:hover {
  color: inherit;
  text-decoration: none;
}
@media (max-width: 540px) {
  div.unrecognized_cell > div.prompt {
    display: none;
  }
}
div.code_cell {
  /* avoid page breaking on code cells when printing */
}
@media print {
  div.code_cell {
    page-break-inside: avoid;
  }
}
/* any special styling for code cells that are currently running goes here */
div.input {
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.input {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_prompt {
  color: #303F9F;
  border-top: 1px solid transparent;
}
div.input_area > div.highlight {
  margin: 0.4em;
  border: none;
  padding: 0px;
  background-color: transparent;
}
div.input_area > div.highlight > pre {
  margin: 0px;
  border: none;
  padding: 0px;
  background-color: transparent;
}
/* The following gets added to the <head> if it is detected that the user has a
 * monospace font with inconsistent normal/bold/italic height.  See
 * notebookmain.js.  Such fonts will have keywords vertically offset with
 * respect to the rest of the text.  The user should select a better font.
 * See: https://github.com/ipython/ipython/issues/1503
 *
 * .CodeMirror span {
 *      vertical-align: bottom;
 * }
 */
.CodeMirror {
  line-height: 1.21429em;
  /* Changed from 1em to our global default */
  font-size: 14px;
  height: auto;
  /* Changed to auto to autogrow */
  background: none;
  /* Changed from white to allow our bg to show through */
}
.CodeMirror-scroll {
  /*  The CodeMirror docs are a bit fuzzy on if overflow-y should be hidden or visible.*/
  /*  We have found that if it is visible, vertical scrollbars appear with font size changes.*/
  overflow-y: hidden;
  overflow-x: auto;
}
.CodeMirror-lines {
  /* In CM2, this used to be 0.4em, but in CM3 it went to 4px. We need the em value because */
  /* we have set a different line-height and want this to scale with that. */
  /* Note that this should set vertical padding only, since CodeMirror assumes
       that horizontal padding will be set on CodeMirror pre */
  padding: 0.4em 0;
}
.CodeMirror-linenumber {
  padding: 0 8px 0 4px;
}
.CodeMirror-gutters {
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.CodeMirror pre {
  /* In CM3 this went to 4px from 0 in CM2. This sets horizontal padding only,
    use .CodeMirror-lines for vertical */
  padding: 0 0.4em;
  border: 0;
  border-radius: 0;
}
.CodeMirror-cursor {
  border-left: 1.4px solid black;
}
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .CodeMirror-cursor {
    border-left: 2px solid black;
  }
}
@media screen and (min-width: 4320px) {
  .CodeMirror-cursor {
    border-left: 4px solid black;
  }
}
/*

Original style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>
Adapted from GitHub theme

*/
.highlight-base {
  color: #000;
}
.highlight-variable {
  color: #000;
}
.highlight-variable-2 {
  color: #1a1a1a;
}
.highlight-variable-3 {
  color: #333333;
}
.highlight-string {
  color: #BA2121;
}
.highlight-comment {
  color: #408080;
  font-style: italic;
}
.highlight-number {
  color: #080;
}
.highlight-atom {
  color: #88F;
}
.highlight-keyword {
  color: #008000;
  font-weight: bold;
}
.highlight-builtin {
  color: #008000;
}
.highlight-error {
  color: #f00;
}
.highlight-operator {
  color: #AA22FF;
  font-weight: bold;
}
.highlight-meta {
  color: #AA22FF;
}
/* previously not defined, copying from default codemirror */
.highlight-def {
  color: #00f;
}
.highlight-string-2 {
  color: #f50;
}
.highlight-qualifier {
  color: #555;
}
.highlight-bracket {
  color: #997;
}
.highlight-tag {
  color: #170;
}
.highlight-attribute {
  color: #00c;
}
.highlight-header {
  color: blue;
}
.highlight-quote {
  color: #090;
}
.highlight-link {
  color: #00c;
}
/* apply the same style to codemirror */
.cm-s-ipython span.cm-keyword {
  color: #008000;
  font-weight: bold;
}
.cm-s-ipython span.cm-atom {
  color: #88F;
}
.cm-s-ipython span.cm-number {
  color: #080;
}
.cm-s-ipython span.cm-def {
  color: #00f;
}
.cm-s-ipython span.cm-variable {
  color: #000;
}
.cm-s-ipython span.cm-operator {
  color: #AA22FF;
  font-weight: bold;
}
.cm-s-ipython span.cm-variable-2 {
  color: #1a1a1a;
}
.cm-s-ipython span.cm-variable-3 {
  color: #333333;
}
.cm-s-ipython span.cm-comment {
  color: #408080;
  font-style: italic;
}
.cm-s-ipython span.cm-string {
  color: #BA2121;
}
.cm-s-ipython span.cm-string-2 {
  color: #f50;
}
.cm-s-ipython span.cm-meta {
  color: #AA22FF;
}
.cm-s-ipython span.cm-qualifier {
  color: #555;
}
.cm-s-ipython span.cm-builtin {
  color: #008000;
}
.cm-s-ipython span.cm-bracket {
  color: #997;
}
.cm-s-ipython span.cm-tag {
  color: #170;
}
.cm-s-ipython span.cm-attribute {
  color: #00c;
}
.cm-s-ipython span.cm-header {
  color: blue;
}
.cm-s-ipython span.cm-quote {
  color: #090;
}
.cm-s-ipython span.cm-link {
  color: #00c;
}
.cm-s-ipython span.cm-error {
  color: #f00;
}
.cm-s-ipython span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}
div.output_wrapper {
  /* this position must be relative to enable descendents to be absolute within it */
  position: relative;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  z-index: 1;
}
/* class for the output area when it should be height-limited */
div.output_scroll {
  /* ideally, this would be max-height, but FF barfs all over that */
  height: 24em;
  /* FF needs this *and the wrapper* to specify full width, or it will shrinkwrap */
  width: 100%;
  overflow: auto;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  display: block;
}
/* output div while it is collapsed */
div.output_collapsed {
  margin: 0px;
  padding: 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
div.out_prompt_overlay {
  height: 100%;
  padding: 0px 0.4em;
  position: absolute;
  border-radius: 2px;
}
div.out_prompt_overlay:hover {
  /* use inner shadow to get border that is computed the same on WebKit/FF */
  -webkit-box-shadow: inset 0 0 1px #000;
  box-shadow: inset 0 0 1px #000;
  background: rgba(240, 240, 240, 0.5);
}
div.output_prompt {
  color: #D84315;
}
/* This class is the outer container of all output sections. */
div.output_area {
  padding: 0px;
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.output_area .MathJax_Display {
  text-align: left !important;
}
div.output_area .rendered_html table {
  margin-left: 0;
  margin-right: 0;
}
div.output_area .rendered_html img {
  margin-left: 0;
  margin-right: 0;
}
div.output_area img,
div.output_area svg {
  max-width: 100%;
  height: auto;
}
div.output_area img.unconfined,
div.output_area svg.unconfined {
  max-width: none;
}
div.output_area .mglyph > img {
  max-width: none;
}
/* This is needed to protect the pre formating from global settings such
   as that of bootstrap */
.output {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.output_area {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
div.output_area pre {
  margin: 0;
  padding: 1px 0 1px 0;
  border: 0;
  vertical-align: baseline;
  color: black;
  background-color: transparent;
  border-radius: 0;
}
/* This class is for the output subarea inside the output_area and after
   the prompt div. */
div.output_subarea {
  overflow-x: auto;
  padding: 0.4em;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
  max-width: calc(100% - 14ex);
}
div.output_scroll div.output_subarea {
  overflow-x: visible;
}
/* The rest of the output_* classes are for special styling of the different
   output types */
/* all text output has this class: */
div.output_text {
  text-align: left;
  color: #000;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
}
/* stdout/stderr are 'text' as well as 'stream', but execute_result/error are *not* streams */
div.output_stderr {
  background: #fdd;
  /* very light red background for stderr */
}
div.output_latex {
  text-align: left;
}
/* Empty output_javascript divs should have no height */
div.output_javascript:empty {
  padding: 0;
}
.js-error {
  color: darkred;
}
/* raw_input styles */
div.raw_input_container {
  line-height: 1.21429em;
  padding-top: 5px;
}
pre.raw_input_prompt {
  /* nothing needed here. */
}
input.raw_input {
  font-family: monospace;
  font-size: inherit;
  color: inherit;
  width: auto;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
}
input.raw_input:focus {
  box-shadow: none;
}
p.p-space {
  margin-bottom: 10px;
}
div.output_unrecognized {
  padding: 5px;
  font-weight: bold;
  color: red;
}
div.output_unrecognized a {
  color: inherit;
  text-decoration: none;
}
div.output_unrecognized a:hover {
  color: inherit;
  text-decoration: none;
}
.rendered_html {
  color: #000;
  /* any extras will just be numbers: */
}
.rendered_html em {
  font-style: italic;
}
.rendered_html strong {
  font-weight: bold;
}
.rendered_html u {
  text-decoration: underline;
}
.rendered_html :link {
  text-decoration: underline;
}
.rendered_html :visited {
  text-decoration: underline;
}
.rendered_html h1 {
  font-size: 185.7%;
  margin: 1.08em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h2 {
  font-size: 157.1%;
  margin: 1.27em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h3 {
  font-size: 128.6%;
  margin: 1.55em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h4 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h5 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h6 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h1:first-child {
  margin-top: 0.538em;
}
.rendered_html h2:first-child {
  margin-top: 0.636em;
}
.rendered_html h3:first-child {
  margin-top: 0.777em;
}
.rendered_html h4:first-child {
  margin-top: 1em;
}
.rendered_html h5:first-child {
  margin-top: 1em;
}
.rendered_html h6:first-child {
  margin-top: 1em;
}
.rendered_html ul:not(.list-inline),
.rendered_html ol:not(.list-inline) {
  padding-left: 2em;
}
.rendered_html ul {
  list-style: disc;
}
.rendered_html ul ul {
  list-style: square;
  margin-top: 0;
}
.rendered_html ul ul ul {
  list-style: circle;
}
.rendered_html ol {
  list-style: decimal;
}
.rendered_html ol ol {
  list-style: upper-alpha;
  margin-top: 0;
}
.rendered_html ol ol ol {
  list-style: lower-alpha;
}
.rendered_html ol ol ol ol {
  list-style: lower-roman;
}
.rendered_html ol ol ol ol ol {
  list-style: decimal;
}
.rendered_html * + ul {
  margin-top: 1em;
}
.rendered_html * + ol {
  margin-top: 1em;
}
.rendered_html hr {
  color: black;
  background-color: black;
}
.rendered_html pre {
  margin: 1em 2em;
  padding: 0px;
  background-color: #fff;
}
.rendered_html code {
  background-color: #eff0f1;
}
.rendered_html p code {
  padding: 1px 5px;
}
.rendered_html pre code {
  background-color: #fff;
}
.rendered_html pre,
.rendered_html code {
  border: 0;
  color: #000;
  font-size: 100%;
}
.rendered_html blockquote {
  margin: 1em 2em;
}
.rendered_html table {
  margin-left: auto;
  margin-right: auto;
  border: none;
  border-collapse: collapse;
  border-spacing: 0;
  color: black;
  font-size: 12px;
  table-layout: fixed;
}
.rendered_html thead {
  border-bottom: 1px solid black;
  vertical-align: bottom;
}
.rendered_html tr,
.rendered_html th,
.rendered_html td {
  text-align: right;
  vertical-align: middle;
  padding: 0.5em 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}
.rendered_html th {
  font-weight: bold;
}
.rendered_html tbody tr:nth-child(odd) {
  background: #f5f5f5;
}
.rendered_html tbody tr:hover {
  background: rgba(66, 165, 245, 0.2);
}
.rendered_html * + table {
  margin-top: 1em;
}
.rendered_html p {
  text-align: left;
}
.rendered_html * + p {
  margin-top: 1em;
}
.rendered_html img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.rendered_html * + img {
  margin-top: 1em;
}
.rendered_html img,
.rendered_html svg {
  max-width: 100%;
  height: auto;
}
.rendered_html img.unconfined,
.rendered_html svg.unconfined {
  max-width: none;
}
.rendered_html .alert {
  margin-bottom: initial;
}
.rendered_html * + .alert {
  margin-top: 1em;
}
[dir="rtl"] .rendered_html p {
  text-align: right;
}
div.text_cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.text_cell > div.prompt {
    display: none;
  }
}
div.text_cell_render {
  /*font-family: "Helvetica Neue", Arial, Helvetica, Geneva, sans-serif;*/
  outline: none;
  resize: none;
  width: inherit;
  border-style: none;
  padding: 0.5em 0.5em 0.5em 0.4em;
  color: #000;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
a.anchor-link:link {
  text-decoration: none;
  padding: 0px 20px;
  visibility: hidden;
}
h1:hover .anchor-link,
h2:hover .anchor-link,
h3:hover .anchor-link,
h4:hover .anchor-link,
h5:hover .anchor-link,
h6:hover .anchor-link {
  visibility: visible;
}
.text_cell.rendered .input_area {
  display: none;
}
.text_cell.rendered .rendered_html {
  overflow-x: auto;
  overflow-y: hidden;
}
.text_cell.rendered .rendered_html tr,
.text_cell.rendered .rendered_html th,
.text_cell.rendered .rendered_html td {
  max-width: none;
}
.text_cell.unrendered .text_cell_render {
  display: none;
}
.text_cell .dropzone .input_area {
  border: 2px dashed #bababa;
  margin: -1px;
}
.cm-header-1,
.cm-header-2,
.cm-header-3,
.cm-header-4,
.cm-header-5,
.cm-header-6 {
  font-weight: bold;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
.cm-header-1 {
  font-size: 185.7%;
}
.cm-header-2 {
  font-size: 157.1%;
}
.cm-header-3 {
  font-size: 128.6%;
}
.cm-header-4 {
  font-size: 110%;
}
.cm-header-5 {
  font-size: 100%;
  font-style: italic;
}
.cm-header-6 {
  font-size: 100%;
  font-style: italic;
}
/*!
*
* IPython notebook webapp
*
*/
@media (max-width: 767px) {
  .notebook_app {
    padding-left: 0px;
    padding-right: 0px;
  }
}
#ipython-main-app {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook_panel {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook {
  font-size: 14px;
  line-height: 20px;
  overflow-y: hidden;
  overflow-x: auto;
  width: 100%;
  /* This spaces the page away from the edge of the notebook area */
  padding-top: 20px;
  margin: 0px;
  outline: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  min-height: 100%;
}
@media not print {
  #notebook-container {
    padding: 15px;
    background-color: #fff;
    min-height: 0;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
@media print {
  #notebook-container {
    width: 100%;
  }
}
div.ui-widget-content {
  border: 1px solid #ababab;
  outline: none;
}
pre.dialog {
  background-color: #f7f7f7;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0.4em;
  padding-left: 2em;
}
p.dialog {
  padding: 0.2em;
}
/* Word-wrap output correctly.  This is the CSS3 spelling, though Firefox seems
   to not honor it correctly.  Webkit browsers (Chrome, rekonq, Safari) do.
 */
pre,
code,
kbd,
samp {
  white-space: pre-wrap;
}
#fonttest {
  font-family: monospace;
}
p {
  margin-bottom: 0;
}
.end_space {
  min-height: 100px;
  transition: height .2s ease;
}
.notebook_app > #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
@media not print {
  .notebook_app {
    background-color: #EEE;
  }
}
kbd {
  border-style: solid;
  border-width: 1px;
  box-shadow: none;
  margin: 2px;
  padding-left: 2px;
  padding-right: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
.jupyter-keybindings {
  padding: 1px;
  line-height: 24px;
  border-bottom: 1px solid gray;
}
.jupyter-keybindings input {
  margin: 0;
  padding: 0;
  border: none;
}
.jupyter-keybindings i {
  padding: 6px;
}
.well code {
  background-color: #ffffff;
  border-color: #ababab;
  border-width: 1px;
  border-style: solid;
  padding: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
/* CSS for the cell toolbar */
.celltoolbar {
  border: thin solid #CFCFCF;
  border-bottom: none;
  background: #EEE;
  border-radius: 2px 2px 0px 0px;
  width: 100%;
  height: 29px;
  padding-right: 4px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
  display: -webkit-flex;
}
@media print {
  .celltoolbar {
    display: none;
  }
}
.ctb_hideshow {
  display: none;
  vertical-align: bottom;
}
/* ctb_show is added to the ctb_hideshow div to show the cell toolbar.
   Cell toolbars are only shown when the ctb_global_show class is also set.
*/
.ctb_global_show .ctb_show.ctb_hideshow {
  display: block;
}
.ctb_global_show .ctb_show + .input_area,
.ctb_global_show .ctb_show + div.text_cell_input,
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border: 1px solid #cfcfcf;
}
.celltoolbar {
  font-size: 87%;
  padding-top: 3px;
}
.celltoolbar select {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  width: inherit;
  font-size: inherit;
  height: 22px;
  padding: 0px;
  display: inline-block;
}
.celltoolbar select:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.celltoolbar select::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.celltoolbar select:-ms-input-placeholder {
  color: #999;
}
.celltoolbar select::-webkit-input-placeholder {
  color: #999;
}
.celltoolbar select::-ms-expand {
  border: 0;
  background-color: transparent;
}
.celltoolbar select[disabled],
.celltoolbar select[readonly],
fieldset[disabled] .celltoolbar select {
  background-color: #eeeeee;
  opacity: 1;
}
.celltoolbar select[disabled],
fieldset[disabled] .celltoolbar select {
  cursor: not-allowed;
}
textarea.celltoolbar select {
  height: auto;
}
select.celltoolbar select {
  height: 30px;
  line-height: 30px;
}
textarea.celltoolbar select,
select[multiple].celltoolbar select {
  height: auto;
}
.celltoolbar label {
  margin-left: 5px;
  margin-right: 5px;
}
.tags_button_container {
  width: 100%;
  display: flex;
}
.tag-container {
  display: flex;
  flex-direction: row;
  flex-grow: 1;
  overflow: hidden;
  position: relative;
}
.tag-container > * {
  margin: 0 4px;
}
.remove-tag-btn {
  margin-left: 4px;
}
.tags-input {
  display: flex;
}
.cell-tag:last-child:after {
  content: "";
  position: absolute;
  right: 0;
  width: 40px;
  height: 100%;
  /* Fade to background color of cell toolbar */
  background: linear-gradient(to right, rgba(0, 0, 0, 0), #EEE);
}
.tags-input > * {
  margin-left: 4px;
}
.cell-tag,
.tags-input input,
.tags-input button {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  box-shadow: none;
  width: inherit;
  font-size: inherit;
  height: 22px;
  line-height: 22px;
  padding: 0px 4px;
  display: inline-block;
}
.cell-tag:focus,
.tags-input input:focus,
.tags-input button:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.cell-tag::-moz-placeholder,
.tags-input input::-moz-placeholder,
.tags-input button::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.cell-tag:-ms-input-placeholder,
.tags-input input:-ms-input-placeholder,
.tags-input button:-ms-input-placeholder {
  color: #999;
}
.cell-tag::-webkit-input-placeholder,
.tags-input input::-webkit-input-placeholder,
.tags-input button::-webkit-input-placeholder {
  color: #999;
}
.cell-tag::-ms-expand,
.tags-input input::-ms-expand,
.tags-input button::-ms-expand {
  border: 0;
  background-color: transparent;
}
.cell-tag[disabled],
.tags-input input[disabled],
.tags-input button[disabled],
.cell-tag[readonly],
.tags-input input[readonly],
.tags-input button[readonly],
fieldset[disabled] .cell-tag,
fieldset[disabled] .tags-input input,
fieldset[disabled] .tags-input button {
  background-color: #eeeeee;
  opacity: 1;
}
.cell-tag[disabled],
.tags-input input[disabled],
.tags-input button[disabled],
fieldset[disabled] .cell-tag,
fieldset[disabled] .tags-input input,
fieldset[disabled] .tags-input button {
  cursor: not-allowed;
}
textarea.cell-tag,
textarea.tags-input input,
textarea.tags-input button {
  height: auto;
}
select.cell-tag,
select.tags-input input,
select.tags-input button {
  height: 30px;
  line-height: 30px;
}
textarea.cell-tag,
textarea.tags-input input,
textarea.tags-input button,
select[multiple].cell-tag,
select[multiple].tags-input input,
select[multiple].tags-input button {
  height: auto;
}
.cell-tag,
.tags-input button {
  padding: 0px 4px;
}
.cell-tag {
  background-color: #fff;
  white-space: nowrap;
}
.tags-input input[type=text]:focus {
  outline: none;
  box-shadow: none;
  border-color: #ccc;
}
.completions {
  position: absolute;
  z-index: 110;
  overflow: hidden;
  border: 1px solid #ababab;
  border-radius: 2px;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  line-height: 1;
}
.completions select {
  background: white;
  outline: none;
  border: none;
  padding: 0px;
  margin: 0px;
  overflow: auto;
  font-family: monospace;
  font-size: 110%;
  color: #000;
  width: auto;
}
.completions select option.context {
  color: #286090;
}
#kernel_logo_widget .current_kernel_logo {
  display: none;
  margin-top: -1px;
  margin-bottom: -1px;
  width: 32px;
  height: 32px;
}
[dir="rtl"] #kernel_logo_widget {
  float: left !important;
  float: left;
}
.modal .modal-body .move-path {
  display: flex;
  flex-direction: row;
  justify-content: space;
  align-items: center;
}
.modal .modal-body .move-path .server-root {
  padding-right: 20px;
}
.modal .modal-body .move-path .path-input {
  flex: 1;
}
#menubar {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  margin-top: 1px;
}
#menubar .navbar {
  border-top: 1px;
  border-radius: 0px 0px 2px 2px;
  margin-bottom: 0px;
}
#menubar .navbar-toggle {
  float: left;
  padding-top: 7px;
  padding-bottom: 7px;
  border: none;
}
#menubar .navbar-collapse {
  clear: left;
}
[dir="rtl"] #menubar .navbar-toggle {
  float: right;
}
[dir="rtl"] #menubar .navbar-collapse {
  clear: right;
}
[dir="rtl"] #menubar .navbar-nav {
  float: right;
}
[dir="rtl"] #menubar .nav {
  padding-right: 0px;
}
[dir="rtl"] #menubar .navbar-nav > li {
  float: right;
}
[dir="rtl"] #menubar .navbar-right {
  float: left !important;
}
[dir="rtl"] ul.dropdown-menu {
  text-align: right;
  left: auto;
}
[dir="rtl"] ul#new-menu.dropdown-menu {
  right: auto;
  left: 0;
}
.nav-wrapper {
  border-bottom: 1px solid #e7e7e7;
}
i.menu-icon {
  padding-top: 4px;
}
[dir="rtl"] i.menu-icon.pull-right {
  float: left !important;
  float: left;
}
ul#help_menu li a {
  overflow: hidden;
  padding-right: 2.2em;
}
ul#help_menu li a i {
  margin-right: -1.2em;
}
[dir="rtl"] ul#help_menu li a {
  padding-left: 2.2em;
}
[dir="rtl"] ul#help_menu li a i {
  margin-right: 0;
  margin-left: -1.2em;
}
[dir="rtl"] ul#help_menu li a i.pull-right {
  float: left !important;
  float: left;
}
.dropdown-submenu {
  position: relative;
}
.dropdown-submenu > .dropdown-menu {
  top: 0;
  left: 100%;
  margin-top: -6px;
  margin-left: -1px;
}
[dir="rtl"] .dropdown-submenu > .dropdown-menu {
  right: 100%;
  margin-right: -1px;
}
.dropdown-submenu:hover > .dropdown-menu {
  display: block;
}
.dropdown-submenu > a:after {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: block;
  content: "\f0da";
  float: right;
  color: #333333;
  margin-top: 2px;
  margin-right: -10px;
}
.dropdown-submenu > a:after.fa-pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.fa-pull-right {
  margin-left: .3em;
}
.dropdown-submenu > a:after.pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.pull-right {
  margin-left: .3em;
}
[dir="rtl"] .dropdown-submenu > a:after {
  float: left;
  content: "\f0d9";
  margin-right: 0;
  margin-left: -10px;
}
.dropdown-submenu:hover > a:after {
  color: #262626;
}
.dropdown-submenu.pull-left {
  float: none;
}
.dropdown-submenu.pull-left > .dropdown-menu {
  left: -100%;
  margin-left: 10px;
}
#notification_area {
  float: right !important;
  float: right;
  z-index: 10;
}
[dir="rtl"] #notification_area {
  float: left !important;
  float: left;
}
.indicator_area {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
[dir="rtl"] .indicator_area {
  float: left !important;
  float: left;
}
#kernel_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  border-left: 1px solid;
}
#kernel_indicator .kernel_indicator_name {
  padding-left: 5px;
  padding-right: 5px;
}
[dir="rtl"] #kernel_indicator {
  float: left !important;
  float: left;
  border-left: 0;
  border-right: 1px solid;
}
#modal_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
[dir="rtl"] #modal_indicator {
  float: left !important;
  float: left;
}
#readonly-indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  margin-top: 2px;
  margin-bottom: 0px;
  margin-left: 0px;
  margin-right: 0px;
  display: none;
}
.modal_indicator:before {
  width: 1.28571429em;
  text-align: center;
}
.edit_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f040";
}
.edit_mode .modal_indicator:before.fa-pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.fa-pull-right {
  margin-left: .3em;
}
.edit_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: ' ';
}
.command_mode .modal_indicator:before.fa-pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.fa-pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f10c";
}
.kernel_idle_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f111";
}
.kernel_busy_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f1e2";
}
.kernel_dead_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f127";
}
.kernel_disconnected_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.pull-right {
  margin-left: .3em;
}
.notification_widget {
  color: #777;
  z-index: 10;
  background: rgba(240, 240, 240, 0.5);
  margin-right: 4px;
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget:focus,
.notification_widget.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.notification_widget:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active:hover,
.notification_widget.active:hover,
.open > .dropdown-toggle.notification_widget:hover,
.notification_widget:active:focus,
.notification_widget.active:focus,
.open > .dropdown-toggle.notification_widget:focus,
.notification_widget:active.focus,
.notification_widget.active.focus,
.open > .dropdown-toggle.notification_widget.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  background-image: none;
}
.notification_widget.disabled:hover,
.notification_widget[disabled]:hover,
fieldset[disabled] .notification_widget:hover,
.notification_widget.disabled:focus,
.notification_widget[disabled]:focus,
fieldset[disabled] .notification_widget:focus,
.notification_widget.disabled.focus,
.notification_widget[disabled].focus,
fieldset[disabled] .notification_widget.focus {
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget .badge {
  color: #fff;
  background-color: #333;
}
.notification_widget.warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning:focus,
.notification_widget.warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.notification_widget.warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active:hover,
.notification_widget.warning.active:hover,
.open > .dropdown-toggle.notification_widget.warning:hover,
.notification_widget.warning:active:focus,
.notification_widget.warning.active:focus,
.open > .dropdown-toggle.notification_widget.warning:focus,
.notification_widget.warning:active.focus,
.notification_widget.warning.active.focus,
.open > .dropdown-toggle.notification_widget.warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  background-image: none;
}
.notification_widget.warning.disabled:hover,
.notification_widget.warning[disabled]:hover,
fieldset[disabled] .notification_widget.warning:hover,
.notification_widget.warning.disabled:focus,
.notification_widget.warning[disabled]:focus,
fieldset[disabled] .notification_widget.warning:focus,
.notification_widget.warning.disabled.focus,
.notification_widget.warning[disabled].focus,
fieldset[disabled] .notification_widget.warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.notification_widget.success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success:focus,
.notification_widget.success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.notification_widget.success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active:hover,
.notification_widget.success.active:hover,
.open > .dropdown-toggle.notification_widget.success:hover,
.notification_widget.success:active:focus,
.notification_widget.success.active:focus,
.open > .dropdown-toggle.notification_widget.success:focus,
.notification_widget.success:active.focus,
.notification_widget.success.active.focus,
.open > .dropdown-toggle.notification_widget.success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  background-image: none;
}
.notification_widget.success.disabled:hover,
.notification_widget.success[disabled]:hover,
fieldset[disabled] .notification_widget.success:hover,
.notification_widget.success.disabled:focus,
.notification_widget.success[disabled]:focus,
fieldset[disabled] .notification_widget.success:focus,
.notification_widget.success.disabled.focus,
.notification_widget.success[disabled].focus,
fieldset[disabled] .notification_widget.success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.notification_widget.info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info:focus,
.notification_widget.info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.notification_widget.info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active:hover,
.notification_widget.info.active:hover,
.open > .dropdown-toggle.notification_widget.info:hover,
.notification_widget.info:active:focus,
.notification_widget.info.active:focus,
.open > .dropdown-toggle.notification_widget.info:focus,
.notification_widget.info:active.focus,
.notification_widget.info.active.focus,
.open > .dropdown-toggle.notification_widget.info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  background-image: none;
}
.notification_widget.info.disabled:hover,
.notification_widget.info[disabled]:hover,
fieldset[disabled] .notification_widget.info:hover,
.notification_widget.info.disabled:focus,
.notification_widget.info[disabled]:focus,
fieldset[disabled] .notification_widget.info:focus,
.notification_widget.info.disabled.focus,
.notification_widget.info[disabled].focus,
fieldset[disabled] .notification_widget.info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.notification_widget.danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger:focus,
.notification_widget.danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.notification_widget.danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active:hover,
.notification_widget.danger.active:hover,
.open > .dropdown-toggle.notification_widget.danger:hover,
.notification_widget.danger:active:focus,
.notification_widget.danger.active:focus,
.open > .dropdown-toggle.notification_widget.danger:focus,
.notification_widget.danger:active.focus,
.notification_widget.danger.active.focus,
.open > .dropdown-toggle.notification_widget.danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  background-image: none;
}
.notification_widget.danger.disabled:hover,
.notification_widget.danger[disabled]:hover,
fieldset[disabled] .notification_widget.danger:hover,
.notification_widget.danger.disabled:focus,
.notification_widget.danger[disabled]:focus,
fieldset[disabled] .notification_widget.danger:focus,
.notification_widget.danger.disabled.focus,
.notification_widget.danger[disabled].focus,
fieldset[disabled] .notification_widget.danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger .badge {
  color: #d9534f;
  background-color: #fff;
}
div#pager {
  background-color: #fff;
  font-size: 14px;
  line-height: 20px;
  overflow: hidden;
  display: none;
  position: fixed;
  bottom: 0px;
  width: 100%;
  max-height: 50%;
  padding-top: 8px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  /* Display over codemirror */
  z-index: 100;
  /* Hack which prevents jquery ui resizable from changing top. */
  top: auto !important;
}
div#pager pre {
  line-height: 1.21429em;
  color: #000;
  background-color: #f7f7f7;
  padding: 0.4em;
}
div#pager #pager-button-area {
  position: absolute;
  top: 8px;
  right: 20px;
}
div#pager #pager-contents {
  position: relative;
  overflow: auto;
  width: 100%;
  height: 100%;
}
div#pager #pager-contents #pager-container {
  position: relative;
  padding: 15px 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
div#pager .ui-resizable-handle {
  top: 0px;
  height: 8px;
  background: #f7f7f7;
  border-top: 1px solid #cfcfcf;
  border-bottom: 1px solid #cfcfcf;
  /* This injects handle bars (a short, wide = symbol) for 
        the resize handle. */
}
div#pager .ui-resizable-handle::after {
  content: '';
  top: 2px;
  left: 50%;
  height: 3px;
  width: 30px;
  margin-left: -15px;
  position: absolute;
  border-top: 1px solid #cfcfcf;
}
.quickhelp {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  line-height: 1.8em;
}
.shortcut_key {
  display: inline-block;
  width: 21ex;
  text-align: right;
  font-family: monospace;
}
.shortcut_descr {
  display: inline-block;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
span.save_widget {
  height: 30px;
  margin-top: 4px;
  display: flex;
  justify-content: flex-start;
  align-items: baseline;
  width: 50%;
  flex: 1;
}
span.save_widget span.filename {
  height: 100%;
  line-height: 1em;
  margin-left: 16px;
  border: none;
  font-size: 146.5%;
  text-overflow: ellipsis;
  overflow: hidden;
  white-space: nowrap;
  border-radius: 2px;
}
span.save_widget span.filename:hover {
  background-color: #e6e6e6;
}
[dir="rtl"] span.save_widget.pull-left {
  float: right !important;
  float: right;
}
[dir="rtl"] span.save_widget span.filename {
  margin-left: 0;
  margin-right: 16px;
}
span.checkpoint_status,
span.autosave_status {
  font-size: small;
  white-space: nowrap;
  padding: 0 5px;
}
@media (max-width: 767px) {
  span.save_widget {
    font-size: small;
    padding: 0 0 0 5px;
  }
  span.checkpoint_status,
  span.autosave_status {
    display: none;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  span.checkpoint_status {
    display: none;
  }
  span.autosave_status {
    font-size: x-small;
  }
}
.toolbar {
  padding: 0px;
  margin-left: -5px;
  margin-top: 2px;
  margin-bottom: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.toolbar select,
.toolbar label {
  width: auto;
  vertical-align: middle;
  margin-right: 2px;
  margin-bottom: 0px;
  display: inline;
  font-size: 92%;
  margin-left: 0.3em;
  margin-right: 0.3em;
  padding: 0px;
  padding-top: 3px;
}
.toolbar .btn {
  padding: 2px 8px;
}
.toolbar .btn-group {
  margin-top: 0px;
  margin-left: 5px;
}
.toolbar-btn-label {
  margin-left: 6px;
}
#maintoolbar {
  margin-bottom: -3px;
  margin-top: -8px;
  border: 0px;
  min-height: 27px;
  margin-left: 0px;
  padding-top: 11px;
  padding-bottom: 3px;
}
#maintoolbar .navbar-text {
  float: none;
  vertical-align: middle;
  text-align: right;
  margin-left: 5px;
  margin-right: 0px;
  margin-top: 0px;
}
.select-xs {
  height: 24px;
}
[dir="rtl"] .btn-group > .btn,
.btn-group-vertical > .btn {
  float: right;
}
.pulse,
.dropdown-menu > li > a.pulse,
li.pulse > a.dropdown-toggle,
li.pulse.open > a.dropdown-toggle {
  background-color: #F37626;
  color: white;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
/** WARNING IF YOU ARE EDITTING THIS FILE, if this is a .css file, It has a lot
 * of chance of beeing generated from the ../less/[samename].less file, you can
 * try to get back the less file by reverting somme commit in history
 **/
/*
 * We'll try to get something pretty, so we
 * have some strange css to have the scroll bar on
 * the left with fix button on the top right of the tooltip
 */
@-moz-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-webkit-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
/*properties of tooltip after "expand"*/
.bigtooltip {
  overflow: auto;
  height: 200px;
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
}
/*properties of tooltip before "expand"*/
.smalltooltip {
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
  text-overflow: ellipsis;
  overflow: hidden;
  height: 80px;
}
.tooltipbuttons {
  position: absolute;
  padding-right: 15px;
  top: 0px;
  right: 0px;
}
.tooltiptext {
  /*avoid the button to overlap on some docstring*/
  padding-right: 30px;
}
.ipython_tooltip {
  max-width: 700px;
  /*fade-in animation when inserted*/
  -webkit-animation: fadeOut 400ms;
  -moz-animation: fadeOut 400ms;
  animation: fadeOut 400ms;
  -webkit-animation: fadeIn 400ms;
  -moz-animation: fadeIn 400ms;
  animation: fadeIn 400ms;
  vertical-align: middle;
  background-color: #f7f7f7;
  overflow: visible;
  border: #ababab 1px solid;
  outline: none;
  padding: 3px;
  margin: 0px;
  padding-left: 7px;
  font-family: monospace;
  min-height: 50px;
  -moz-box-shadow: 0px 6px 10px -1px #adadad;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  border-radius: 2px;
  position: absolute;
  z-index: 1000;
}
.ipython_tooltip a {
  float: right;
}
.ipython_tooltip .tooltiptext pre {
  border: 0;
  border-radius: 0;
  font-size: 100%;
  background-color: #f7f7f7;
}
.pretooltiparrow {
  left: 0px;
  margin: 0px;
  top: -16px;
  width: 40px;
  height: 16px;
  overflow: hidden;
  position: absolute;
}
.pretooltiparrow:before {
  background-color: #f7f7f7;
  border: 1px #ababab solid;
  z-index: 11;
  content: "";
  position: absolute;
  left: 15px;
  top: 10px;
  width: 25px;
  height: 25px;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -o-transform: rotate(45deg);
}
ul.typeahead-list i {
  margin-left: -10px;
  width: 18px;
}
[dir="rtl"] ul.typeahead-list i {
  margin-left: 0;
  margin-right: -10px;
}
ul.typeahead-list {
  max-height: 80vh;
  overflow: auto;
}
ul.typeahead-list > li > a {
  /** Firefox bug **/
  /* see https://github.com/jupyter/notebook/issues/559 */
  white-space: normal;
}
ul.typeahead-list  > li > a.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .typeahead-list {
  text-align: right;
}
.cmd-palette .modal-body {
  padding: 7px;
}
.cmd-palette form {
  background: white;
}
.cmd-palette input {
  outline: none;
}
.no-shortcut {
  min-width: 20px;
  color: transparent;
}
[dir="rtl"] .no-shortcut.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .command-shortcut.pull-right {
  float: left !important;
  float: left;
}
.command-shortcut:before {
  content: "(command mode)";
  padding-right: 3px;
  color: #777777;
}
.edit-shortcut:before {
  content: "(edit)";
  padding-right: 3px;
  color: #777777;
}
[dir="rtl"] .edit-shortcut.pull-right {
  float: left !important;
  float: left;
}
#find-and-replace #replace-preview .match,
#find-and-replace #replace-preview .insert {
  background-color: #BBDEFB;
  border-color: #90CAF9;
  border-style: solid;
  border-width: 1px;
  border-radius: 0px;
}
[dir="ltr"] #find-and-replace .input-group-btn + .form-control {
  border-left: none;
}
[dir="rtl"] #find-and-replace .input-group-btn + .form-control {
  border-right: none;
}
#find-and-replace #replace-preview .replace .match {
  background-color: #FFCDD2;
  border-color: #EF9A9A;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .insert {
  background-color: #C8E6C9;
  border-color: #A5D6A7;
  border-radius: 0px;
}
#find-and-replace #replace-preview {
  max-height: 60vh;
  overflow: auto;
}
#find-and-replace #replace-preview pre {
  padding: 5px 10px;
}
.terminal-app {
  background: #EEE;
}
.terminal-app #header {
  background: #fff;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.terminal-app .terminal {
  width: 100%;
  float: left;
  font-family: monospace;
  color: white;
  background: black;
  padding: 0.4em;
  border-radius: 2px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
}
.terminal-app .terminal,
.terminal-app .terminal dummy-screen {
  line-height: 1em;
  font-size: 14px;
}
.terminal-app .terminal .xterm-rows {
  padding: 10px;
}
.terminal-app .terminal-cursor {
  color: black;
  background: white;
}
.terminal-app #terminado-container {
  margin-top: 20px;
}
/*# sourceMappingURL=style.min.css.map */
    </style>
<style type="text/css">
    .highlight .hll { background-color: #ffffcc }
.highlight  { background: #f8f8f8; }
.highlight .c { color: #408080; font-style: italic } /* Comment */
.highlight .err { border: 1px solid #FF0000 } /* Error */
.highlight .k { color: #008000; font-weight: bold } /* Keyword */
.highlight .o { color: #666666 } /* Operator */
.highlight .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: #408080; font-style: italic } /* Comment.Multiline */
.highlight .cp { color: #BC7A00 } /* Comment.Preproc */
.highlight .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: #408080; font-style: italic } /* Comment.Single */
.highlight .cs { color: #408080; font-style: italic } /* Comment.Special */
.highlight .gd { color: #A00000 } /* Generic.Deleted */
.highlight .ge { font-style: italic } /* Generic.Emph */
.highlight .gr { color: #FF0000 } /* Generic.Error */
.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
.highlight .gi { color: #00A000 } /* Generic.Inserted */
.highlight .go { color: #888888 } /* Generic.Output */
.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
.highlight .gs { font-weight: bold } /* Generic.Strong */
.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
.highlight .gt { color: #0044DD } /* Generic.Traceback */
.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: #008000 } /* Keyword.Pseudo */
.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: #B00040 } /* Keyword.Type */
.highlight .m { color: #666666 } /* Literal.Number */
.highlight .s { color: #BA2121 } /* Literal.String */
.highlight .na { color: #7D9029 } /* Name.Attribute */
.highlight .nb { color: #008000 } /* Name.Builtin */
.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
.highlight .no { color: #880000 } /* Name.Constant */
.highlight .nd { color: #AA22FF } /* Name.Decorator */
.highlight .ni { color: #999999; font-weight: bold } /* Name.Entity */
.highlight .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
.highlight .nf { color: #0000FF } /* Name.Function */
.highlight .nl { color: #A0A000 } /* Name.Label */
.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
.highlight .nv { color: #19177C } /* Name.Variable */
.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
.highlight .w { color: #bbbbbb } /* Text.Whitespace */
.highlight .mb { color: #666666 } /* Literal.Number.Bin */
.highlight .mf { color: #666666 } /* Literal.Number.Float */
.highlight .mh { color: #666666 } /* Literal.Number.Hex */
.highlight .mi { color: #666666 } /* Literal.Number.Integer */
.highlight .mo { color: #666666 } /* Literal.Number.Oct */
.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
.highlight .sc { color: #BA2121 } /* Literal.String.Char */
.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
.highlight .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
.highlight .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
.highlight .sx { color: #008000 } /* Literal.String.Other */
.highlight .sr { color: #BB6688 } /* Literal.String.Regex */
.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
.highlight .ss { color: #19177C } /* Literal.String.Symbol */
.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
.highlight .fm { color: #0000FF } /* Name.Function.Magic */
.highlight .vc { color: #19177C } /* Name.Variable.Class */
.highlight .vg { color: #19177C } /* Name.Variable.Global */
.highlight .vi { color: #19177C } /* Name.Variable.Instance */
.highlight .vm { color: #19177C } /* Name.Variable.Magic */
.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
    </style>
<style type="text/css">
    /*This file contains any manual css for this page that needs to override the global styles.
This is only required when different pages style the same element differently. This is just
a hack to deal with our current css styles and no new styling should be added in this file.*/

#ipython-main-app {
    position: relative;
}
#jupyter-main-app {
    position: relative;
}

    </style>


<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
body {
  overflow: visible;
  padding: 8px;
}

div#notebook {
  overflow: visible;
  border-top: none;
}@media print {
  div.cell {
    display: block;
    page-break-inside: avoid;
  } 
  div.output_wrapper { 
    display: block;
    page-break-inside: avoid; 
  }
  div.output { 
    display: block;
    page-break-inside: avoid; 
  }
}
</style>

<!-- Custom stylesheet, it must be in the same directory as the html file -->
<link rel="stylesheet" href="custom.css">

<!-- Loading mathjax macro -->
<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-AMS_HTML"></script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
            processEscapes: true,
            processEnvironments: true
        },
        // Center justify equations in code and markdown cells. Elsewhere
        // we use CSS to left justify single line equations in code cells.
        displayAlign: 'center',
        "HTML-CSS": {
            styles: {'.MathJax_Display': {"margin": 0}},
            linebreaks: { automatic: true }
        }
    });
    </script>
    <!-- End of mathjax configuration --></head>

 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/jqueryui/1.12.1/jquery-ui.css">

<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/jqueryui/1.9.1/jquery-ui.min.js"></script>

<link rel="stylesheet" type="text/css" href="https://rawgit.com/ipython-contrib/jupyter_contrib_nbextensions/master/src/jupyter_contrib_nbextensions/nbextensions/toc2/main.css">

<link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<script src="https://rawgit.com/ipython-contrib/jupyter_contrib_nbextensions/master/src/jupyter_contrib_nbextensions/nbextensions/toc2/toc2.js"></script>

<script>
$( document ).ready(function(){

            var cfg = {"base_numbering": 1, "nav_menu": {}, "number_sections": true, "sideBar": true, "skip_h1_title": true, "title_cell": "Table of Contents", "title_sidebar": "Contents", "toc_cell": true, "toc_position": {}, "toc_section_display": true, "toc_window_display": false};

            // fire the main function with these parameters
            require(['nbextensions/toc2/toc2'], function (toc2) {
                toc2.table_of_contents(cfg);
            });
    });
</script>
<body>
  <div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><h1>Table of Contents<span class="tocSkip"></span></h1></p>
<div class="toc"><ul class="toc-item"><li><span><a href="#Context" data-toc-modified-id="Context-1"><span class="toc-item-num">1&nbsp;&nbsp;</span>Context</a></span></li><li><span><a href="#Content" data-toc-modified-id="Content-2"><span class="toc-item-num">2&nbsp;&nbsp;</span>Content</a></span></li><li><span><a href="#Acknowledgements" data-toc-modified-id="Acknowledgements-3"><span class="toc-item-num">3&nbsp;&nbsp;</span>Acknowledgements</a></span></li><li><span><a href="#Inspiration" data-toc-modified-id="Inspiration-4"><span class="toc-item-num">4&nbsp;&nbsp;</span>Inspiration</a></span></li><li><span><a href="#1.-Data-Info" data-toc-modified-id="1.-Data-Info-5"><span class="toc-item-num">5&nbsp;&nbsp;</span>1. Data Info</a></span><ul class="toc-item"><li><span><a href="#Pairplot" data-toc-modified-id="Pairplot-5.1"><span class="toc-item-num">5.1&nbsp;&nbsp;</span>Pairplot</a></span></li></ul></li><li><span><a href="#Correlation-Matrix" data-toc-modified-id="Correlation-Matrix-6"><span class="toc-item-num">6&nbsp;&nbsp;</span>Correlation Matrix</a></span></li><li><span><a href="#Building-machine-Learning-Models" data-toc-modified-id="Building-machine-Learning-Models-7"><span class="toc-item-num">7&nbsp;&nbsp;</span>Building machine Learning Models</a></span></li><li><span><a href="#Choosing-a-model" data-toc-modified-id="Choosing-a-model-8"><span class="toc-item-num">8&nbsp;&nbsp;</span>Choosing a model</a></span></li></ul></div>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>



<div class="output_text output_subarea output_execute_result">
<pre>[&#39;beers.csv&#39;, &#39;breweries.csv&#39;]</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Initializing-packages">Initializing packages<a class="anchor-link" href="#Initializing-packages">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Importing-datasets">Importing datasets<a class="anchor-link" href="#Importing-datasets">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Description-about-Problem">Description about Problem<a class="anchor-link" href="#Description-about-Problem">&#182;</a></h1><h2 id="Context">Context<a class="anchor-link" href="#Context">&#182;</a></h2><p>It's a great time to be a craft beer fan in the U.S.! There are a ton of beer styles and brands to choose from and breweries have become very successful in the last several years. Breweries owe it all to beer lovers around the world! This dataset contains a list of 2,410 US craft beers and 510 US breweries. The beers and breweries are linked together by the "id". This data was collected in January 2017 from CraftCans.com. The dataset is an a tidy format and values have been cleaned up for your enjoyment.</p>
<h2 id="Content">Content<a class="anchor-link" href="#Content">&#182;</a></h2><p>beers.csv - Contains data on 2000+ craft canned beers</p>
<p>breweries.csv - Contains data for 500+ breweries in the United States</p>
<p>Abbreviation: ABV: ABV-Alcohol by volume , IBU: International Bitterness Units</p>
<h2 id="Acknowledgements">Acknowledgements<a class="anchor-link" href="#Acknowledgements">&#182;</a></h2><p>If you are interested in learning more about how this dataset was acquired, I wrote an extensive blogpost about it <a href="http://www.jeannicholashould.com/python-web-scraping-tutorial-for-craft-beers.html">http://www.jeannicholashould.com/python-web-scraping-tutorial-for-craft-beers.html</a>.</p>
<h2 id="Inspiration">Inspiration<a class="anchor-link" href="#Inspiration">&#182;</a></h2><p>Can you predict the beer type from the characteristics provided in the dataset?</p>
<p>What is the most popular beer in North Dakota?</p>
<p>Cheers to beer</p>
<p><img src="data:image/jpeg;base64,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" alt="pintsender.jpg"></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Understand-the-dataset">Understand the dataset<a class="anchor-link" href="#Understand-the-dataset">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Unnamed: 0</th>
      <th>abv</th>
      <th>ibu</th>
      <th>id</th>
      <th>name</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>0.050</td>
      <td>NaN</td>
      <td>1436</td>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>408</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>0.066</td>
      <td>NaN</td>
      <td>2265</td>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>0.071</td>
      <td>NaN</td>
      <td>2264</td>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>0.090</td>
      <td>NaN</td>
      <td>2263</td>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>0.075</td>
      <td>NaN</td>
      <td>2262</td>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Unnamed: 0</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>0.050</td>
      <td>NaN</td>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>408</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>0.066</td>
      <td>NaN</td>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>0.071</td>
      <td>NaN</td>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>0.090</td>
      <td>NaN</td>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>0.075</td>
      <td>NaN</td>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Unnamed: 0</th>
      <th>name</th>
      <th>city</th>
      <th>state</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Joining-breweries-and-canned-beer-dataset">Joining breweries and canned beer dataset<a class="anchor-link" href="#Joining-breweries-and-canned-beer-dataset">&#182;</a></h1><p>The beers and breweries are linked together by the "id".</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>   id    abv  ibu                 name                           style  \
0   0  0.050  NaN             Pub Beer             American Pale Lager   
1   1  0.066  NaN          Devil&#39;s Cup         American Pale Ale (APA)   
2   2  0.071  NaN  Rise of the Phoenix                    American IPA   
3   3  0.090  NaN             Sinister  American Double / Imperial IPA   
4   4  0.075  NaN        Sex and Candy                    American IPA   

   brewery_id  ounces  
0         408    12.0  
1         177    12.0  
2         177    12.0  
3         177    12.0  
4         177    12.0  
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>



<div class="output_text output_subarea output_execute_result">
<pre>Index([&#39;id&#39;, &#39;abv&#39;, &#39;ibu&#39;, &#39;name_x&#39;, &#39;style&#39;, &#39;brewery_id&#39;, &#39;ounces&#39;, &#39;name_y&#39;,
       &#39;city&#39;, &#39;state&#39;, &#39;_merge&#39;],
      dtype=&#39;object&#39;)</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name_x</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
      <th>name_y</th>
      <th>city</th>
      <th>state</th>
      <th>_merge</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>0.050</td>
      <td>NaN</td>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>408</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
      <td>both</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>0.066</td>
      <td>NaN</td>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>177</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
      <td>both</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>0.071</td>
      <td>NaN</td>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
      <td>both</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>0.090</td>
      <td>NaN</td>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
      <td>both</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>0.075</td>
      <td>NaN</td>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
      <td>both</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Dropping-some-columns">Dropping some columns<a class="anchor-link" href="#Dropping-some-columns">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name_x</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
      <th>name_y</th>
      <th>city</th>
      <th>state</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>0.050</td>
      <td>NaN</td>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>408</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>0.066</td>
      <td>NaN</td>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>177</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>0.071</td>
      <td>NaN</td>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>0.090</td>
      <td>NaN</td>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>0.075</td>
      <td>NaN</td>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Renaming-columns">Renaming columns<a class="anchor-link" href="#Renaming-columns">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>0.050</td>
      <td>NaN</td>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>408</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>0.066</td>
      <td>NaN</td>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>177</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>0.071</td>
      <td>NaN</td>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>0.090</td>
      <td>NaN</td>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>0.075</td>
      <td>NaN</td>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>   id    abv  ibu         name_of_beer                           style  \
0   0  0.050  NaN             Pub Beer             American Pale Lager   
1   1  0.066  NaN          Devil&#39;s Cup         American Pale Ale (APA)   
2   2  0.071  NaN  Rise of the Phoenix                    American IPA   
3   3  0.090  NaN             Sinister  American Double / Imperial IPA   
4   4  0.075  NaN        Sex and Candy                    American IPA   

   brewery_id  ounces            name_of_brewery           city state  
0         408    12.0         NorthGate Brewing     Minneapolis    MN  
1         177    12.0  Against the Grain Brewery     Louisville    KY  
2         177    12.0   Jack&#39;s Abby Craft Lagers     Framingham    MA  
3         177    12.0  Mike Hess Brewing Company      San Diego    CA  
4         177    12.0    Fort Point Beer Company  San Francisco    CA  
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>        id    abv   ibu          name_of_beer                     style  \
2405  2405  0.067  45.0             Belgorado               Belgian IPA   
2406  2406  0.052   NaN         Rail Yard Ale  American Amber / Red Ale   
2407  2407  0.055   NaN       B3K Black Lager               Schwarzbier   
2408  2408  0.055  40.0   Silverback Pale Ale   American Pale Ale (APA)   
2409  2409  0.052   NaN  Rail Yard Ale (2009)  American Amber / Red Ale   

      brewery_id  ounces name_of_brewery city state  
2405         424    12.0             NaN  NaN   NaN  
2406         424    12.0             NaN  NaN   NaN  
2407         424    12.0             NaN  NaN   NaN  
2408         424    12.0             NaN  NaN   NaN  
2409         424    12.0             NaN  NaN   NaN  
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Preprocessing-the-joined-dataset">Preprocessing the joined dataset<a class="anchor-link" href="#Preprocessing-the-joined-dataset">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="1.-Data-Info">1. Data Info<a class="anchor-link" href="#1.-Data-Info">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>(2410, 10)
&lt;class &#39;pandas.core.frame.DataFrame&#39;&gt;
Int64Index: 2410 entries, 0 to 2409
Data columns (total 10 columns):
 #   Column           Non-Null Count  Dtype  
---  ------           --------------  -----  
 0   id               2410 non-null   int64  
 1   abv              2348 non-null   float64
 2   ibu              1405 non-null   float64
 3   name_of_beer     2410 non-null   object 
 4   style            2405 non-null   object 
 5   brewery_id       2410 non-null   int64  
 6   ounces           2410 non-null   float64
 7   name_of_brewery  558 non-null    object 
 8   city             558 non-null    object 
 9   state            558 non-null    object 
dtypes: float64(3), int64(2), object(5)
memory usage: 207.1+ KB
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>id                    0
abv                  62
ibu                1005
name_of_beer          0
style                 5
brewery_id            0
ounces                0
name_of_brewery    1852
city               1852
state              1852
dtype: int64
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>&lt;class &#39;pandas.core.frame.DataFrame&#39;&gt;
Int64Index: 2410 entries, 0 to 2409
Data columns (total 10 columns):
 #   Column           Non-Null Count  Dtype  
---  ------           --------------  -----  
 0   id               2410 non-null   int64  
 1   abv              2410 non-null   float64
 2   ibu              2410 non-null   float64
 3   name_of_beer     2410 non-null   object 
 4   style            2405 non-null   object 
 5   brewery_id       2410 non-null   int64  
 6   ounces           2410 non-null   float64
 7   name_of_brewery  558 non-null    object 
 8   city             558 non-null    object 
 9   state            558 non-null    object 
dtypes: float64(3), int64(2), object(5)
memory usage: 207.1+ KB
None
   id    abv        ibu         name_of_beer                           style  \
0   0  0.050  42.713167             Pub Beer             American Pale Lager   
1   1  0.066  42.713167          Devil&#39;s Cup         American Pale Ale (APA)   
2   2  0.071  42.713167  Rise of the Phoenix                    American IPA   
3   3  0.090  42.713167             Sinister  American Double / Imperial IPA   
4   4  0.075  42.713167        Sex and Candy                    American IPA   

   brewery_id  ounces            name_of_brewery           city state  
0         408    12.0         NorthGate Brewing     Minneapolis    MN  
1         177    12.0  Against the Grain Brewery     Louisville    KY  
2         177    12.0   Jack&#39;s Abby Craft Lagers     Framingham    MA  
3         177    12.0  Mike Hess Brewing Company      San Diego    CA  
4         177    12.0    Fort Point Beer Company  San Francisco    CA  
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>558</th>
      <td>558</td>
      <td>0.047</td>
      <td>42.713167</td>
      <td>White Zombie Ale</td>
      <td>Witbier</td>
      <td>331</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>559</th>
      <td>559</td>
      <td>0.052</td>
      <td>42.713167</td>
      <td>Firewater India Pale Ale</td>
      <td>American IPA</td>
      <td>331</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>560</th>
      <td>560</td>
      <td>0.056</td>
      <td>42.713167</td>
      <td>Farmer Ted's Farmhouse Cream Ale</td>
      <td>Cream Ale</td>
      <td>331</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>561</th>
      <td>561</td>
      <td>0.048</td>
      <td>16.000000</td>
      <td>Whitecap Wit</td>
      <td>Witbier</td>
      <td>285</td>
      <td>16.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>562</th>
      <td>562</td>
      <td>0.078</td>
      <td>16.000000</td>
      <td>Seiche Scottish Ale</td>
      <td>Scottish Ale</td>
      <td>285</td>
      <td>16.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2405</th>
      <td>2405</td>
      <td>0.067</td>
      <td>45.000000</td>
      <td>Belgorado</td>
      <td>Belgian IPA</td>
      <td>424</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2406</th>
      <td>2406</td>
      <td>0.052</td>
      <td>42.713167</td>
      <td>Rail Yard Ale</td>
      <td>American Amber / Red Ale</td>
      <td>424</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2407</th>
      <td>2407</td>
      <td>0.055</td>
      <td>42.713167</td>
      <td>B3K Black Lager</td>
      <td>Schwarzbier</td>
      <td>424</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2408</th>
      <td>2408</td>
      <td>0.055</td>
      <td>40.000000</td>
      <td>Silverback Pale Ale</td>
      <td>American Pale Ale (APA)</td>
      <td>424</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2409</th>
      <td>2409</td>
      <td>0.052</td>
      <td>42.713167</td>
      <td>Rail Yard Ale (2009)</td>
      <td>American Amber / Red Ale</td>
      <td>424</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
<p>1852 rows × 10 columns</p>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>&lt;class &#39;pandas.core.frame.DataFrame&#39;&gt;
Int64Index: 2410 entries, 0 to 2409
Data columns (total 10 columns):
 #   Column           Non-Null Count  Dtype  
---  ------           --------------  -----  
 0   id               2410 non-null   int64  
 1   abv              2410 non-null   float64
 2   ibu              2410 non-null   float64
 3   name_of_beer     2410 non-null   object 
 4   style            2410 non-null   object 
 5   brewery_id       2410 non-null   int64  
 6   ounces           2410 non-null   float64
 7   name_of_brewery  2410 non-null   object 
 8   city             2410 non-null   object 
 9   state            2410 non-null   object 
dtypes: float64(3), int64(2), object(5)
memory usage: 207.1+ KB
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2405</th>
      <td>2405</td>
      <td>0.067</td>
      <td>45.000000</td>
      <td>Belgorado</td>
      <td>Belgian IPA</td>
      <td>424</td>
      <td>12.0</td>
      <td>Blackrocks Brewery</td>
      <td>Portland</td>
      <td>CO</td>
    </tr>
    <tr>
      <th>2406</th>
      <td>2406</td>
      <td>0.052</td>
      <td>42.713167</td>
      <td>Rail Yard Ale</td>
      <td>American Amber / Red Ale</td>
      <td>424</td>
      <td>12.0</td>
      <td>Blackrocks Brewery</td>
      <td>Portland</td>
      <td>CO</td>
    </tr>
    <tr>
      <th>2407</th>
      <td>2407</td>
      <td>0.055</td>
      <td>42.713167</td>
      <td>B3K Black Lager</td>
      <td>Schwarzbier</td>
      <td>424</td>
      <td>12.0</td>
      <td>Blackrocks Brewery</td>
      <td>Portland</td>
      <td>CO</td>
    </tr>
    <tr>
      <th>2408</th>
      <td>2408</td>
      <td>0.055</td>
      <td>40.000000</td>
      <td>Silverback Pale Ale</td>
      <td>American Pale Ale (APA)</td>
      <td>424</td>
      <td>12.0</td>
      <td>Blackrocks Brewery</td>
      <td>Portland</td>
      <td>CO</td>
    </tr>
    <tr>
      <th>2409</th>
      <td>2409</td>
      <td>0.052</td>
      <td>42.713167</td>
      <td>Rail Yard Ale (2009)</td>
      <td>American Amber / Red Ale</td>
      <td>424</td>
      <td>12.0</td>
      <td>Blackrocks Brewery</td>
      <td>Portland</td>
      <td>CO</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="EDA">EDA<a class="anchor-link" href="#EDA">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Pairplot">Pairplot<a class="anchor-link" href="#Pairplot">&#182;</a></h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>



<div class="output_text output_subarea output_execute_result">
<pre>&lt;seaborn.axisgrid.PairGrid at 0x2881c91c0c8&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"> </div>



<div class="output_png output_subarea ">
<img src="output_36_1.png"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Correlation-Matrix">Correlation Matrix<a class="anchor-link" href="#Correlation-Matrix">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>             abv       ibu    ounces
abv     1.000000  0.516560  0.167589
ibu     0.516560  1.000000  0.039995
ounces  0.167589  0.039995  1.000000
</pre>
</div>
</div>

<div class="output_area">

    <div class="prompt"> </div>



<div class="output_png output_subarea ">
<img src="output_38_1.png"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Scaling-the-datasets">Scaling the datasets<a class="anchor-link" href="#Scaling-the-datasets">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
      <th>abv_scale</th>
      <th>ibu_scale</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
      <td>0.385827</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
      <td>0.511811</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
      <td>0.551181</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
      <td>0.700787</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
      <td>0.582677</td>
      <td>0.288904</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Detecting-outliers">Detecting outliers<a class="anchor-link" href="#Detecting-outliers">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>



<div class="output_text output_subarea output_execute_result">
<pre>&lt;matplotlib.axes._subplots.AxesSubplot at 0x2881d0e82c8&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"> </div>



<div class="output_png output_subarea ">
<img src="output_43_1.png"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>



<div class="output_text output_subarea output_execute_result">
<pre>&lt;matplotlib.axes._subplots.AxesSubplot at 0x2881d151cc8&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"> </div>



<div class="output_png output_subarea ">
<img src="output_44_1.png"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
      <th>abv_scale</th>
      <th>ibu_scale</th>
      <th>ibu_scale_zscore</th>
      <th>abv_scale_zscore</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
      <td>0.385827</td>
      <td>0.288904</td>
      <td>0.0</td>
      <td>-0.707805</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
      <td>0.511811</td>
      <td>0.288904</td>
      <td>0.0</td>
      <td>0.481535</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
      <td>0.551181</td>
      <td>0.288904</td>
      <td>0.0</td>
      <td>0.853203</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
      <td>0.700787</td>
      <td>0.288904</td>
      <td>0.0</td>
      <td>2.265544</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
      <td>0.582677</td>
      <td>0.288904</td>
      <td>0.0</td>
      <td>1.150538</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stderr output_text">
<pre>C:\Users\MasterDK-Laptop\anaconda3\lib\site-packages\pandas\core\frame.py:3997: SettingWithCopyWarning: 
A value is trying to be set on a copy of a slice from a DataFrame

See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
  errors=errors,
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
      <th>abv_scale</th>
      <th>ibu_scale</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
      <td>0.385827</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
      <td>0.511811</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
      <td>0.551181</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
      <td>0.700787</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
      <td>0.582677</td>
      <td>0.288904</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>


<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ounces</th>
      <th>abv_scale</th>
      <th>ibu_scale</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>ounces</th>
      <td>1.000000</td>
      <td>0.166022</td>
      <td>0.035642</td>
    </tr>
    <tr>
      <th>abv_scale</th>
      <td>0.166022</td>
      <td>1.000000</td>
      <td>0.499503</td>
    </tr>
    <tr>
      <th>ibu_scale</th>
      <td>0.035642</td>
      <td>0.499503</td>
      <td>1.000000</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Building-machine-Learning-Models">Building machine Learning Models<a class="anchor-link" href="#Building-machine-Learning-Models">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Inspiration
Can you predict the beer type from the characteristics provided in the dataset?</p>
<p>What is the most popular beer in North Dakota?</p>
<p>Cheers to beer</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>   abv_scale  ibu_scale  ounces                           style
0   0.385827   0.288904    12.0             American Pale Lager
1   0.511811   0.288904    12.0         American Pale Ale (APA)
2   0.551181   0.288904    12.0                    American IPA
3   0.700787   0.288904    12.0  American Double / Imperial IPA
4   0.582677   0.288904    12.0                    American IPA
shape of dataset is: (2379, 4)
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Choosing-a-model">Choosing a model<a class="anchor-link" href="#Choosing-a-model">&#182;</a></h2><p>In statistics, multinomial logistic regression is a classification method that generalizes <strong>logistic regression to multiclass problems, i.e. with more than two possible discrete outcomes.</strong>[1]</p>
<p>That is, it is a model that is used to predict the probabilities of the <strong>different possible outcomes of a categorically distributed dependent variable</strong>, given a <strong>set of 
independent variables (which may be real-valued, binary-valued, categorical-valued, etc.).</strong></p>
<p>Reference: <a href="https://en.wikipedia.org/wiki/Multinomial_logistic_regression">https://en.wikipedia.org/wiki/Multinomial_logistic_regression</a></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Training-and-test-creation">Training and test creation<a class="anchor-link" href="#Training-and-test-creation">&#182;</a></h1><p>Stratification is the process of rearranging the data so as to ensure that each fold is a good representative of the whole.</p>
<p>For example, in a binary classification problem where each class comprises of 50% of the data, it is best to 
arrange the data such that in every fold, each class comprises of about half the instances.</p>
<p>It is generally a better approach when dealing with both bias and variance. A randomly selected fold might not adequately represent the minor class, particularly in cases where there is a huge class imbalance.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Logistic-regression-with-multinomial-classification">Logistic regression with multinomial classification<a class="anchor-link" href="#Logistic-regression-with-multinomial-classification">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stderr output_text">
<pre>C:\Users\MasterDK-Laptop\anaconda3\lib\site-packages\sklearn\linear_model\_logistic.py:764: ConvergenceWarning: lbfgs failed to converge (status=1):
STOP: TOTAL NO. of ITERATIONS REACHED LIMIT.

Increase the number of iterations (max_iter) or scale the data as shown in:
    https://scikit-learn.org/stable/modules/preprocessing.html
Please also refer to the documentation for alternative solver options:
    https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression
  extra_warning_msg=_LOGISTIC_SOLVER_CONVERGENCE_MSG)
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Confusion-matrix">Confusion matrix<a class="anchor-link" href="#Confusion-matrix">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>Confusion Matrix : 
 [[0 0 0 ... 0 0 0]
 [0 0 0 ... 0 0 0]
 [0 0 0 ... 0 0 0]
 ...
 [0 0 0 ... 0 0 0]
 [0 0 0 ... 0 0 0]
 [0 0 0 ... 0 0 0]]
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Accuracy-score">Accuracy score<a class="anchor-link" href="#Accuracy-score">&#182;</a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"> </div>

<div class="output_subarea output_stream output_stdout output_text">
<pre>Accuracy :  0.26218487394957984
</pre>
</div>
</div>

</div>
</div>

</div>
    </div>
  </div>
</body>

 


</html>
