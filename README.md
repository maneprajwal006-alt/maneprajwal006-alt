
<!-- HEADER SECTION -->
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:3b82f6,100:8b5cf6&height=250&section=header&text=Prajwal%20Mane&fontSize=70&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Computer%20Science%20Engineering%20Student&descAlignY=55&descAlign=50" alt="Header" width="100%" />

  <a href="https://github.com/maneprajwal006-alt">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&pause=1000&color=06B6D4&center=true&vCenter=true&width=600&lines=Web+Developer;Problem+Solver;Future+Full-Stack+Developer;Code+to+Learn" alt="Typing SVG" />
  </a>
</div>

<br>

<!-- PROFILE ANIMATION -->
<div align="center">
  <img src="http://googleusercontent.com/image_collection/image_retrieval/5126218280659009110" alt="Futuristic AI Coding" width="400" style="border-radius: 15px; box-shadow: 0px 4px 15px rgba(0, 255, 255, 0.3);" />
</div>

<br>

<!-- ABOUT ME SECTION -->
<h2 align="center">🚀 About Me</h2>

<table align="center" width="100%">
  <tr>
    <td width="60%" valign="top">
      <h3>Hey there! 👋</h3>
      <p>I am a passionate <strong>Computer Science Engineering</strong> student at the Ashokrao Mane Group of Institutions. I have a strong foundation in frontend development and am actively expanding my skill set to become a Full-Stack Developer. I thrive on problem-solving, building real-world architecture, and constantly learning new technologies.</p>
      <p>My core focus right now is mastering <strong>JavaScript, Node.js, and Data Structures & Algorithms</strong> to build robust, scalable applications.</p>
    </td>
    <td width="40%" valign="top">
      <h3>⚡ Quick Facts</h3>
      <ul>
        <li>🎓 <strong>Education:</strong> B.Tech CSE</li>
        <li>💻 <strong>Domain:</strong> Web Development</li>
        <li>⚡ <strong>Focus:</strong> JavaScript, Node.js</li>
        <li>⚙️ <strong>Backend:</strong> Express & REST APIs</li>
        <li>🧠 <strong>Core:</strong> DSA & Problem Solving</li>
        <li>🏆 <strong>Goal:</strong> Hackathons & Open Source</li>
      </ul>
    </td>
  </tr>
</table>

<br>

<!-- UNIQUE INTERESTS: 3D MODELING & AI -->
<h2 align="center">🎨 Beyond The Code: Creative Tech & The revised layout replaces the traditional project grid with a dynamic academic showcase, featuring CSS glassmorphism, floating animations, and placeholder slots for external images.

**Key Additions**
*   **Floating Elements:** CSS keyframe animations that create a continuous, smooth levitation effect on the main profile headers.
*   **Glassmorphism Design:** Semi-transparent, blurred card backgrounds for a modern, sleek aesthetic.
*   **Interactive Image Gallery:** Hover-triggered scaling and shadow effects to present unique interests rather than standard project lists.

**HTML & CSS Implementation**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Profile</title>
    <style>
        body {
            margin: 0;
            font-family: system-ui, sans-serif;
            background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
            color: white;
            overflow-x: hidden;
        }

        /* Floating Animation */
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }

        .hero-section {
            text-align: center;
            padding: 100px 20px 40px;
            animation: float 4s ease-in-out infinite;
        }

        .hero-section h1 {
            font-size: 3rem;
            background: -webkit-linear-gradient(#4facfe, #00f2fe);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* Glassmorphism Gallery (Replaces Projects) */
        .gallery-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
            padding: 20px 50px 80px;
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            width: 320px;
            transition: transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275), box-shadow 0.4s ease;
            cursor: pointer;
        }

        .glass-card:hover {
            transform: translateY(-10px) scale(1.03);
            box-shadow: 0 20px 40px rgba(0,0,0,0.4);
        }

        .glass-card img {
            width: 100%;
            border-radius: 10px;
            height: 220px;
            object-fit: cover;
            transition: filter 0.3s ease;
            filter: grayscale(20%);
        }
