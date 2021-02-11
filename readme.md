# cloudinary component

**no styling or css is required for this task**

1. Setup a minimal `Node.js` server with `Express.js`
2. Setup a minimal `Vue.js` application
3. Create free [Cloudinary](https://cloudinary.com) test account
4. Create a `Vue.js` component called `image.vue`
5. In `image.vue` create a simple html container without styling

```html
  <div class="upload">
    <div class="upload__placeholder">Upload</div>
    <div v-if="image" class="upload__image"><img /></div>
  </div>
```

6. In the `mounted` hook, install the [Cloudinary Upload Widget](https://cloudinary.com/documentation/upload_widget)
7. The cloudinary widget comes with the option of `signed` or `unsigned` uploads. Configure the widget to work with [`signed` uploads](https://cloudinary.com/documentation/upload_widget#signed_uploads).
8. Follow the [`cloudinary` docs](https://cloudinary.com/documentation/upload_widget#signed_uploads) to use your simple `Node.js` server to create the cloudinary upload widget signature.
9. Configure the cloudinary widget to use cropping with an aspect ratio of 1:1
10. Configure the cloudinary widget to accept only one image
10. When you click on the `.upload` html element, open the cloudinary upload widget
11. When you successsfully uploaded an image, store the image into the dataset of `image.vue`. This should result in showing the `.upload__image` container and hiding the `upload__placeholder` container.

