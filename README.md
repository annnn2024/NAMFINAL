# NAMFINAL
TELEHEALTH WEB
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CARE.CONNECT</title>
    <style>
        /* General Body Styling */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f3f4f7; /* Light Background */
            color: #333;
        }
        
        /* Header */
        header {
            background: linear-gradient(to right, #FF7E5F, #FEB47B); /* Gradient colors */
            color: white;
            text-align: center;
            padding: 50px 20px;
            font-size: 36px;
            font-weight: bold;
            border-bottom: 3px solid #FF5F6D;
        }
        
        /* Container for Sections */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Section Title */
        h2, h3 {
            color: #4CAF50;
            text-align: center;
            margin-bottom: 20px;
        }
        
        /* Section Styling */
        section {
            padding: 40px;
            margin: 20px 0;
            border-radius: 8px;
            background-color: #ffffff;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }
        
        /* Button Styling */
        .button {
            background-color: #81C784;
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 18px;
            transition: background-color 0.3s ease;
            display: inline-block;
            text-align: center;
            margin-top: 15px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        /* Button Hover Effect */
        .button:hover {
            background-color: #66BB6A;
        }

        /* Feature Box Styling */
        .feature-box {
            background-color: #fff;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            margin-bottom: 30px;
        }

        /* AI Feature Box */
        .ai-feature {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            margin-top: 30px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.05);
        }

        .ai-feature input,
        .ai-feature textarea {
            width: 100%;
            padding: 12px;
            border-radius: 8px;
            border: 2px solid #81C784;
            margin-top: 10px;
            margin-bottom: 10px;
        }

        .ai-feature button {
            background-color: #FF7E5F;
            color: white;
            padding: 12px 24px;
            border-radius: 8px;
            border: none;
            font-size: 16px;
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .ai-feature button:hover {
            background-color: #FF5F6D;
        }

        /* Footer */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 15px;
            font-size: 16px;
        }

        /* Responsive Media Queries */
        @media only screen and (max-width: 768px) {
            header {
                font-size: 28px;
                padding: 30px 20px;
            }
            .container {
                padding: 10px;
            }
            .feature-box {
                padding: 20px;
            }
            .button {
                padding: 12px 25px;
            }
        }
    </style>
</head>
<body>

<!-- Header -->
<header>
    <h1>WELCOME TO CARE.CONNECT</h1>
</header>

<!-- Container for Main Content -->
<div class="container">

    <!-- Introduction Section -->
    <section id="intro">
        <h2>Welcome to the Future of Telehealth</h2>
        <p>CARE.CONNECT is an AI-powered telehealth platform designed to offer seamless and accessible healthcare to all, leveraging digital communication, remote monitoring, and virtual consultations.</p>
        <p>Our platform ensures that you can connect with healthcare providers from anywhere and receive personalized care. It is time to take control of your health with advanced tools that bridge the gap between patients and doctors.</p>

        <div class="feature-box">
            <h3>Explore Our Services</h3>
            <button class="button" onclick="window.location.href='#about-us'">About Us</button>
        </div>
        <div class="feature-box">
            <h3>Patient Information</h3>
            <button class="button" onclick="window.location.href='#patient-info'">Enter Patient Info</button>
        </div>
        <div class="feature-box">
            <h3>Get Your E-Prescription</h3>
            <button class="button" onclick="window.location.href='#prescription'">E-Prescription</button>
        </div>

        <div class="ai-feature">
            <h3>AI Symptom Checker</h3>
            <input type="text" id="symptom-input" placeholder="Enter your symptoms...">
            <button class="button" onclick="checkSymptoms()">Check Symptoms</button>
            <p id="symptom-result"></p>
        </div>

        <div class="ai-feature">
            <h3>AI Medical Assistant</h3>
            <textarea id="assistant-input" placeholder="Ask your medical question..."></textarea>
            <button class="button" onclick="getMedicalAdvice()">Get Advice</button>
            <p id="assistant-result"></p>
        </div>
    </section>

    <!-- Vitals Monitoring Section (New Page) -->
    <section id="vitals-monitoring">
        <h2>Vitals Monitoring</h2>
        <p>Track your vitals such as blood pressure and heart rate in real-time. This feature helps monitor your health and ensures early detection of any health issues.</p>
        
        <form>
            <label for="bp">Blood Pressure:</label><br>
            <input type="text" id="bp" name="bp" placeholder="Enter your blood pressure"><br><br>

            <label for="heartRate">Heart Rate:</label><br>
            <input type="text" id="heartRate" name="heartRate" placeholder="Enter your heart rate"><br><br>

            <button class="button" onclick="alert('Vitals Saved')">Save Vitals</button><br><br>
        </form>
    </section>

    <!-- About Us Section -->
    <section id="about-us">
        <h2>About Us</h2>
        <p>At CARE.CONNECT, we are committed to improving the healthcare experience for everyone. Our platform integrates AI and telemedicine technologies to connect patients with top doctors from around the world, ensuring high-quality and accessible healthcare services.</p>
        <h3>Meet Our Top Doctors:</h3>
        <ul>
            <li><strong>Dr. John Doe</strong> - Cardiologist <br>Email: johndoe@careconnect.com</li>
            <li><strong>Dr. Jane Smith</strong> - Neurologist <br>Email: janesmith@careconnect.com</li>
            <li><strong>Dr. Emily Davis</strong> - General Practitioner <br>Email: emilydavis@careconnect.com</li>
        </ul>
        <button class="button" onclick="window.location.href='#patient-info'">Proceed to Patient Info</button>
    </section>

    <!-- Patient Information Section -->
    <section id="patient-info">
        <h2>Patient Information</h2>
        <form>
            <label for="username">Username:</label><br>
            <input type="text" id="username" name="username"><br><br>

            <label for="contact">Contact Number:</label><br>
            <input type="text" id="contact" name="contact"><br><br>

           
            <label for="history">History of Illness:</label><br>
            <textarea id="history" name="history"></textarea><br><br>

            <button class="button" onclick="alert('Consultation Started')">Consult Now</button><br><br>
            <button class="button" onclick="alert('Emergency Signal Sent')">Send Emergency Signal</button>
        </form>
    </section>

    <!-- E-Prescription Page -->
    <section id="prescription">
        <h2>E-Prescription</h2>
        <p>Choose your preferred payment method to process your prescription:</p>
        <form>
            <label for="payment-method">Choose Payment Method:</label><br>
            <select id="payment-method" name="payment-method">
                <option value="credit-card">Credit Card</option>
                <option value="paypal">PayPal</option>
                <option value="bank-transfer">Bank Transfer</option>
            </select><br><br>
            <button class="button" onclick="alert('Payment Successful')">Pay Now</button>
        </form>
        <button class="button" onclick="window.location.href='#thank-you'">Go to Thank You Page</button>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 CARE.CONNECT | All Rights Reserved</p>
    </footer>
</div>

<script>
    // Simulate AI-based Symptom Checker
    function checkSymptoms() {
        var symptom = document.getElementById('symptom-input').value.toLowerCase();
        var result = '';
        if (symptom.includes('headache')) {
            result = 'You may be experiencing a migraine or tension headache. Consider drinking water, resting, or consulting a doctor if symptoms persist.';
        } else if (symptom.includes('fever')) {
            result = 'A fever could indicate an infection or viral illness. If it continues for more than 3 days or reaches over 102°F, seek medical attention.';
        } else if (symptom.includes('cough')) {
            result = 'A cough could be due to various factors like a cold, flu, or allergies. If it lasts more than two weeks, consider seeing a doctor.';
        } else {
            result = 'Symptom not recognized. Please enter more detailed symptoms or consult a healthcare provider for personalized advice.';
        }
        document.getElementById('symptom-result').innerText = result;
    }

    // Simulate AI Medical Assistant
    function getMedicalAdvice() {
        var question = document.getElementById('assistant-input').value.toLowerCase();
        var response = '';

        if (question.includes('cough')) {
            response = 'A cough could be caused by allergies, viral infections, or a common cold. Try drinking warm fluids, using a humidifier, or seeing a doctor if the cough persists for more than two weeks.';
        } else if (question.includes('headache')) {
            response = 'Headaches can be caused by stress, dehydration, or lack of sleep. Ensure you’re hydrated, try relaxing, and get sufficient rest. If your headaches are chronic, consult a doctor.';
        } else {
            response = 'I\'m sorry, I can only provide advice based on common symptoms. For specific concerns, please consult with a doctor.';
        }

        document.getElementById('assistant-result').innerText = response;
    }
</script>

</body>
</html>
