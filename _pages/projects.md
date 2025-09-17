---
title: "Projects"
permalink: /projects/
layout: single
author_profile: true
---

Here are some of the projects I’ve worked on:
---

## 🎮 Game Review App
A full-stack mobile application that allows users to post, browse, and engage with game reviews in an interactive way. Built with a focus on smooth navigation, dynamic content, and engaging UI/UX.
- Developed using **React Native, Redux, and REST APIs**
- Supports user-generated reviews, fetching external data, and real-time updates

<div class="carousel-container">
  <button class="prev" onclick="moveSlide(this, -1)">❮</button>
  <div class="carousel-slide">
    <img src="/assets/gameapp.png" alt="Game Review App Screenshot">
    <img src="/assets/gameapp-1.png" alt="Game Review App Screenshot 1">
    <img src="/assets/gameapp-2.png" alt="Game Review App Screenshot 2">
    <img src="/assets/gameapp-3.png" alt="Game Review App Screenshot 3">
    <img src="/assets/gameapp-4.png" alt="Game Review App Screenshot 4">
    <img src="/assets/gameapp-5.png" alt="Game Review App Screenshot 5">
    <img src="/assets/gameapp-6.png" alt="Game Review App Screenshot 6">
  </div>
  <button class="next" onclick="moveSlide(this, 1)">❯</button>
</div>

### Features
- Browse Reviews: Explore user-submitted reviews of different games.
- Post Reviews: Add personal game reviews with title, rating, and description.
- Adaptive UI: Stunning responsive design for iOS and Android.
- Smooth Navigation: Implemented with React Navigation for seamless flow.
- State Management: Robust data handling using Redux and Context API.
- Dynamic Content: Integrated REST APIs for fetching external game data.

### Technologies
React Native | Redux | REST APIs | JavaScript  

<a href="https://github.com/Saiyukta/CriticShare" target="_blank"> 📂 View Code on GitHub </a> 

---

## 🏛️ Museum Artefacts Website
A responsive web application that allows users to explore and learn about museum artefacts, built with a focus on usability, functionality, and interactive design.
- Developed using **HTML, CSS, PHP, and MySQL**
- Allows users to explore and learn about artefacts with a clean and responsive design  

<div class="carousel-container">
  <button class="prev" onclick="moveSlide(this, -1)">❮</button>
  <div class="carousel-slide">
    <img src="/assets/muesem.png" alt="Museum Screenshot">
    <img src="/assets/museum-1.png" alt="Museum Screenshot 1">
    <img src="/assets/museum-2.png" alt="Museum Screenshot 2">
    <img src="/assets/museum-3.png" alt="Museum Screenshot 4">
    <img src="/assets/museum-4.png" alt="Museum Screenshot 4">
    <img src="/assets/museum-5.png" alt="Museum Screenshot 5">
    <img src="/assets/museum-6.png" alt="Museum Screenshot 6">
    <img src="/assets/museum-7.png" alt="Museum Screenshot 7">
  </div>
  <button class="next" onclick="moveSlide(this, 1)">❯</button>
</div>

### Features
- Browse artefacts by category or search keywords
- View detailed artefact pages with images and descriptions
- Admin panel with full CRUD functionality for managing artefacts
- User authentication for secure admin access (login/logout)
- Responsive design for desktop, tablet, and mobile

### Technologies
HTML | CSS | JavaScript | PHP | MySQL

 <a href="https://github.com/Saiyukta/MuseumArtefactsWebsite" target="_blank"> 📂 View Code on GitHub </a> |  <a href="/assets/Museum_Report.pdf" download>Download Report</a>

---

## 🎭 Musical Ticket Booking GUI
A web-based ticket booking system designed to provide users with a seamless and interactive experience for browsing musicals, checking schedules, and booking tickets.
- Developed using **Java, NetBeans, PHP, and MySQL**
- Allows users to explore musicals list, view show dates & times, and book tickets  

<div class="carousel-container">
  <button class="prev" onclick="moveSlide(this, -1)">❮</button>
  <div class="carousel-slide">
    <img src="/assets/musical.png" alt="Ticket Screenshot">
    <img src="/assets/musical-1.png" alt="Ticket Screenshot 1">
    <img src="/assets/musical-2.png" alt="Ticket Screenshot 2">
    <img src="/assets/musical-3.png" alt="Ticket Screenshot 3">
    <img src="/assets/musical-4.png" alt="Ticket Screenshot 4">
    <img src="/assets/musical-5.png" alt="Ticket Screenshot 5">
    <img src="/assets/musical-6.png" alt="Ticket Screenshot 6">
  </div>
  <button class="next" onclick="moveSlide(this, 1)">❯</button>
</div>

### Features
- Browse Musicals: View available shows with descriptions and details.
- Schedule Display: Check show timings and venues.
- Ticket Booking: Select ticket types (adult, senior, student) and quantities.
- Receipt Generation: Automatically generates a booking confirmation or receipt.
- Dynamic Schedule Management: Admin can add, update, or remove shows.
- User-Friendly GUI: Intuitive interface for smooth navigation.
- Future-Ready: Designed to support online payments and advanced authentication.

### Technologies
Java | NetBeans | PHP | MySQL  

<a href="https://github.com/Saiyukta/LondonMusicalTicketSystem" target="_blank"> 📂 View Code on GitHub </a> |  <a href="/assets/Musical_GUI_Report.pdf" download>Download Report</a>

---

<!-- Carousel Styles -->
<style>
.carousel-container {
  position: relative;
  width: 90%;
  margin: 20px auto;
  overflow: hidden;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.2);
}
.carousel-slide {
  display: flex;
  transition: transform 0.5s ease-in-out;
}
.carousel-slide img {
  width: 100%;
  border-radius: 12px;
  flex-shrink: 0;
}
.prev, .next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background-color: rgba(0,0,0,0.5);
  color: white;
  border: none;
  font-size: 24px;
  padding: 8px 12px;
  cursor: pointer;
  border-radius: 50%;
  z-index: 10;
}
.prev { left: 10px; }
.next { right: 10px; }
</style>

<!-- Carousel Script -->
<script>
function moveSlide(button, direction) {
  const container = button.closest('.carousel-container');
  const slide = container.querySelector('.carousel-slide');
  const images = slide.querySelectorAll('img');
  const slideWidth = images[0].clientWidth;

  // track current index
  if (!container.currentIndex) container.currentIndex = 0;

  container.currentIndex += direction;

  if (container.currentIndex < 0) {
    container.currentIndex = images.length - 1;
  } else if (container.currentIndex >= images.length) {
    container.currentIndex = 0;
  }

  slide.style.transform = `translateX(${-slideWidth * container.currentIndex}px)`;
}
</script>
