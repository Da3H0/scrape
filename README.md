# FloodPath Water Level API

This is a Flask-based API that scrapes and provides water level data from PAGASA.

## Deployment Instructions

### Deploying to Render.com

1. Create a free account on [Render.com](https://render.com)
2. Click "New +" and select "Web Service"
3. Connect your GitHub repository
4. Configure the deployment:
   - Name: floodpath-api (or your preferred name)
   - Environment: Python
   - Build Command: `pip install -r requirements.txt`
   - Start Command: `gunicorn app:app`
   - Plan: Free

5. Click "Create Web Service"

The service will be automatically deployed and you'll get a URL like `https://your-app-name.onrender.com`

### API Endpoints

- GET `/water-level`: Returns the latest water level data from PAGASA stations

### Local Development

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Run the application:
```bash
python app.py
```

The API will be available at `http://localhost:10000` (or the port you set) 