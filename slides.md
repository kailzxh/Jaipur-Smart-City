---
# Jaipur: The Journey to a Smart City
theme: seriph
background: https://images.unsplash.com/photo-1730100628933-71caa2821ca9?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
class: text-center
highlighter: shiki
lineNumbers: false
drawings:
  persist: false
transition: slide-left
title: Jaipur - The Smart City Journey
mdc: true
---

# Jaipur: The Journey to a Smart City

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <a href="https://www.jaipur.gov.in/" target="_blank" alt="Jaipur Official"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:globe />
  </a>
</div>

<!-- This is the first slide introducing our topic -->

---
layout: two-cols
transition: fade-out
---

# The Pink City

<div class="flex flex-col items-center">
  <div v-motion
    :initial="{ x: -80, opacity: 0 }"
    :enter="{ x: 0, opacity: 1, transition: { delay: 200, duration: 1000 } }">
    <img src="https://plus.unsplash.com/premium_photo-1697730286559-98b1a193eef6?q=80&w=2036&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="rounded-lg shadow-xl" />
    <p class="text-sm opacity-70 mt-2">Traditional architecture of Jaipur</p>
  </div>
</div>

::right::

<div class="pt-12 pl-10">
  <ul>
    <li v-motion
      :initial="{ x: 100, opacity: 0 }"
      :enter="{ x: 0, opacity: 1, transition: { delay: 300, duration: 1000 } }">
      Founded in 1727 by Maharaja Sawai Jai Singh II
    </li>
    <li v-motion
      :initial="{ x: 100, opacity: 0 }"
      :enter="{ x: 0, opacity: 1, transition: { delay: 600, duration: 1000 } }">
      Known for its distinctive pink buildings
    </li>
    <li v-motion
      :initial="{ x: 100, opacity: 0 }"
      :enter="{ x: 0, opacity: 1, transition: { delay: 900, duration: 1000 } }">
      UNESCO World Heritage Site since 2019
    </li>
  </ul>
</div>

<!-- Introduction to Jaipur's historical context -->

---
layout: center
class: text-center
transition: slide-up
---

# Jaipur: Then & Now

<div class="grid grid-cols-2 gap-4">
  <div v-motion :initial="{ x: -100, opacity: 0 }" :enter="{ x: 0, opacity: 1 }">
    <img src="https://images.unsplash.com/photo-1584297875607-e85a9608d5b7?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="rounded-lg shadow-xl" />
    <p class="text-sm opacity-50 mt-2">Traditional Jaipur</p>
  </div>
  <div v-motion :initial="{ x: 100, opacity: 0 }" :enter="{ x: 0, opacity: 1, transition: { delay: 500 } }">
    <img src="https://jaipurbeat.com/wp-content/uploads/2016/05/9-wtp1.jpg" class="rounded-lg shadow-xl" />
    <p class="text-sm opacity-50 mt-2">Modern Developments</p>
  </div>
</div>

<!-- Comparison showing traditional vs. emerging modern Jaipur -->

---
layout: center
background: https://source.unsplash.com/OOT1IjfsYhI/1920x1080
class: text-center
transition: zoom-in
---

# Challenges Before Smart City Initiative

<div class="grid grid-cols-3 gap-6 pt-10">
  <div class="bg-white bg-opacity-15 backdrop-blur-sm p-4 rounded-lg" v-motion :initial="{ y: 100, opacity: 0 }" :enter="{ y: 0, opacity: 1, transition: { delay: 200 } }">
    <carbon:traffic-flow class="text-4xl mx-auto text-orange-400" />
    <h3 class="text-xl font-bold mt-2">Traffic Congestion</h3>
  </div>
  
  <div class="bg-white bg-opacity-15 backdrop-blur-sm p-4 rounded-lg" v-motion :initial="{ y: 100, opacity: 0 }" :enter="{ y: 0, opacity: 1, transition: { delay: 400 } }">
    <carbon:rain-drop class="text-4xl mx-auto text-blue-400" />
    <h3 class="text-xl font-bold mt-2">Water Management</h3>
  </div>
  
  <div class="bg-white bg-opacity-15 backdrop-blur-sm p-4 rounded-lg" v-motion :initial="{ y: 100, opacity: 0 }" :enter="{ y: 0, opacity: 1, transition: { delay: 600 } }">
    <carbon:battery-charging class="text-4xl mx-auto text-yellow-400" />
    <h3 class="text-xl font-bold mt-2">Energy Inefficiency</h3>
  </div>
</div>

<!-- Key challenges faced by Jaipur before smart city initiative -->

---
layout: full
transition: slide-left
---

# Key Urban Metrics Before 2015

<div class="h-80 pt-5" v-motion :initial="{ y: 50, opacity: 0 }" :enter="{ y: 0, opacity: 1 }">
  <BarChart 
    :data="{
      labels: ['Traffic Congestion', 'Air Quality Index', 'Digital Services', 'Water Management', 'Waste Management'],
      datasets: [
        {
          label: 'Performance Score (0-100)',
          data: [35, 45, 20, 30, 25],
          backgroundColor: ['#FF6B6B', '#FFA86B', '#4ECDC4', '#45B7D1', '#9055A2']
        }
      ]
    }"
    :options="{
      animation: {
        duration: 2000,
      },
      scales: {
        y: {
          beginAtZero: true,
          max: 100
        }
      }
    }"
  />
</div>

<p class="text-xs opacity-50 text-center mt-2">Source: Jaipur Municipal Corporation Data (2015)</p>

<!-- Data visualization of key urban metrics before smart city initiative -->

---
transition: fade
layout: image-right
image: https://images.unsplash.com/photo-1686477316633-562a65893e36?q=80&w=1977&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
---

# Turning Point: Smart City Mission

