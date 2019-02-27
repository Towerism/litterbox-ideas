<template lang="pug">
  section#footer.wrapper
    .title The Rest Of It
    .container
      header.style1
        h2 Ipsum sapien elementum portitor?
        p
          | Sed turpis tortor, tincidunt sed ornare in metus porttitor mollis nunc in aliquet.
          br
          | 								Nam pharetra laoreet imperdiet volutpat etiam feugiat.
      .row
        .col-6.col-12-medium
          // Contact Form
          section
            form(method='post', action='#')
              .row.gtr-50
                .col-6.col-12-small
                  input#contact-name(type='text', name='name', placeholder='Name')
                .col-6.col-12-small
                  input#contact-email(type='text', name='email', placeholder='Email')
                .col-12
                  textarea#contact-message(name='message', placeholder='Message', rows='4')
                .col-12
                  ul.actions
                    li
                      input.style1(type='submit', value='Send')
                    li
                      input.style2(type='reset', value='Reset')
        .col-6.col-12-medium
          // Contact
          section.feature-list.small
            .row
              .col-6.col-12-small
                section
                  h3.icon.fa-home Mailing Address
                  p
                    | Untitled Corp
                    br
                    | 														1234 Somewhere Rd
                    br
                    | 														Nashville, TN 00000
              .col-6.col-12-small
                section
                  h3.icon.fa-comment Social
                  p
                    a(href='#') @untitled-corp
                    br
                    a(href='#') linkedin.com/untitled
                    br
                    a(href='#') facebook.com/untitled
              .col-6.col-12-small
                section
                  h3.icon.fa-envelope Email
                  p
                    a(href='#') info@untitled.tld
              .col-6.col-12-small
                section
                  h3.icon.fa-phone Phone
                  p
                    | (000) 555-0000
      #copyright
        ul
          li © Untitled.
          li
            | Design:
            a(href='http://html5up.net') HTML5 UP
</template>
