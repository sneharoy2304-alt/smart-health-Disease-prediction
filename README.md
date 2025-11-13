# 🏥 Smart Health Disease Prediction System

A comprehensive, AI-powered web application for predicting heart diseases using advanced Machine Learning algorithms.

## 🎯 Overview

The Smart Health Disease Prediction System uses a Random Forest ML model to predict heart disease based on 13 key health parameters with 85%+ accuracy. Built with FastAPI, React, and MongoDB.

## ✨ Key Features

- ✅ AI-powered heart disease prediction (85%+ accuracy)
- ✅ Role-based access (Admin, Doctor, Patient)
- ✅ Doctor recommendations for at-risk patients
- ✅ Prediction history tracking
- ✅ Real-time analytics dashboard
- ✅ Modern responsive UI with Tailwind CSS
- ✅ Secure JWT authentication

## 🚀 Quick Start

### Access the Application

The application is already running! Access it at your deployment URL.

### Default Login Credentials

**Admin Account:**
- Username: `admin`
- Password: `admin123`

**Sample Doctors** (Password: `doctor123`):
- dr.sarah, dr.michael, dr.emily, dr.david, dr.lisa

## 👥 User Roles

### Patient 🩺
- Register & create health profile
- Get heart disease predictions
- View prediction history
- Access recommended doctors
- Submit feedback

### Doctor 👨‍⚕️
- View patient predictions
- Review health analytics
- Monitor at-risk patients

### Admin 🔧
- Manage doctors
- View system statistics
- Access all predictions
- Review feedback

## 📊 How to Use

### For Patients:

1. **Register**: Go to Register page and create an account
2. **Login**: Sign in with your credentials
3. **Predict**: Click "Predict Disease" and enter 13 health parameters:
   - Age, Sex, Chest Pain Type
   - Blood Pressure, Cholesterol
   - Blood Sugar, ECG Results
   - Heart Rate, Exercise Data
   - And more...
4. **View Results**: Get instant prediction with accuracy score
5. **Consult Doctors**: View recommended cardiologists if at risk

### For Doctors:

1. **Register**: Create doctor account (awaits admin approval)
2. **Login**: Access after admin approval
3. **Dashboard**: View all patient predictions and analytics

### For Admin:

1. **Login**: Use admin credentials
2. **Manage**: Add/approve/delete doctors
3. **Monitor**: View system statistics and user feedback

## 🏗️ Tech Stack

**Backend:**
- FastAPI (Python)
- MongoDB (Motor async)
- scikit-learn (ML)
- JWT Authentication

**Frontend:**
- React 19
- Tailwind CSS
- Axios
- React Router v7

## 📝 API Documentation

Access interactive API docs at: `/docs` (Swagger UI)

### Key Endpoints:

- `POST /api/auth/login` - User login
- `POST /api/auth/register` - User registration
- `POST /api/predict` - Make prediction
- `GET /api/doctors/approved` - Get approved doctors
- `GET /api/predictions` - Get prediction history

## 🔐 Security

- JWT token authentication
- Bcrypt password hashing
- Role-based access control
- Input validation with Pydantic
- CORS configuration

## 📦 Project Structure

```
/app/
├── backend/              # FastAPI server
│   ├── server.py        # Main application
│   ├── models.py        # Data models
│   ├── auth.py          # Authentication
│   ├── ml_model.py      # ML prediction model
│   └── requirements.txt
│
└── frontend/            # React application
    ├── src/
    │   ├── App.js
    │   ├── components/  # Navbar, Footer
    │   ├── pages/       # All pages
    │   ├── context/     # Auth context
    │   └── utils/       # API utilities
    └── package.json
```

## 🎨 Screenshots & Features

### Landing Page
- Modern hero section
- Feature highlights
- How it works guide
- Call-to-action buttons

### Patient Dashboard
- Prediction history
- Health statistics
- Quick prediction access
- Doctor recommendations

### Admin Dashboard
- System statistics
- Doctor management
- Patient list
- Feedback review

## 🧪 ML Model Details

**Random Forest Classifier:**
- 100 decision trees
- Max depth: 10
- Training accuracy: ~85%
- 13 input features
- Binary output (Healthy/At Risk)

## 🛠️ Restart Services

If needed, restart the application:

```bash
# Restart all services
sudo supervisorctl restart all

# Check status
sudo supervisorctl status

# View logs
tail -f /var/log/supervisor/backend.out.log
tail -f /var/log/supervisor/frontend.out.log
```

## ⚠️ Important Notes

1. **Medical Disclaimer**: This is an educational project. Always consult qualified healthcare professionals for medical advice.

2. **Demo Data**: The system includes 5 sample doctors for demonstration purposes.

3. **Prediction Accuracy**: The ML model achieves ~85% accuracy on test data.

## 📞 Support & Credits

**Developer**: Suraj Chadha (2210987034)
**Organization**: ThinkNEXT Technologies Private Limited
**Program**: 6-Month Industrial Training (AI, ML, Deep Learning)
**Institution**: Chitkara University

**Mentors:**
- Manpreet Kaur (Python Trainer & Developer)
- Dr. Ruchi Mittal (Professor, Computer Applications)

---

**Built with ❤️ using FastAPI, React, and Machine Learning**

**For medical emergencies, call 911 immediately!**