<div v-click class="mt-6">
  <carbon:pedestrian class="text-blue-500 text-4xl inline-block" /> <span class="text-xl">Selected in Round 1 (2015)</span>
</div>

<div v-click class="mt-6">
  <carbon:money class="text-green-500 text-4xl inline-block" /> <span class="text-xl">₹2,401 Crore Budget</span>
</div>

<div v-click class="mt-6">
  <carbon:partnership class="text-purple-500 text-4xl inline-block" /> <span class="text-xl">PPP Model Implementation</span>
</div>

<div v-click class="mt-6">
  <carbon:chart-multitype class="text-pink-500 text-4xl inline-block" /> <span class="text-xl">Area-Based Development</span>
</div>

<div v-click class="mt-6">
  <carbon:idea class="text-amber-500 text-4xl inline-block" /> <span class="text-xl">Pan-City Solutions</span>
</div>

<!-- Introduction to Smart City Mission and how Jaipur was selected -->

---
layout: center
transition: slide-up
render: true
---

<div class="w-full pt-6" v-motion :initial="{ y: 80, opacity: 0 }" :enter="{ y: 0, opacity: 1 }">
  <div class="relative h-24">
    <!-- Timeline Line -->
    <div class="absolute w-full h-1 bg-gray-300 top-1/2"></div>

    <!-- Timeline Points -->
  <div v-click class="absolute left-0 top-1/2 transform -translate-y-1/2 -translate-x-1">
      <div class="w-6 h-6 rounded-full bg-red-500 border-4 border-white shadow-lg"></div>
      <div class="absolute top-8 -left-14 w-28 text-center">
        <p class="text-sm font-bold">2015</p>
        <p class="text-xs">Selection</p>
      </div>
    </div>

  <div v-click class="absolute left-1/4 top-1/2 transform -translate-y-1/2">
      <div class="w-6 h-6 rounded-full bg-yellow-500 border-4 border-white shadow-lg"></div>
      <div class="absolute top-8 -left-14 w-28 text-center">
        <p class="text-sm font-bold">2017</p>
        <p class="text-xs">Planning Phase</p>
      </div>
    </div>

  <div v-click class="absolute left-1/2 top-1/2 transform -translate-y-1/2 -translate-x-3">
      <div class="w-6 h-6 rounded-full bg-green-500 border-4 border-white shadow-lg"></div>
      <div class="absolute top-8 -left-14 w-28 text-center">
        <p class="text-sm font-bold">2019</p>
        <p class="text-xs">Implementation</p>
      </div>
    </div>

  <div v-click class="absolute left-3/4 top-1/2 transform -translate-y-1/2">
      <div class="w-6 h-6 rounded-full bg-blue-500 border-4 border-white shadow-lg"></div>
      <div class="absolute top-8 -left-14 w-28 text-center">
        <p class="text-sm font-bold">2021</p>
        <p class="text-xs">Major Milestones</p>
      </div>
    </div>
    <div v-click class="absolute right-0 top-1/2 transform -translate-y-1/2 translate-x-1">
      <div class="w-6 h-6 rounded-full bg-purple-500 border-4 border-white shadow-lg"></div>
      <div class="absolute top-8 -left-14 w-28 text-center">
        <p class="text-sm font-bold">2023</p>
        <p class="text-xs">Advanced Phase</p>
      </div>
    </div>
    
  </div>
</div>


<!-- Timeline showing key milestones in Jaipur's smart city journey -->

---
layout: image-left
image: https://images.unsplash.com/photo-1740052969517-dca821fd4b69?q=80&w=1975&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
transition: slide-up
---

# Smart Mobility

<div v-click>
  <h3 class="text-2xl text-orange-500 font-bold">Metro Rail Network</h3>
  <p class="mb-4">Expanded to connect key areas with reduced traffic congestion</p>
</div>

<div v-click>
  <h3 class="text-2xl text-green-500 font-bold">Smart Bus System</h3>
  <p class="mb-4">GPS-tracked, electric buses with real-time arrival information</p>
</div>

<div v-click>
  <h3 class="text-2xl text-blue-500 font-bold">E-Rickshaws</h3>
  <p class="mb-4">Clean last-mile connectivity solution reducing emissions</p>
</div>

<div v-click>
  <h3 class="text-2xl text-purple-500 font-bold">Transport App</h3>
  <p>Unified city transport information and booking platform</p>
</div>

<!-- Smart mobility features implemented in Jaipur -->

---
layout: center
transition: slide-left
---

# Intelligent Traffic Management System

<div class="grid grid-cols-2 gap-8 pt-10">
  <div class="relative overflow-hidden rounded-xl shadow-xl" v-motion :initial="{ x: -50, opacity: 0 }" :enter="{ x: 0, opacity: 1 }">
    <img src="https://images.unsplash.com/photo-1648515298105-d8c30a81c13a?q=80&w=2076&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="w-full h-64 object-cover" />
    <div class="absolute bottom-0 left-0 right-0 bg-gradient-to-t from-black/70 to-transparent p-4">
      <h3 class="text-white text-xl font-bold">Adaptive Traffic Signals</h3>
      <p class="text-white text-sm opacity-80">Responds to real-time traffic conditions</p>
    </div>
  </div>
  
  <div class="relative overflow-hidden rounded-xl shadow-xl" v-motion :initial="{ x: 50, opacity: 0 }" :enter="{ x: 0, opacity: 1, transition: { delay: 300 } }">
    <img src="https://images.unsplash.com/photo-1732149779890-3fe3e7b5fdb8?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="w-full h-64 object-cover" />
    <div class="absolute bottom-0 left-0 right-0 bg-gradient-to-t from-black/70 to-transparent p-4">
      <h3 class="text-white text-xl font-bold">Traffic Monitoring Center</h3>
      <p class="text-white text-sm opacity-80">Centralizing control and response systems</p>
    </div>
  </div>
