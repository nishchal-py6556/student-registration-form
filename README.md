
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Student Registration Form</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  <style>
    * {
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #1f4037, #99f2c8);
      color: #2c3e50;
    }

    .container {
      max-width: 850px;
      background: white;
      margin: 40px auto;
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 12px 30px rgba(0, 0, 0, 0.2);
      transition: 0.3s;
    }

    h2 {
      text-align: center;
      color: #1abc9c;
      margin-bottom: 30px;
      font-size: 32px;
    }

    .form-group {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      margin-bottom: 20px;
    }

    .form-group > div {
      flex: 1 1 45%;
    }

    label {
      font-weight: bold;
      display: block;
      margin-bottom: 6px;
    }

    input[type="text"],
    input[type="email"],
    input[type="date"],
    input[type="file"],
    textarea,
    select {
      width: 100%;
      padding: 12px;
      border: 2px solid #ecf0f1;
      border-radius: 10px;
      outline: none;
      transition: 0.3s;
    }

    input:focus, textarea:focus, select:focus {
      border-color: #1abc9c;
      box-shadow: 0 0 8px rgba(26, 188, 156, 0.3);
    }

    .radio-group {
      margin-top: 10px;
    }

    .radio-group label {
      margin-right: 20px;
      font-weight: normal;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 10px;
    }

    table th, table td {
      padding: 12px;
      text-align: center;
      border: 1px solid #ccc;
    }

    textarea {
      resize: vertical;
      min-height: 100px;
    }

    .btn-group {
      text-align: center;
      margin-top: 30px;
    }

    .btn-group button {
      background-color: #1abc9c;
      color: white;
      border: none;
      padding: 12px 25px;
      margin: 10px;
      font-size: 16px;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s;
    }

    .btn-group button:hover {
      background-color: #16a085;
    }

    .icon-label i {
      margin-right: 8px;
      color: #16a085;
    }

    @media (max-width: 768px) {
      .form-group > div {
        flex: 1 1 100%;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h2><i class="fa-solid fa-user-graduate"></i> Student Registration Form</h2>
    <form>
      <div class="form-group">
        <div>
          <label class="icon-label"><i class="fa fa-user"></i> First Name:</label>
          <input type="text" placeholder="e.g. Nishchal">
        </div>
        <div>
          <label class="icon-label"><i class="fa fa-user"></i> Last Name:</label>
          <input type="text" placeholder="e.g. Sharma">
        </div>
      </div>

      <div class="form-group">
        <div>
          <label class="icon-label"><i class="fa fa-envelope"></i> Email:</label>
          <input type="email" placeholder="example@mail.com">
        </div>
        <div>
          <label class="icon-label"><i class="fa fa-phone"></i> Phone Number:</label>
          <input type="text" placeholder="10-digit number">
        </div>
      </div>

      <div class="form-group">
        <div>
          <label class="icon-label"><i class="fa fa-globe"></i> Country:</label>
          <input type="text" value="Nepal">
        </div>
        <div>
          <label class="icon-label"><i class="fa fa-location-dot"></i> Address:</label>
          <input type="text" placeholder="e.g. Kathmandu">
        </div>
      </div>

      <div class="form-group">
        <div>
          <label class="icon-label"><i class="fa fa-calendar"></i> Date of Birth:</label>
          <input type="date">
        </div>
        <div>
          <label class="icon-label"><i class="fa fa-user-tie"></i> Father's Name:</label>
          <input type="text">
        </div>
      </div>

      <div class="form-group">
        <div>
          <label class="icon-label"><i class="fa fa-user-tie"></i> Mother's Name:</label>
          <input type="text">
        </div>
        <div>
          <label class="icon-label"><i class="fa fa-venus-mars"></i> Gender:</label>
          <div class="radio-group">
            <label><input type="radio" name="gender"> Male</label>
            <label><input type="radio" name="gender"> Female</label>
            <label><input type="radio" name="gender"> Other</label>
          </div>
        </div>
      </div>

      <div class="form-group">
        <div>
          <label class="icon-label"><i class="fa fa-book"></i> Course:</label>
          <select>
            <option>Science</option>
            <option>Management</option>
            <option>Humanities</option>
            <option>Law</option>
          </select>
        </div>
        <div>
          <label class="icon-label"><i class="fa fa-upload"></i> Upload Photo:</label>
          <input type="file">
        </div>
      </div>

      <label class="icon-label"><i class="fa fa-graduation-cap"></i> Qualification:</label>
      <table>
        <tr>
          <th>SL No</th>
          <th>Examination</th>
          <th>Board</th>
          <th>Percentage</th>
          <th>Year</th>
        </tr>
        <tr>
          <td>1</td>
          <td>Class X</td>
          <td><input type="text"></td>
          <td><input type="text"></td>
          <td><input type="text"></td>
        </tr>
        <tr>
          <td>2</td>
          <td>Class VIII</td>
          <td><input type="text"></td>
          <td><input type="text"></td>
          <td><input type="text"></td>
        </tr>
      </table>

      <label class="icon-label"><i class="fa fa-comment"></i> About Yourself:</label>
      <textarea placeholder="Tell us something about yourself..."></textarea>

      <div class="btn-group">
        <button type="submit"><i class="fa fa-paper-plane"></i> Submit</button>
        <button type="reset"><i class="fa fa-eraser"></i> Reset</button>
      </div>
    </form>
  </div>
</body>
</html>
