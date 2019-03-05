
close slack, 
then edit the indicated file by add the following block at the bottom
save
then reopen slack

/Applications/Slack.app/Contents/Resources/app.asar.unpacked/src/static/ssb-interop.js

```document.addEventListener('DOMContentLoaded', function() {
  let tt__customCss = `.menu ul li a:not(.inline_menu_link) {color: #fff !important;}`
  $.ajax({
      url: 'https://cdn.rawgit.com/laCour/slack-night-mode/master/css/raw/black.css',
      success: function(css) {
          $("<style></style>").appendTo('head').html(css + tt__customCss);
          $("<style></style>").appendTo('head').html('.p-threads_footer__input--legacy .p-message_input_field {background: padding-box #545454}');
          $("<style></style>").appendTo('head').html('.p-threads_footer__input--legacy .p-message_input_file_button {background: padding-box #545454}');
          $("<style></style>").appendTo('head').html('.p-threads_footer__input--legacy .p-message_input_field .ql-placeholder {color: #e6e6e6}');
          $("<style></style>").appendTo('head').html('.p-threads_footer__input .p-message_input_field.focus~.p-message_input_file_button:not(:hover) {color: #949494}');
          $("<style></style>").appendTo('head').html('.c-texty_input.focus .c-texty_input__button {color: #949494}');
          $("<style></style>").appendTo('head').html('.p-channel_sidebar {background: #363636 !important}');
          $("<style></style>").appendTo('head').html('#client_body:not(.onboarding):not(.feature_global_nav_layout):before {background: inherit;}');
      }
  });
});```