</div>

<div class="pt-8 text-center">
  <div v-click class="inline-block bg-green-500 text-white px-4 py-2 rounded-full text-sm font-bold">
    <carbon:chart-line class="inline mr-1" /> 30% Reduction in Travel Time
  </div>
</div>

<!-- Intelligent traffic management system features -->

---
layout: center
transition: zoom-in
---

# Smart Street Lighting

<div class="relative w-full h-80" v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { duration: 1500 } }">
  <img src="https://plus.unsplash.com/premium_photo-1739739796004-0e0132daa87a?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="w-full h-full object-cover rounded-xl" />
  
  <div v-click class="absolute top-10 left-10 bg-white/80 backdrop-blur-sm p-3 rounded-lg shadow-lg">
    <h3 class="text-lg font-bold text-gray-800">LED Conversion</h3>
    <p class="text-sm text-gray-700">95% of street lights converted to LED</p>
  </div>
  
  <div v-click class="absolute top-10 right-10 bg-white/80 backdrop-blur-sm p-3 rounded-lg shadow-lg">
    <h3 class="text-lg font-bold text-gray-800">Motion Sensors</h3>
    <p class="text-sm text-gray-700">Adaptive brightness based on movement</p>
  </div>
  
  <div v-click class="absolute bottom-10 left-10 bg-white/80 backdrop-blur-sm p-3 rounded-lg shadow-lg">
    <h3 class="text-lg font-bold text-gray-800">Energy Savings</h3>
    <p class="text-sm text-gray-700">67% reduction in energy consumption</p>
  </div>
  
  <div v-click class="absolute bottom-10 right-10 bg-white/80 backdrop-blur-sm p-3 rounded-lg shadow-lg">
    <h3 class="text-lg font-bold text-gray-800">Remote Monitoring</h3>
    <p class="text-sm text-gray-700">Centralized dashboard for maintenance</p>
  </div>
</div>

<!-- Smart street lighting system implemented in Jaipur -->

---
layout: full
transition: slide-up
---

# Digital Infrastructure

<div class="grid grid-cols-3 gap-6 pt-10">
  <div class="bg-gradient-to-br from-blue-500 to-blue-700 text-white p-6 rounded-xl shadow-lg" v-motion :initial="{ y: 50, opacity: 0 }" :enter="{ y: 0, opacity: 1, transition: { delay: 200 } }">
    <carbon:wifi class="text-5xl mb-4" />
    <h3 class="text-xl font-bold mb-2">Public Wi-Fi</h3>
    <p class="text-sm opacity-80">300+ hotspots across tourist spots, markets and public spaces</p>
  </div>
  
  <div class="bg-gradient-to-br from-purple-500 to-purple-700 text-white p-6 rounded-xl shadow-lg" v-motion :initial="{ y: 50, opacity: 0 }" :enter="{ y: 0, opacity: 1, transition: { delay: 400 } }">
    <carbon:store class="text-5xl mb-4" />
    <h3 class="text-xl font-bold mb-2">Digital Kiosks</h3>
    <p class="text-sm opacity-80">Self-service terminals for government services and tourist information</p>
  </div>
  
  <div class="bg-gradient-to-br from-pink-500 to-pink-700 text-white p-6 rounded-xl shadow-lg" v-motion :initial="{ y: 50, opacity: 0 }" :enter="{ y: 0, opacity: 1, transition: { delay: 600 } }">
    <carbon:iot-platform class="text-5xl mb-4" />
    <h3 class="text-xl font-bold mb-2">IoT Network</h3>
    <p class="text-sm opacity-80">Citywide sensor network for environment, traffic and infrastructure monitoring</p>
  </div>
</div>

<!-- Digital infrastructure development in Jaipur -->

---
layout: two-cols
transition: fade-out
---

# Smart Water Management

<div class="pr-10">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcToiynbzeUi1oMbc6_EIpELzVYIc0xMrp9svw&s" class="rounded-lg shadow-lg mb-6" />
  
  <div class="space-y-4">
    <div v-click class="flex items-start">
      <div class="bg-blue-500 p-2 rounded-full text-white mr-4">
        <mdi:gauge class="text-xl" />
      </div>
      <div>
        <h3 class="font-bold">Smart Meters</h3>
        <p class="text-sm">Real-time water consumption tracking</p>
      </div>
    </div>
    
    <div v-click class="flex items-start">
      <div class="bg-blue-500 p-2 rounded-full text-white mr-4">
        <carbon:warning-alt class="text-xl" />
      </div>
      <div>
        <h3 class="font-bold">Leak Detection</h3>
        <p class="text-sm">AI-based monitoring reduces water loss</p>
      </div>
    </div>
  </div>
</div>

::right::

<div class="pl-4 pt-6">
  <h3 class="text-xl font-bold mb-6 text-blue-600">Water Savings Impact</h3>
  
  <div class="h-64" v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 500 } }">
    <LineChart 
      :data="{
        labels: ['2018', '2019', '2020', '2021', '2022', '2023'],
        datasets: [
          {
            label: 'Water Wastage (Million Liters)',
            data: [460, 420, 350, 280, 230, 190],
            borderColor: '#3B82F6',
            backgroundColor: 'rgba(59, 130, 246, 0.2)',
            tension: 0.3,
            fill: true
          }
        ]
      }"
      :options="{
        animation: {
          duration: 2000
        }
      }"
    />
  </div>
  
  <p class="text-xs opacity-50 text-center mt-2">Source: Jaipur Water Supply Department</p>
</div>

<!-- Smart water management systems and their impact -->

---
layout: center
class: text-center
transition: slide-left
---

# Waste Management Revolution

