# File Upload Service

This project is a file upload service built with Node.js, Express, and MongoDB. It supports uploading files to the local server and Cloudinary, and sends email notifications upon successful uploads.

## Features

- Upload files to the local server
- Upload images and videos to Cloudinary
- Resize images before uploading
- Send email notifications after successful uploads

## Prerequisites

- Node.js
- MongoDB
- Cloudinary account
- Email account for sending notifications

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/fileupload.git
    cd fileupload
    ```

2. Install dependencies:
    ```sh
    npm install
    ```

3. Create a [.env](http://_vscodecontentref_/0) file in the root directory and add your environment variables:
    ```env
    CLOUD_NAME=your_cloud_name
    API_KEY=your_api_key
    API_SECRET=your_api_secret
    MONGODB_URL=your_mongodb_url
    PORT=your_port
    MAIL_HOST=your_mail_host
    MAIL_USER=your_mail_user
    MAIL_PASS=your_mail_pass
    ```

4. Start the server:
    ```sh
    npm run dev
    ```

## API Endpoints

- `POST /api/v1/upload/localFileUpload`: Upload a file to the local server
- `POST /api/v1/upload/imageUpload`: Upload an image to Cloudinary
- `POST /api/v1/upload/videoUpload`: Upload a video to Cloudinary
- `POST /api/v1/upload/imageSizeReducer`: Resize and upload an image to Cloudinary

## Project Structure
