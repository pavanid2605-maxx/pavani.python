# pavani.html
<!doctype html>
<html>
<head>
  <meta charset="utf-8">
  <title>Sample Form</title>
  <style>
    body { font-family: Arial; max-width: 800px; margin: 20px; }
    label { display:block; margin-top:10px; }
    fieldset { margin-top:15px; padding:10px; }
  </style>
</head>
<body>
  <h1>Registration Form (demo)</h1>

  <form action="/submit-registration" method="post" enctype="multipart/form-data">
    <fieldset>
      <legend>Personal info</legend>
      <label for="name">Full name
        <input id="name" name="name" type="text" placeholder="John Doe" required maxlength="100">
      </label>

      <label for="email">Email
        <input id="email" name="email" type="email" placeholder="you@example.com" required>
      </label>

      <label for="dob">Date of birth
        <input id="dob" name="dob" type="date" required>
      </label>
    </fieldset>

    <fieldset>
      <legend>Preferences</legend>
      <p>Choose your interests:</p>
      <label><input type="checkbox" name="interest" value="music"> Music</label>
      <label><input type="checkbox" name="interest" value="sports"> Sports</label>
      <label><input type="checkbox" name="interest" value="art"> Art</label>

      <p>Choose one subscription:</p>
      <label><input type="radio" name="plan" value="free" checked> Free</label>
      <label><input type="radio" name="plan" value="pro"> Pro</label>
    </fieldset>

    <label for="country">Country</label>
    <select id="country" name="country" required>
      <option value="">(select)</option>
      <option value="in">India</option>
      <option value="us">United States</option>
    </select>

    <label for="bio">Short bio</label>
    <textarea id="bio" name="bio" rows="4" cols="40" placeholder="Tell us briefly..."></textarea>

    <label for="photo">Upload a profile photo</label>
    <input id="photo" name="photo" type="file" accept="image/*">

    <input type="hidden" name="form_id" value="reg_2025">

    <p style="margin-top:12px;">
      <button type="submit">Register</button>
      <button type="reset">Reset</button>
    </p>
  </form>
</body>
</html>

