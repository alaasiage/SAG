# SAG
Client scheduling portal for SAG. Securely request or book professional tax and accounting consultation appointments.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Request an Appointment</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            padding: 40px;
        }
        .booking-card {
            max-width: 450px;
            margin: 0 auto;
            background: #fff;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        label { display: block; margin-top: 15px; font-weight: bold; color: #444; }
        input, select, textarea {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
        }
        button {
            width: 100%;
            background-color: #007bff;
            color: white;
            padding: 12px;
            border: none;
            border-radius: 4px;
            margin-top: 20px;
            font-size: 16px;
            cursor: pointer;
        }
        button:hover { background-color: #0056b3; }
    </style>
</head>
<body>

    <div class="booking-card">
        <h2>Book a Meeting</h2>
        <!-- Sign up at Formspree.io to get a unique action URL -->
        <form action="https://formspree.io" method="POST">
            <label for="name">Your Name</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Email Address</label>
            <input type="email" id="email" name="email" required>

            <label for="date">Preferred Date</label>
            <input type="date" id="date" name="date" required>

            <label for="time">Preferred Time</label>
            <select id="time" name="time" required>
                <option value="09:00">09:00 AM</option>
                <option value="10:30">10:30 AM</option>
                <option value="13:00">01:00 PM</option>
                <option value="15:30">03:30 PM</option>
            </select>

            <label for="notes">Meeting Notes</label>
            <textarea id="notes" name="notes" rows="3" placeholder="What should we discuss?"></textarea>

            <button type="submit">Submit Request</button>
        </form>
    </div>

</body>
</html>
