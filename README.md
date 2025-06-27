
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>The Village School System</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
  <style>
    html { scroll-behavior: smooth; }
    body { background-color: #1f2937; }
    .btn-primary {
      background-color: #2563eb;
      color: white;
      padding: 0.5rem 1.5rem;
      border-radius: 9999px;
      transition: all 0.3s ease;
    }
    .btn-primary:hover { background-color: #1e40af; }
    .classy-table th, .classy-table td {
      border: 1px solid #4b5563;
      padding: 12px;
    }
    .classy-table {
      border-collapse: collapse;
      width: 100%;
      background-color: #2d3748;
      color: #f9fafb;
      border-radius: 8px;
    }
  </style>
</head>
<body class="font-sans text-gray-100">

  <!-- Navbar -->
  <nav class="bg-gray-800 p-4 fixed top-0 w-full z-50 shadow-md">
    <div class="max-w-7xl mx-auto flex justify-center gap-4 text-white text-sm md:text-base">
      <a href="#home" class="hover:text-blue-400">Home</a>
      <a href="#about" class="hover:text-blue-400">About</a>
      <a href="#datesheet" class="hover:text-blue-400">Datesheet</a>
      <a href="#fee" class="hover:text-blue-400">Fee</a>
      <a href="#syllabus" class="hover:text-blue-400">Syllabus</a>
      <a href="#contact" class="hover:text-blue-400">Contact</a>
      <a href="#apply" class="hover:text-blue-400">Apply</a>
    </div>
  </nav>

  <!-- Home -->
  <section id="home" class="py-24 px-6 text-center bg-gray-900" data-aos="fade-up">
    <h1 class="text-5xl font-bold mb-4">The Village School System</h1>
    <p class="text-lg mb-4">The Right & Easy Way to Learn</p>
    <p class="text-gray-300 max-w-2xl mx-auto">Welcome to a place where education meets innovation. We nurture young minds with love, discipline, and creativity from Class 1 to 8.</p>
  </section>

  <!-- About Us -->
  <section id="about" class="py-16 px-6 bg-gray-800 text-center" data-aos="fade-up">
    <h2 class="text-3xl font-bold mb-4">About Us</h2>
    <p class="max-w-3xl mx-auto">TVSS is committed to providing quality education through a modern, interactive approach. Our aim is to make learning accessible and joyful for all students. Our staff is trained to nurture every child’s potential.</p>
  </section>

  <!-- Datesheet -->
  <section id="datesheet" class="py-16 px-6 bg-gray-900 text-center" data-aos="fade-up">
    <h2 class="text-3xl font-bold mb-6">Datesheet</h2>
    <div class="flex flex-col md:flex-row gap-4 justify-center">
      <select id="datesheet-class" class="p-2 rounded text-black">
        <option value="">Select Class</option>
        <option value="1">Class 1</option><option value="2">Class 2</option>
        <option value="3">Class 3</option><option value="4">Class 4</option>
        <option value="5">Class 5</option><option value="6">Class 6</option>
        <option value="7">Class 7</option><option value="8">Class 8</option>
      </select>
      <select id="datesheet-term" class="p-2 rounded text-black">
        <option value="">Select Term</option>
        <option value="mid">Mid Term</option>
        <option value="final">Final Term</option>
      </select>
    </div>
    <div id="datesheet-output" class="mt-6 text-left max-w-xl mx-auto"></div>
  </section>
  <!-- Fee Structure -->
  <section id="fee" class="py-16 px-6 bg-gray-800 text-center" data-aos="fade-up">
    <h2 class="text-3xl font-bold mb-6">Fee Structure</h2>
    <select id="fee-class" class="p-2 rounded text-black">
      <option value="">Select Class</option>
      <option value="1">Class 1</option><option value="2">Class 2</option>
      <option value="3">Class 3</option><option value="4">Class 4</option>
      <option value="5">Class 5</option><option value="6">Class 6</option>
      <option value="7">Class 7</option><option value="8">Class 8</option>
    </select>
    <div id="fee-output" class="mt-6"></div>
  </section>

  <!-- Syllabus -->
  <section id="syllabus" class="py-16 px-6 bg-gray-900 text-center" data-aos="fade-up">
    <h2 class="text-3xl font-bold mb-6">Syllabus</h2>
    <div class="flex flex-col md:flex-row gap-4 justify-center">
      <select id="syllabus-class" class="p-2 rounded text-black">
        <option value="">Select Class</option>
        <option value="1">Class 1</option><option value="2">Class 2</option>
        <option value="3">Class 3</option><option value="4">Class 4</option>
        <option value="5">Class 5</option><option value="6">Class 6</option>
        <option value="7">Class 7</option><option value="8">Class 8</option>
      </select>
      <select id="syllabus-term" class="p-2 rounded text-black">
        <option value="">Select Term</option>
        <option value="mid">Mid Term</option>
        <option value="final">Final Term</option>
      </select>
    </div>
    <div id="syllabus-output" class="mt-6 text-left max-w-xl mx-auto"></div>
  </section>

  <!-- Contact -->
  <section id="contact" class="py-16 px-6 bg-gray-800 text-center" data-aos="fade-up">
    <h2 class="text-3xl font-bold mb-6">Contact Us</h2>
    <form class="space-y-4 max-w-xl mx-auto">
      <input type="text" placeholder="Name" class="w-full p-2 rounded text-black" required />
      <input type="email" placeholder="Email" class="w-full p-2 rounded text-black" required />
      <input type="tel" placeholder="WhatsApp Number" class="w-full p-2 rounded text-black" required />
      <textarea placeholder="Your Message" class="w-full p-2 rounded text-black" required></textarea>
      <button class="btn-primary w-full">Send Message</button>
    </form>
  </section>
  <!-- Apply Now -->
  <section id="apply" class="py-16 px-6 bg-gray-900 text-center" data-aos="fade-up">
    <h2 class="text-3xl font-bold mb-6">Apply Now</h2>
    <form id="applyForm" class="space-y-4 max-w-xl mx-auto">
      <input required type="text" placeholder="Student Name" class="w-full p-2 rounded text-black" />
      <input required type="text" placeholder="Father's Name" class="w-full p-2 rounded text-black" />
      <input required type="number" min="1" max="8" placeholder="Class" class="w-full p-2 rounded text-black" />
      <input required type="tel" placeholder="Contact Number" class="w-full p-2 rounded text-black" />
      <input required type="email" placeholder="Email Address" class="w-full p-2 rounded text-black" />
      <textarea required placeholder="Why TVSS?" class="w-full p-2 rounded text-black"></textarea>
      <button class="btn-primary w-full">Submit Application</button>
      <p id="formMessage" class="text-green-400 hidden">Form submitted!</p>
    </form>
  </section>

  <!-- Scripts -->
  <script>
    const datesheets = {
      1: { mid: 'Math: 10 July', final: 'Math: 5 Dec' },
      2: { mid: 'Eng: 11 July', final: 'Eng: 6 Dec' },
      3: { mid: 'Urdu: 12 July', final: 'Urdu: 7 Dec' },
      4: { mid: 'Sci: 13 July', final: 'Sci: 8 Dec' },
      5: { mid: 'Hist: 14 July', final: 'Hist: 9 Dec' },
      6: { mid: 'Comp: 15 July', final: 'Comp: 10 Dec' },
      7: { mid: 'Geo: 16 July', final: 'Geo: 11 Dec' },
      8: { mid: 'Bio: 17 July', final: 'Bio: 12 Dec' }
    };
    const fees = {
      1: 1000, 2: 1100, 3: 1200, 4: 1300,
      5: 1400, 6: 1500, 7: 1600, 8: 1700
    };
    const syllabus = {
      1: { mid: ['ABC', '1-10'], final: ['Words', '10-20'] },
      2: { mid: ['Eng', 'Add'], final: ['Sentences', 'Subtract'] },
      3: { mid: ['Urdu', 'Tables'], final: ['Dictation', 'Shapes'] },
      4: { mid: ['Islamiyat', 'Div'], final: ['History', 'Fractions'] },
      5: { mid: ['Sci', 'Data'], final: ['Charts', 'Analysis'] },
      6: { mid: ['Essay', 'Decimal'], final: ['Report', 'Geometry'] },
      7: { mid: ['Computer', 'Bio'], final: ['ICT', 'Chem'] },
      8: { mid: ['Physics', 'Math'], final: ['Theory', 'Experiments'] }
    };

    document.getElementById('datesheet-class').addEventListener('change', showDatesheet);
    document.getElementById('datesheet-term').addEventListener('change', showDatesheet);
    function showDatesheet() {
      const cls = document.getElementById('datesheet-class').value;
      const term = document.getElementById('datesheet-term').value;
      const data = datesheets[cls]?.[term];
      document.getElementById('datesheet-output').innerHTML = data ? `<p>${data}</p>` : '';
    }

    document.getElementById('fee-class').addEventListener('change', function () {
      const cls = this.value;
      const fee = fees[cls];
      document.getElementById('fee-output').innerHTML = fee
        ? `<table class="classy-table mt-4 mx-auto"><tr><th>Class</th><th>Monthly Fee</th></tr><tr><td>${cls}</td><td>PKR ${fee}</td></tr></table>`
        : '';
    });

    document.getElementById('syllabus-class').addEventListener('change', showSyllabus);
    document.getElementById('syllabus-term').addEventListener('change', showSyllabus);
    function showSyllabus() {
      const cls = document.getElementById('syllabus-class').value;
      const term = document.getElementById('syllabus-term').value;
      const list = syllabus[cls]?.[term];
      document.getElementById('syllabus-output').innerHTML = list ? `<ul class="list-disc pl-6">${list.map(x => `<li>${x}</li>`).join('')}</ul>` : '';
    }

    document.getElementById('applyForm').addEventListener('submit', function(e) {
      e.preventDefault();
      document.getElementById('formMessage').classList.remove('hidden');
      this.reset();
    });
  </script>
  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script>AOS.init();</script>
</body>
</html>