<div class="grid grid-cols-2 gap-8 pt-10">
  <div class="text-left" v-motion :initial="{ x: -50, opacity: 0 }" :enter="{ x: 0, opacity: 1 }">
    <h3 class="text-2xl font-bold text-green-600 mb-4">Before</h3>
    <ul class="space-y-2">
      <li v-click class="flex items-center">
        <carbon:close-filled class="text-red-500 mr-2" /> Irregular collection
      </li>
      <li v-click class="flex items-center">
        <carbon:close-filled class="text-red-500 mr-2" /> Manual tracking
      </li>
      <li v-click class="flex items-center">
        <carbon:close-filled class="text-red-500 mr-2" /> Limited segregation
      </li>
      <li v-click class="flex items-center">
        <carbon:close-filled class="text-red-500 mr-2" /> Landfill focused
      </li>
    </ul>
    
    <img src="https://images.unsplash.com/photo-1591284080149-58e039950b29?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="mt-6 rounded-lg shadow-md" />
  </div>
  
  <div class="text-left" v-motion :initial="{ x: 50, opacity: 0 }" :enter="{ x: 0, opacity: 1, transition: { delay: 300 } }">
    <h3 class="text-2xl font-bold text-green-600 mb-4">After</h3>
    <ul class="space-y-2">
      <li v-click class="flex items-center">
        <carbon:checkmark-filled class="text-green-500 mr-2" /> GPS-tracked collection fleet
      </li>
      <li v-click class="flex items-center">
        <carbon:checkmark-filled class="text-green-500 mr-2" /> Smart bins with fill-level sensors
      </li>
      <li v-click class="flex items-center">
        <carbon:checkmark-filled class="text-green-500 mr-2" /> Automated segregation facilities
      </li>
      <li v-click class="flex items-center">
        <carbon:checkmark-filled class="text-green-500 mr-2" /> Waste-to-energy conversion
      </li>
    </ul>
    
    <img src="https://plus.unsplash.com/premium_photo-1726786836056-79f08e0334fa?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="mt-6 rounded-lg shadow-md" />
  </div>
</div>

<!-- Waste management transformation with before/after comparison -->

---
transition: fade
---

# E-Governance & Citizen Services

<div class="grid grid-cols-3 gap-4 pt-6">
  <div v-click class="bg-white shadow-lg rounded-xl overflow-hidden transform transition hover:scale-105">
    <div class="h-2 bg-blue-500"></div>
    <div class="p-5">
      <carbon:application-web class="text-4xl text-blue-500 mb-3" />
      <h3 class="font-bold text-lg mb-2">Jaipur 311 App</h3>
      <p class="text-sm text-gray-600">Citizen reporting platform for municipal issues</p>
    </div>
  </div>
  
  <div v-click class="bg-white shadow-lg rounded-xl overflow-hidden transform transition hover:scale-105">
    <div class="h-2 bg-green-500"></div>
    <div class="p-5">
      <carbon:document class="text-4xl text-green-500 mb-3" />
      <h3 class="font-bold text-lg mb-2">e-Services Portal</h3>
      <p class="text-sm text-gray-600">Online certificates and permissions processing</p>
    </div>
  </div>
  
  <div v-click class="bg-white shadow-lg rounded-xl overflow-hidden transform transition hover:scale-105">
    <div class="h-2 bg-purple-500"></div>
    <div class="p-5">
      <carbon:currency class="text-4xl text-purple-500 mb-3" />
      <h3 class="font-bold text-lg mb-2">Digital Payments</h3>
      <p class="text-sm text-gray-600">Unified platform for all city-related payments</p>
    </div>
  </div>
  
  <div v-click class="bg-white shadow-lg rounded-xl overflow-hidden transform transition hover:scale-105">
    <div class="h-2 bg-pink-500"></div>
    <div class="p-5">
      <carbon:chat class="text-4xl text-pink-500 mb-3" />
      <h3 class="font-bold text-lg mb-2">Smart Feedback</h3>
      <p class="text-sm text-gray-600">Citizen input collection and sentiment analysis</p>
    </div>
  </div>
  
  <div v-click class="bg-white shadow-lg rounded-xl overflow-hidden transform transition hover:scale-105">
    <div class="h-2 bg-yellow-500"></div>
    <div class="p-5">
      <carbon:analytics class="text-4xl text-yellow-500 mb-3" />
      <h3 class="font-bold text-lg mb-2">Open Data Portal</h3>
      <p class="text-sm text-gray-600">Public access to city data for transparency</p>
    </div>
  </div>
  
  <div v-click class="bg-white shadow-lg rounded-xl overflow-hidden transform transition hover:scale-105">
    <div class="h-2 bg-red-500"></div>
    <div class="p-5">
      <carbon:location class="text-4xl text-red-500 mb-3" />
      <h3 class="font-bold text-lg mb-2">City GIS Platform</h3>
      <p class="text-sm text-gray-600">Spatial planning and service locator</p>
    </div>
  </div>
</div>

<!-- E-governance and digital citizen services -->

---
layout: two-cols
transition: slide-up
---

# Public Safety & Security

<div class="pr-6">
  <img src="https://images.unsplash.com/photo-1651338703370-e292e06239dc?w=600&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MjB8fGNpdHklMjBzZXJjdXJpdHklMjBzeXN0ZW0lMjBjYW1lcmFzfGVufDB8MHwwfHx8MA%3D%3D" class="rounded-xl shadow-lg mb-6" />
  
  <div v-click>
    <h3 class="text-lg font-bold text-red-600 mb-2">Integrated Command Center</h3>
    <p class="text-sm">Centralized monitoring of all city security systems and emergency response coordination</p>
  </div>
</div>

::right::

