# How To:  Image Positioning

## Default Positioning

By default, images are positioned vertically aligned relative to the location the `.ve-image` tag is defined in the source text.  The image will be rendered as wide as possible such that the height is no more than 40% of the window height.  Try changing the window height and notice how the height of the image adjusts.

.ve-image wc:Chiang_Kai-shek_memorial_2_amk.jpg

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Odio ut enim blandit volutpat maecenas volutpat blandit. Risus viverra adipiscing at in tellus integer. Cras adipiscing enim eu turpis egestas pretium aenean. Egestas pretium aenean pharetra magna ac placerat. Amet risus nullam eget felis eget nunc lobortis mattis aliquam. Aliquet lectus proin nibh nisl condimentum id. Id diam vel quam elementum pulvinar etiam non quam lacus. Amet mattis vulputate enim nulla aliquet porttitor. Tortor condimentum lacinia quis vel. Feugiat nisl pretium fusce id.

## Full Positioning

Similar to the default mode, images are positioned vertically aligned relative to the location the `.ve-image` tag is defined in the source text.  The image is rendered as wide as possible but the _height is not restricted to 40% of the window height_.

.ve-image wc:Chiang_Kai-shek_memorial_2_amk.jpg full

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Odio ut enim blandit volutpat maecenas volutpat blandit. Risus viverra adipiscing at in tellus integer. Cras adipiscing enim eu turpis egestas pretium aenean. Egestas pretium aenean pharetra magna ac placerat. Amet risus nullam eget felis eget nunc lobortis mattis aliquam. Aliquet lectus proin nibh nisl condimentum id. Id diam vel quam elementum pulvinar etiam non quam lacus. Amet mattis vulputate enim nulla aliquet porttitor. Tortor condimentum lacinia quis vel. Feugiat nisl pretium fusce id.

## Right and Left Positioning

When the positioning is defined as `left` or `right` the image is aligned with the left or right side of the window and the width is restricted to 50% of the window.  The image height is scaled to retain the original image orientation. Any text that follows the `ve-image` within the same section will be positioned on the opposite side of the window and will wrap around the image if the text length exceeds the image height.

.ve-image wc:Chiang_Kai-shek_memorial_2_amk.jpg right

Neque ornare aenean euismod elementum nisi quis eleifend. Enim eu turpis egestas pretium aenean pharetra magna ac placerat. Semper feugiat nibh sed pulvinar. Et odio pellentesque diam volutpat commodo sed egestas egestas fringilla. Duis tristique sollicitudin nibh sit amet commodo nulla facilisi nullam. Massa tempor nec feugiat nisl pretium fusce. Pellentesque adipiscing commodo elit at. Facilisis magna etiam tempor orci eu. Pellentesque eu tincidunt tortor aliquam nulla. Nulla porttitor massa id neque aliquam vestibulum morbi blandit cursus. Ornare suspendisse sed nisi lacus sed viverra tellus in hac. At quis risus sed vulputate odio ut enim. Justo donec enim diam vulputate ut pharetra sit.

Cras tincidunt lobortis feugiat vivamus at augue. Malesuada proin libero nunc consequat interdum varius sit. Donec adipiscing tristique risus nec feugiat in fermentum posuere. Congue quisque egestas diam in arcu cursus euismod. Urna duis convallis convallis tellus id. Tristique sollicitudin nibh sit amet commodo nulla facilisi nullam. Posuere morbi leo urna molestie. Purus faucibus ornare suspendisse sed nisi lacus. Nulla aliquet porttitor lacus luctus accumsan tortor posuere ac ut. At tempor commodo ullamcorper a lacus vestibulum sed arcu. Nulla facilisi nullam vehicula ipsum. Feugiat pretium nibh ipsum consequat nisl vel pretium lectus quam. Tempus quam pellentesque nec nam aliquam. Mattis ullamcorper velit sed ullamcorper morbi tincidunt.

## "Sticky" Images

In some cases it is desireable to force the image to remain visible when text in the same section is scrolled.  Adding the `sticky` attribute to a `.ve-image` declaration will stick the image at the top of the window when scolling text in the same section.  The sticky attribute can be used with default, full, left, or right positioning.  When used with default or full positioning text will scroll behind the image.  With left or right positioning the text will scroll in the adjacent column.

## Full Positioning with Sticky

.ve-image wc:Chiang_Kai-shek_memorial_2_amk.jpg sticky

Sagittis orci a scelerisque purus. Montes nascetur ridiculus mus mauris. Consectetur a erat nam at lectus urna duis convallis. Pellentesque dignissim enim sit amet venenatis urna cursus eget nunc. Est ultricies integer quis auctor. Lobortis mattis aliquam faucibus purus in massa. Ipsum nunc aliquet bibendum enim facilisis gravida neque. Mattis ullamcorper velit sed ullamcorper morbi tincidunt ornare massa. Tincidunt praesent semper feugiat nibh sed. Viverra tellus in hac habitasse. Consectetur adipiscing elit pellentesque habitant morbi.

Est pellentesque elit ullamcorper dignissim cras. Pulvinar elementum integer enim neque volutpat ac. Interdum velit euismod in pellentesque massa placerat duis. Nulla aliquet porttitor lacus luctus accumsan tortor. Morbi enim nunc faucibus a pellentesque sit amet porttitor eget. Lectus nulla at volutpat diam ut venenatis tellus. Egestas pretium aenean pharetra magna ac placerat vestibulum. Nisl nisi scelerisque eu ultrices vitae auctor eu. Eget magna fermentum iaculis eu non. Hac habitasse platea dictumst vestibulum rhoncus est. Elementum eu facilisis sed odio morbi quis commodo odio. Egestas pretium aenean pharetra magna ac placerat vestibulum lectus. Vehicula ipsum a arcu cursus vitae congue mauris. Vulputate sapien nec sagittis aliquam malesuada bibendum arcu.

## Right Positioning with Sticky

.ve-image wc:Chiang_Kai-shek_memorial_2_amk.jpg right sticky

Sagittis orci a scelerisque purus. Montes nascetur ridiculus mus mauris. Consectetur a erat nam at lectus urna duis convallis. Pellentesque dignissim enim sit amet venenatis urna cursus eget nunc. Est ultricies integer quis auctor. Lobortis mattis aliquam faucibus purus in massa. Ipsum nunc aliquet bibendum enim facilisis gravida neque. Mattis ullamcorper velit sed ullamcorper morbi tincidunt ornare massa. Tincidunt praesent semper feugiat nibh sed. Viverra tellus in hac habitasse. Consectetur adipiscing elit pellentesque habitant morbi.

Est pellentesque elit ullamcorper dignissim cras. Pulvinar elementum integer enim neque volutpat ac. Interdum velit euismod in pellentesque massa placerat duis. Nulla aliquet porttitor lacus luctus accumsan tortor. Morbi enim nunc faucibus a pellentesque sit amet porttitor eget. Lectus nulla at volutpat diam ut venenatis tellus. Egestas pretium aenean pharetra magna ac placerat vestibulum. Nisl nisi scelerisque eu ultrices vitae auctor eu. Eget magna fermentum iaculis eu non. Hac habitasse platea dictumst vestibulum rhoncus est. Elementum eu facilisis sed odio morbi quis commodo odio. Egestas pretium aenean pharetra magna ac placerat vestibulum lectus. Vehicula ipsum a arcu cursus vitae congue mauris. Vulputate sapien nec sagittis aliquam malesuada bibendum arcu.