# Sponsor-test-2

<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Redirecting...</title>
  <script>
    // List of URLs to cycle through
    const sponsors = [
      "https://www.mlb.com/",
      "https://atlanticleague.com/",
      "https://youtu.be/rMLYM_ZVu-4?si=sAvUj-oxKFcRPCV0"
    ];

    // Get the current index from localStorage (or start at -1)
    let currentIndex = parseInt(localStorage.getItem("sponsorIndex") || -1);

    // Move to the next index
    currentIndex = (currentIndex + 1) % sponsors.length;

    // Save the new index to localStorage
    localStorage.setItem("sponsorIndex", currentIndex);

    // Redirect to the new URL
    window.location.href = sponsors[currentIndex];
  </script>
</head>
<body>
  <p>Redirecting to sponsor...</p>
</body>
</html>