<div class="space-y-4 pl-6">
  <div v-click class="bg-white/60 backdrop-blur-sm p-4 rounded-lg shadow-md">
    <div class="flex items-center">
      <carbon:security class="text-xl text-red-500 mr-3" />
      <h3 class="font-bold">5,000+ CCTV Cameras</h3>
    </div>
    <p class="text-sm mt-1">AI-powered video analytics for incident detection</p>
  </div>
  
  <div v-click class="bg-white/60 backdrop-blur-sm p-4 rounded-lg shadow-md">
    <div class="flex items-center">
      <carbon:help class="text-xl text-red-500 mr-3" />
      <h3 class="font-bold">Emergency Response System</h3>
    </div>
    <p class="text-sm mt-1">Reduced response time from 25 to 8 minutes</p>
  </div>
  
  <div v-click class="bg-white/60 backdrop-blur-sm p-4 rounded-lg shadow-md">
    <div class="flex items-center">
      <carbon:pedestrian class="text-xl text-red-500 mr-3" />
      <h3 class="font-bold">Women Safety Initiatives</h3>
    </div>
    <p class="text-sm mt-1">Pink zones with enhanced security in public areas</p>
  </div>
  
  <div v-click class="bg-white/60 backdrop-blur-sm p-4 rounded-lg shadow-md">
    <div class="flex items-center">
      <carbon:warning class="text-xl text-red-500 mr-3" />
      <h3 class="font-bold">Disaster Management</h3>
    </div>
    <p class="text-sm mt-1">Early warning systems for urban flooding and other disasters</p>
  </div>
</div>

<!-- Public safety and security infrastructure -->

---
layout: center
class: text-center
transition: fade-out
---

# Smart Tourism - Heritage Meets Technology

<div class="grid grid-cols-2 gap-8 pt-8">
  <div v-motion :initial="{ x: -80, opacity: 0 }" :enter="{ x: 0, opacity: 1 }">
    <img src="https://source.unsplash.com/EXdXLrZXS9Q/500x300" class="rounded-lg shadow-lg mb-4" />
    
  <div v-click class="bg-white/90 backdrop-blur-sm rounded-lg p-4 -mt-20 mx-10 relative shadow-lg z-10">
      <h3 class="font-bold text-pink-600">AR Historical Experiences</h3>
      <p class="text-sm">Bringing monuments to life with augmented reality</p>
    </div>
  </div>
  
  <div v-motion :initial="{ x: 80, opacity: 0 }" :enter="{ x: 0, opacity: 1, transition: { delay: 300 } }">
    <img src="https://source.unsplash.com/yZ4cX5-Vu2o/500x300" class="rounded-lg shadow-lg mb-4" />
    
  <div v-click class="bg-white/90 backdrop-blur-sm rounded-lg p-4 -mt-20 mx-10 relative shadow-lg z-10">
      <h3 class="font-bold text-pink-600">Smart Tourist Guides</h3>
      <p class="text-sm">Personalized recommendations and navigation</p>
    </div>
  </div>
</div>

<div class="grid grid-cols-3 gap-4 mt-12">
  <div v-click class="bg-pink-100 p-3 rounded-lg">
    <carbon:translate class="text-pink-600 text-2xl mb-2" />
    <p class="text-sm font-medium">Multilingual Kiosks</p>
  </div>
  
  <div v-click class="bg-pink-100 p-3 rounded-lg">
    <carbon:qr-code class="text-pink-600 text-2xl mb-2" />
    <p class="text-sm font-medium">QR-Enabled Exhibits</p>
  </div>
  
  <div v-click class="bg-pink-100 p-3 rounded-lg">
    <carbon:wifi class="text-pink-600 text-2xl mb-2" />
    <p class="text-sm font-medium">Wi-Fi Heritage Zones</p>
  </div>
</div>

<!-- Smart tourism initiatives merging heritage with technology -->

---
layout: center
transition: zoom-in
background: https://plus.unsplash.com/premium_photo-1680302170723-1318f0a8859b?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
class: text-center
---

# Renewable Energy Initiatives

<div class="grid grid-cols-3 gap-6 pt-8">
  <div v-click class="bg-white/80 backdrop-blur-sm p-5 rounded-xl text-left">
    <carbon:solar-panel class="text-4xl text-yellow-500 mb-3" />
    <h3 class="text-xl font-bold mb-2">Solar City</h3>
    <p class="text-sm">30% of government buildings powered by rooftop solar panels</p>
  </div>
  
  <div v-click class="bg-white/80 backdrop-blur-sm p-5 rounded-xl text-left">
    <carbon:chart-multitype class="text-4xl text-green-500 mb-3" />
    <h3 class="text-xl font-bold mb-2">Smart Grid</h3>
    <p class="text-sm">Advanced metering and distribution automation reducing losses by 18%</p>
  </div>
  
  <div v-click class="bg-white/80 backdrop-blur-sm p-5 rounded-xl text-left">
    <carbon:idea class="text-4xl text-blue-500 mb-3" />
    <h3 class="text-xl font-bold mb-2">Energy Efficiency</h3>
    <p class="text-sm">Green building standards for all new constructions reducing consumption</p>
  </div>
</div>

<div v-click class="mt-10 bg-white/90 backdrop-blur-sm inline-block px-6 py-3 rounded-full shadow-lg">
  <div class="flex items-center">
    <carbon:battery-charging class="text-3xl text-green-600 mr-3" />
    <span class="text-xl font-bold">42% Renewable Energy Share by 2023</span>
  </div>
</div>

<!-- Renewable energy initiatives and progress -->

---
layout: full
transition: slide-left
---

# Environmental Monitoring Network

