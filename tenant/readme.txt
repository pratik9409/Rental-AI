Tenant Application Generator
This is a Streamlit application that allows tenants to generate a comprehensive application for rental properties. The application collects various documents and information from the tenant and generates a combined PDF file containing all the submitted data. The generated PDF can be sent directly to the tenant's email address or to the landlord/realtor/property manager upon request.

Technologies Used
Python
Streamlit
AWS S3 (Amazon Simple Storage Service)
MongoDB
PyMongo
Boto3
Reportlab
PyPDF2
Docx2pdf
Pytesseract (for OCR)
Pillow
pdf2image
smtplib (for sending emails)
Features
Tenant Information Collection: The application collects essential information from the tenant, such as their name, email address, phone number, and a brief introduction.

Document Upload: Tenants can upload various documents to support their application, including:

Credit Score Reports (PDF, DOCX, TXT)
Job Letters (PDF, DOCX, TXT)
Paystubs (PDF, DOCX, TXT)
Curriculum Vitae (CV) (PDF, DOCX, TXT)
Bank Statements (PDF, DOCX, TXT)
Form 310 Lease (Residential Tenancy Agreement) (PDF, DOCX, TXT)
Landlord Reference Letters (PDF, DOCX, TXT)
YouTube Video Introduction: Tenants can optionally provide a 1-minute YouTube video introduction URL.

Document Processing and Storage: The uploaded documents are processed and stored in an Amazon S3 bucket. PDF files are converted to images using pdf2image, and OCR (Optical Character Recognition) is performed on the images using pytesseract to extract text content. The extracted text is then stored as a separate TXT file in S3.

Tenant Data Storage: Tenant information and metadata are stored in a MongoDB database for future reference.

PDF Generation: A combined PDF file is generated, containing the tenant's textual information and all the uploaded documents. The PDF is created using the reportlab library.

Email Delivery: The generated PDF file can be sent directly to the tenant's email address, with an optional attachment containing the combined PDF.

Listing Selection: Tenants can select the address they are applying for from a list of available listings fetched from the S3 bucket.

Automatic Landlord/Realtor/Property Manager Submission: Upon request, the application can automatically send the generated PDF to the landlord/realtor/property manager associated with the selected listing.

Setup and Installation
Clone the repository:
git clone https://github.com/your-repo/tenant-application-generator.git



Install the required Python packages:
pip install -r requirements.txt



Set up the required environment variables:

AWS_ACCESS_KEY_ID: Your AWS Access Key ID
AWS_SECRET_ACCESS_KEY: Your AWS Secret Access Key
BUCKET_NAME: The name of your AWS S3 bucket
MONGO_URI: The connection URI for your MongoDB database
EMAIL_PASS: The password for the email account used to send application emails
Run the Streamlit application:

streamlit run TenantPortal.py



Access the application in your web browser at the provided local URL.