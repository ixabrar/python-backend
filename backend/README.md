# Service Hub Backend

Flask API server for the Service Hub platform.

## Setup

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Set up environment variables in `.env` file:
```
MONGO_URI=your_mongodb_connection_string
FLASK_DEBUG=True
```

3. Run the server:
```bash
python app.py
```

## API Endpoints

### Admin Endpoints
- `POST /api/admin/create-user` - Create a new user
- `GET /api/admin/users` - Get all users
- `PUT /api/admin/set-prices` - Set prices for a user

### User Endpoints
- `POST /api/auth/login` - User login
- `GET /api/user/prices/<user_id>` - Get user prices

The server runs on `http://localhost:5000`