<div class="grid grid-cols-2 gap-8 pt-6">
  <div v-click>
    <h3 class="text-xl font-bold text-green-600 mb-4">Air Quality Management</h3>
    <img src="https://source.unsplash.com/9NCZyWkYWiU/500x250" class="rounded-lg shadow-lg mb-4" />
    
  <div class="bg-white/90 backdrop-blur-sm p-4 rounded-lg shadow-md -mt-16 mx-16 relative z-10">
      <p class="text-sm">Network of 50+ IoT-based air quality monitors providing real-time data</p>
    </div>
  </div>
  
  <div v-click>
    <h3 class="text-xl font-bold text-blue-600 mb-4">Noise Pollution Control</h3>
    <img src="https://images.unsplash.com/photo-1605776988089-105148e14767?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="rounded-lg shadow-lg mb-4" />
    
  <div class="bg-white/90 backdrop-blur-sm p-4 rounded-lg shadow-md -mt-16 mx-16 relative z-10">
      <p class="text-sm">Smart sensors in high-traffic areas with automated enforcement system</p>
    </div>
  </div>
</div>

<div class="pt-12" v-click>
  <div class="h-64">
    <LineChart 
      :data="{
        labels: ['2016', '2017', '2018', '2019', '2020', '2021', '2022', '2023'],
        datasets: [
          {
            label: 'Average AQI (Air Quality Index)',
            data: [210, 195, 180, 160, 140, 125, 115, 105],
            borderColor: '#10B981',
            backgroundColor: 'rgba(16, 185, 129, 0.2)',
            tension: 0.3,
            fill: true
          }
        ]
      }"
      :options="{
        animation: { duration: 2000 },
        scales: { y: { beginAtZero: false } }
      }"
    />
  </div>
  <p class="text-xs opacity-50 text-center mt-1">Source: Jaipur Pollution Control Board</p>
</div>

<!-- Environmental monitoring network and impact -->

---
layout: two-cols
transition: fade
---

# Urban Development Transformation

<div class="pr-10">
  <img src="https://images.unsplash.com/photo-1551035418-5e03824702e5?w=600&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8cGVkZXN0cmFpbiUyMGZyaWVuZGx5fGVufDB8MHwwfHx8MA%3D%3D" class="rounded-lg shadow-lg mb-6" />
  
  <div class="space-y-4">
    <div v-click class="flex items-start">
      <div class="bg-teal-500 p-2 rounded-full text-white mr-4">
        <carbon:pedestrian class="text-xl" />
      </div>
      <div>
        <h3 class="font-bold">Pedestrian-Friendly</h3>
        <p class="text-sm">Walkable neighborhoods and car-free zones</p>
      </div>
    </div>
    
  <div v-click class="flex items-start">
      <div class="bg-teal-500 p-2 rounded-full text-white mr-4">
        <carbon:tree class="text-xl" />
      </div>
      <div>
        <h3 class="font-bold">Green Spaces</h3>
        <p class="text-sm">30% increase in urban parks and gardens</p>
      </div>
    </div>
    
  <div v-click class="flex items-start">
      <div class="bg-teal-500 p-2 rounded-full text-white mr-4">
        <carbon:building class="text-xl" />
      </div>
      <div>
        <h3 class="font-bold">Smart Districts</h3>
        <p class="text-sm">Integrated zones with all smart facilities</p>
      </div>
    </div>
  </div>
</div>

::right::

<div class="pt-6 pl-6">
  <h3 class="text-xl font-bold mb-8 text-teal-600">Urban Form Transformation</h3>
  
  <div class="space-y-6">
    <div v-click class="relative h-16">
      <div class="absolute left-0 top-0 bottom-0 w-3/4 bg-teal-200 rounded-md"></div>
      <div class="absolute left-0 top-0 bottom-0 w-1/4 bg-teal-500 rounded-md"></div>
      <div class="absolute left-6 top-1/2 transform -translate-y-1/2 font-bold text-teal-800">Mixed-Use Development</div>
      <div class="absolute right-6 top-1/2 transform -translate-y-1/2 font-bold">25%</div>
    </div>
    
  <div v-click class="relative h-16">
      <div class="absolute left-0 top-0 bottom-0 w-2/3 bg-blue-200 rounded-md"></div>
      <div class="absolute left-0 top-0 bottom-0 w-1/3 bg-blue-500 rounded-md"></div>
      <div class="absolute left-6 top-1/2 transform -translate-y-1/2 font-bold text-blue-800">Public Transport Coverage</div>
      <div class="absolute right-6 top-1/2 transform -translate-y-1/2 font-bold">33%</div>
    </div>
    
  <div v-click class="relative h-16">
      <div class="absolute left-0 top-0 bottom-0 w-1/2 bg-purple-200 rounded-md"></div>
      <div class="absolute left-0 top-0 bottom-0 w-1/2 bg-purple-500 rounded-md"></div>
      <div class="absolute left-6 top-1/2 transform -translate-y-1/2 font-bold text-purple-800">Connected Green Spaces</div>
      <div class="absolute right-6 top-1/2 transform -translate-y-1/2 font-bold">50%</div>
    </div>
  </div>
</div>

<!-- Urban development transformation with metrics -->

---
layout: center
class: text-center
transition: slide-up
---

# Smart Healthcare Ecosystem

