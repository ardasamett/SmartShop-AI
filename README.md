# Smart Shop AI
### 🛍️ AI-Powered E-Commerce Recommendation System

![](https://i.ibb.co/Hdr8v9g/Untitled-diagram-2024-10-27-193328.png)


A sophisticated recommendation system to provide personalized product recommendations based on user behavior and preferences.

## 🌟 Key Features

-  Real-time personalized product recommendations  
-  User behavior tracking and analysis  
-  Feedback collection system  
-  Rating system with visual star display  
-  Caching mechanism for improved performance  
-  Timeout handling for API requests  
-  Error handling and user feedback  
-  Responsive UI design  

##  Architecture


![](https://i.ibb.co/QvPCNvZ/Untitled-diagram-2024-10-27-202649.png)

The system is built using a modern tech stack:

### ⚙️ Backend 
- 🚀 FastAPI for the REST API  
- 🗄️ SQLAlchemy for database management  
- 🧠 Python-based ML recommendation engine  
- 🗃️ PostgreSQL database  

### 🎨 Frontend
- ⚛️ Next.js for the React framework  
- 🔧 TypeScript for type safety  
- 🎨 TailwindCSS for styling  
- 🔄 Real-time state management  

For detailed architectural information and implementation, check out our [technical blog post](https://medium.com/@sametarda.dev/building-an-ai-powered-e-commerce-recommendation-system-a-comprehensive-overview-c89613a0777d).

## 🚀 Getting Started

### 🛠️ Installation

1. **Clone the repository**  
```bash
git clone https://github.com/ardasamett/SmartShop-AI.git
cd SmartShop-AI
```

2. **Backend Setup**  
```bash
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
pip install -r requirements.txt
```

3. **Frontend Setup**  
```bash
cd UI
npm install
```

4. **Environment Configuration**  
Create `.env` files for both backend and frontend:

`.env`:
```env
DATABASE_URL=sqlite:///./ecommerce.db
GOOGLE_API_KEY=your_gemini_api_key
MODEL_NAME=gemini-1.5-flash 
```

### 🚦 Running the Application

1. **Start the Backend Server**  
```bash
uvicorn app.main:app --reload
```
API will be available at `http://localhost:8000`.

2. **Start the Frontend Development Server**  
```bash
cd UI
npm run dev
```
Frontend will be available at `http://localhost:3000`.

3. **Generate Test Data**  
Before using the application, generate test data by visiting:
```
http://localhost:8000/debug/generate-data
```
This will return a test user ID to test the application.

### 🔑 Key Endpoints

- `GET /recommendations/{user_id}` - Fetch personalized recommendations  
- `POST /feedback` - Submit recommendation feedback  
- `GET /debug/generate-data` - Generate test data  
- `GET /debug/users` - Fetch sample users  
- `GET /debug/products` - Fetch sample products  

### 🧪 Testing the Application

1. Generate test data via the `/debug/generate-data` endpoint.  
2. Copy the returned `test_user_id`.  
3. Visit `http://localhost:3000`.  
4. Enter the test user ID to see personalized recommendations.  
5. Interact with the recommendations and provide feedback.  

## 📊 System Components

1. **User Behavior Tracking**  
   - Captures user interactions  
   - Stores behavioral data for analysis  

2. **Recommendation Engine**  
   - Processes user behavior data  
   - Generates personalized recommendations  
   - Uses machine learning algorithms  

3. **Feedback System**  
   - Collects user feedback  
   - Manages ratings and reviews  
   - Ensures continuous improvement  

## 🛠️ Technical Details

### 🗂️ Database Schema  
Main tables include:  
-  Products  
-  Users  
-  UserBehavior  
-  RecommendationFeedback  

## 📈 Performance Optimizations

-  Caching mechanism for faster responses  
-  Timeout handling (10 seconds)  
-  Optimized database queries  
-  Frontend performance improvements  

## 🤝 Contributing

Contributions are welcome! Please review our contributing guidelines before submitting any pull requests.


## 📚 Additional Resources

- 📄 Detailed architecture and implementation: [Technical Blog Post](https://medium.com/@sametarda.dev/building-an-ai-powered-e-commerce-recommendation-system-a-comprehensive-overview-c89613a0777d)  
- 📖 API Documentation: Available at the `/docs` endpoint  
- 🧩 Frontend Component Documentation: Available in the UI directory  




## 📧 Contact

[LinkedIn](https://www.linkedin.com/in/ardasamet/)

