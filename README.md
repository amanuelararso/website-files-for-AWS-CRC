# Website Files for Cloud Resume Challenge

This repository contains the HTML, CSS, and image files for the Cloud Resume Challenge website. When changes are pushed to this repository, the associated S3 bucket is automatically updated.

## Features

- **Automatic Deployment**: GitHub Actions are configured to automatically update the S3 bucket hosting the website whenever changes are pushed to the repository.
- **Static Website**: The repository includes an `index.html` file, CSS for styling, and images used on the website.

## Setup

### Prerequisites

- AWS account with an S3 bucket configured to host a static website.
- AWS CLI configured with your credentials.
- GitHub repository linked to your S3 bucket.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/amanuelararso/website-files-for-AWS-CRC.git
   cd website-files-for-AWS-CRC
   ```

2. **Set up GitHub Secrets:**
   - `AWS_ACCESS_KEY_ID`
   - `AWS_SECRET_ACCESS_KEY`
   - `AWS_REGION`
   - `S3_BUCKET_NAME`

3. **Configure GitHub Actions:**
   The workflow file (`.github/workflows/main.yml`) is already set up to deploy the website files automatically.

## Usage

1. **Make changes to the website files:**
   Modify the `index.html`, CSS files, or images as needed.

2. **Push changes to the repository:**
   ```bash
   git add .
   git commit -m "Update website files"
   git push origin main
   ```

3. **Automatic Deployment:**
   GitHub Actions will trigger and update your S3 bucket with the latest website files.

## Dependencies

- None

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## Contact

For any questions or issues, please open an issue in this repository.