<div class="grid grid-cols-12 gap-4 pt-8">
  <div v-click class="col-span-4 bg-white rounded-xl shadow-lg overflow-hidden">
    <div class="h-2 bg-red-500"></div>
    <div class="p-5">
      <carbon:hospital class="text-4xl text-red-500 mb-3" />
      <h3 class="font-bold">Telemedicine Network</h3>
      <p class="text-sm mt-2">Connecting 30+ hospitals for remote consultations</p>
    </div>
  </div>
  
  <div v-click class="col-span-4 bg-white rounded-xl shadow-lg overflow-hidden">
    <div class="h-2 bg-blue-500"></div>
    <div class="p-5">
      <carbon:development class="text-4xl text-blue-500 mb-3" />
      <h3 class="font-bold">Health Analytics</h3>
      <p class="text-sm mt-2">AI-powered disease outbreak prediction</p>
    </div>
  </div>
  
  <div v-click class="col-span-4 bg-white rounded-xl shadow-lg overflow-hidden">
    <div class="h-2 bg-green-500"></div>
    <div class="p-5">
      <mdi-pill class="text-4xl text-green-500 mb-3" />
      <h3 class="font-bold">e-Pharmacy Network</h3>
      <p class="text-sm mt-2">Medicine delivery optimized by demand patterns</p>
    </div>
  </div>
  
  <div v-click class="col-span-6 bg-white rounded-xl shadow-lg overflow-hidden mt-4">
    <div class="h-2 bg-orange-500"></div>
    <div class="p-5">
      <carbon:document class="text-4xl text-orange-500 mb-3" />
      <h3 class="font-bold">Unified Health Records</h3>
      <p class="text-sm mt-2">Electronic health records accessible across all city healthcare facilities</p>
    </div>
  </div>
  
  <div v-click class="col-span-6 bg-white rounded-xl shadow-lg overflow-hidden mt-4">
    <div class="h-2 bg-purple-500"></div>
    <div class="p-5">
      <carbon:ai-status class="text-4xl text-purple-500 mb-3" />
      <h3 class="font-bold">Smart Ambulance System</h3>
      <p class="text-sm mt-2">Traffic priority system reducing response time by 62%</p>
    </div>
  </div>
</div>

<!-- Smart healthcare ecosystem development -->

---
transition: zoom-in
background: https://images.unsplash.com/photo-1659019479972-82d9e3e8cfb7?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
class: text-center
---

# Economic Impact

<div class="pt-10" v-click>
  <div class="inline-block bg-white/90 backdrop-blur-sm px-6 py-3 rounded-xl shadow-xl">
    <h1 class="text-3xl font-bold text-blue-800">₹5,200+ Crore</h1>
    <p class="text-lg">Economic Value Generated</p>
  </div>
</div>

<div class="grid grid-cols-3 gap-6 pt-10">
  <div v-click class="bg-white/80 backdrop-blur-sm p-5 rounded-xl">
    <h2 class="text-2xl font-bold text-green-600">28%</h2>
    <p>Increase in Tourism Revenue</p>
  </div>
  
  <div v-click class="bg-white/80 backdrop-blur-sm p-5 rounded-xl">
    <h2 class="text-2xl font-bold text-blue-600">15,000+</h2>
    <p>New Tech Jobs Created</p>
  </div>
  
  <div v-click class="bg-white/80 backdrop-blur-sm p-5 rounded-xl">
    <h2 class="text-2xl font-bold text-purple-600">42%</h2>
    <p>Rise in Property Values</p>
  </div>
</div>

<div class="pt-10" v-click>
  <div class="inline-block bg-white/70 backdrop-blur-sm px-6 py-2 rounded-full">
    <carbon:growth class="inline-block text-2xl text-green-600 mr-2" /> <span class="text-xl font-medium">Jaipur's GDP growth rate: 12.4% (2023)</span>
  </div>
</div>

<!-- Economic impact of smart city initiatives -->

---
layout: center
transition: slide-left
---

# Citizen Satisfaction Metrics

<div class="w-full pt-8" v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 300 } }">
  <div class="h-64">
    <BarChart 
      :data="{
        labels: ['Transport', 'Safety', 'Water', 'Cleanliness', 'Digital Services', 'Healthcare'],
        datasets: [
          {
            label: 'Before Smart City (2015)',
            data: [35, 40, 30, 25, 15, 45],
            backgroundColor: 'rgba(239, 68, 68, 0.7)'
          },
          {
            label: 'After Implementation (2023)',
            data: [78, 82, 76, 72, 88, 80],
            backgroundColor: 'rgba(16, 185, 129, 0.7)'
          }
        ]
      }"
      :options="{
        indexAxis: 'y',
        animation: { duration: 2000 },
        scales: { x: { max: 100 } }
      }"
    />
  </div>
</div>

<div class="bg-gray-50 rounded-lg shadow-md p-4 mt-6" v-click>
  <p class="text-sm text-center">
    <carbon:user-multiple class="inline text-blue-500" /> Overall citizen satisfaction increased from <span class="font-bold text-red-500">32%</span> to <span class="font-bold text-green-500">79%</span>
  </p>
</div>

<!-- Citizen satisfaction metrics before and after smart city implementation -->

---
layout: image-right
image: https://plus.unsplash.com/premium_photo-1664635402369-f9a972139fa4?q=80&w=1975&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
transition: fade-out
---

# Future Vision: Jaipur 2030

<div class="space-y-6">
  <div v-click class="bg-white/80 backdrop-blur-sm p-4 rounded-lg shadow-md">
    <carbon:iot-platform class="text-3xl text-blue-600 mb-2" />
    <h3 class="text-lg font-bold">Hyperconnected Infrastructure</h3>
    <p class="text-sm">10X increase in IoT sensors across all systems</p>
  </div>
  
  <div v-click class="bg-white/80 backdrop-blur-sm p-4 rounded-lg shadow-md">
    <carbon:ai-status class="text-3xl text-purple-600 mb-2" />
    <h3 class="text-lg font-bold">AI-Driven Governance</h3>
    <p class="text-sm">Predictive services anticipating citizen needs</p>
  </div>
  
  <div v-click class="bg-white/80 backdrop-blur-sm p-4 rounded-lg shadow-md">
    <carbon:earth class="text-3xl text-green-600 mb-2" />
    <h3 class="text-lg font-bold">Carbon-Neutral City</h3>
    <p class="text-sm">100% renewable energy and zero-emission zones</p>
  </div>
  
  <div v-click class="bg-white/80 backdrop-blur-sm p-4 rounded-lg shadow-md">
    <carbon:augmented-reality class="text-3xl text-amber-600 mb-2" />
    <h3 class="text-lg font-bold">Digital Twin</h3>
    <p class="text-sm">Complete virtual replica for planning and management</p>
  </div>
