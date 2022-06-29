- name: Cloudinary Upload Images
  uses: emmanuelgautier/cloudinary-upload-action@v1.0

- name: Cloudinary Upload Image
      uses: aws-actions/configure-aws-credentials@v1
      with:
          cloud-name: ${{ secrets.CLOUDINARY_CLOUD_NAME }}
          api-key: ${{ secrets.CLOUDINARY_API_KEY }}
          api-secret: ${{ secrets.CLOUDINARY_API_SECRET }}
          image: "./your-image.jpg"