</div>

<!-- Future vision for Jaipur as a smart city -->

---
layout: full
transition: slide-up
---

# Smart Jaipur: Key Learnings

<div class="grid grid-cols-2 gap-8 pt-10">
  <div v-click class="bg-gradient-to-br from-green-50 to-green-100 p-6 rounded-xl shadow-md border border-green-200">
    <h3 class="text-xl font-bold text-green-700 mb-4">Success Factors</h3>
    
  <ul class="space-y-3">
      <li class="flex items-start">
        <carbon:checkmark-filled class="text-green-600 mt-1 mr-2 flex-shrink-0" />
        <span>Strong public-private partnership model</span>
      </li>
      <li class="flex items-start">
        <carbon:checkmark-filled class="text-green-600 mt-1 mr-2 flex-shrink-0" />
        <span>Citizen-centric approach with continuous feedback</span>
      </li>
      <li class="flex items-start">
        <carbon:checkmark-filled class="text-green-600 mt-1 mr-2 flex-shrink-0" />
        <span>Phased implementation with quick wins</span>
      </li>
      <li class="flex items-start">
        <carbon:checkmark-filled class="text-green-600 mt-1 mr-2 flex-shrink-0" />
        <span>Balancing heritage preservation with technological innovation</span>
      </li>
    </ul>
  </div>
  
  <div v-click class="bg-gradient-to-br from-amber-50 to-amber-100 p-6 rounded-xl shadow-md border border-amber-200">
    <h3 class="text-xl font-bold text-amber-700 mb-4">Challenges Overcome</h3>
    
   <ul class="space-y-3">
      <li class="flex items-start">
        <carbon:close-filled class="text-amber-600 mt-1 mr-2 flex-shrink-0" />
        <span>Digital divide across population segments</span>
      </li>
      <li class="flex items-start">
        <carbon:close-filled class="text-amber-600 mt-1 mr-2 flex-shrink-0" />
        <span>Infrastructure integration with existing systems</span>
      </li>
      <li class="flex items-start">
        <carbon:close-filled class="text-amber-600 mt-1 mr-2 flex-shrink-0" />
        <span>Data privacy and security concerns</span>
      </li>
      <li class="flex items-start">
        <carbon:close-filled class="text-amber-600 mt-1 mr-2 flex-shrink-0" />
        <span>Administrative complexity across departments</span>
      </li>
    </ul>
  </div>
</div>

<!-- Key learnings from Jaipur's smart city journey -->

---
layout: center
class: text-center
transition: fade
---

# Jaipur Smart City: Awards & Recognition

<div class="grid grid-cols-3 gap-6 pt-8">
  <div v-click class="relative group">
    <div class="absolute inset-0 bg-gradient-to-r from-blue-500 to-purple-500 rounded-lg blur opacity-30 group-hover:opacity-50 transition duration-300"></div>
    <div class="relative bg-white p-5 rounded-lg shadow-lg">
      <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-3">
        <carbon:trophy class="text-3xl text-blue-600" />
      </div>
      <h3 class="font-bold mb-2">Smart Cities India Award</h3>
      <p class="text-sm text-gray-600">Heritage Conservation Category, 2022</p>
    </div>
  </div>
  
  <div v-click class="relative group">
    <div class="absolute inset-0 bg-gradient-to-r from-green-500 to-teal-500 rounded-lg blur opacity-30 group-hover:opacity-50 transition duration-300"></div>
    <div class="relative bg-white p-5 rounded-lg shadow-lg">
      <div class="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mx-auto mb-3">
        <carbon:earth class="text-3xl text-green-600" />
      </div>
      <h3 class="font-bold mb-2">World Smart City Award</h3>
      <p class="text-sm text-gray-600">Finalist - Mobility Solution, 2021</p>
    </div>
  </div>
  
  <div v-click class="relative group">
    <div class="absolute inset-0 bg-gradient-to-r from-amber-500 to-orange-500 rounded-lg blur opacity-30 group-hover:opacity-50 transition duration-300"></div>
    <div class="relative bg-white p-5 rounded-lg shadow-lg">
      <div class="w-16 h-16 bg-amber-100 rounded-full flex items-center justify-center mx-auto mb-3">
        <carbon:idea class="text-3xl text-amber-600" />
      </div>
      <h3 class="font-bold mb-2">National e-Governance Award</h3>
      <p class="text-sm text-gray-600">Excellence in Citizen-Centric Service, 2023</p>
    </div>
  </div>
</div>

<div v-click class="mt-8 relative group inline-block">
  <div class="absolute inset-0 bg-gradient-to-r from-pink-500 to-red-500 rounded-full blur opacity-30 group-hover:opacity-50 transition duration-300"></div>
  <div class="relative bg-white px-8 py-3 rounded-full shadow-lg">
    <h3 class="font-bold text-lg">ISO 37122:2019 Certification</h3>
    <p class="text-sm text-gray-600">Sustainable Cities and Communities Indicators</p>
  </div>
</div>

<!-- Awards and recognition received by Jaipur for smart city initiatives -->

---
layout: end
class: text-center
---

# Thank You

<div class="pt-8 pb-12">
  <span class="px-2 py-1">Jaipur: Blending Heritage with Innovation</span>
</div>

<div class="abs-bl m-6 flex gap-2">
  <a href="https://www.smartcities.gov.in/" target="_blank" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:globe />
  </a>
  <a href="https://jscljaipur.in/" target="_blank" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:home />
  </a>
</div>

<!-- Closing slide with contact information -->