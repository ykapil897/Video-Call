<h1>Video Calling App</h1>
<p>
A modern, full-stack <strong>video calling application</strong> built with a robust backend powered by 
<strong>Spring Boot</strong>, <strong>WebRTC</strong>, and <strong>WebSockets</strong>, paired with a sleek frontend using 
<strong>HTML</strong>, <strong>CSS</strong>, <strong>JavaScript</strong>, <strong>STOMP Client</strong>, and <strong>SockJS</strong>.  
This project showcases real-time peer-to-peer communication with seamless signaling and a smooth user experience.
</p>

<h2>✨ Features</h2>
<ul>
    <li>High-quality, real-time <strong>video + audio</strong> communication.</li>
    <li>Reliable and efficient <strong>signaling</strong> over WebSockets.</li>
    <li>Clean, responsive, and interactive user interface.</li>
    <li>Easy-to-extend architecture integrating <strong>WebRTC P2P</strong> capabilities.</li>
    <li>WebSocket communication enhanced with the <strong>STOMP protocol</strong>.</li>
</ul>

<hr>

<h2>🧰 Technologies Used</h2>

<h3>Backend</h3>
<ul>
    <li><strong>Spring Boot</strong>: REST API + WebSocket signaling server.</li>
    <li><strong>WebRTC</strong>: Peer-to-peer video and audio transmission.</li>
    <li><strong>WebSockets</strong>: Real-time signaling channel for metadata exchange.</li>
</ul>

<h3>Frontend</h3>
<ul>
    <li><strong>HTML, CSS, JavaScript</strong>: Lightweight and responsive UI.</li>
    <li><strong>STOMP Client</strong>: Structured messaging over WebSockets.</li>
    <li><strong>SockJS</strong>: Robust fallback for environments lacking WebSocket support.</li>
</ul>

<hr>

<h2>📐 System Architecture</h2>
<p>
The application relies on <strong>WebRTC</strong> to establish secure peer-to-peer media channels, while a 
<strong>Spring Boot WebSocket server</strong> handles signaling for exchanging 
<strong>SDP</strong> and <strong>ICE</strong> candidates.  
This architecture ensures smooth connection setup and reliable cross-network communication.
</p>

<h3>🖼️ System Design Diagram</h3>
<p>The diagram below illustrates the signaling flow and peer connection handshake:</p>
<img src="systemDesign.png" alt="System Design Diagram" style="max-width:100%; height:auto;">

<hr>

<h2>🚀 Project Setup</h2>

<h3>Backend Setup</h3>
<ol>
    <li>Clone the repository:
        <pre><code>git clone &lt;repository-url&gt;</code></pre>
    </li>
    <li>Move into the backend directory:
        <pre><code>cd backend</code></pre>
    </li>
    <li>Start the Spring Boot application:
        <pre><code>./mvnw spring-boot:run</code></pre>
    </li>
    <li>Open <strong>https://localhost:3000</strong> to launch the frontend interface.</li>
</ol>

<hr>

<h2>⚙️ How It Works</h2>
<ol>
    <li><strong>Signaling Phase</strong>
        <ul>
            <li>The client connects to the WebSocket signaling server.</li>
            <li>SDP offers/answers and ICE candidates are exchanged over the WebSocket channel.</li>
        </ul>
    </li>

    <li><strong>Peer-to-Peer Connection</strong>
        <ul>
            <li>WebRTC APIs establish a direct, encrypted channel between both users.</li>
        </ul>
    </li>

    <li><strong>Media Streaming</strong>
        <ul>
            <li>Local audio and video streams are captured and transmitted through the P2P connection.</li>
        </ul>
    </li>
</ol>

<hr>

<h2>🤝 Contributing</h2>
<p>
Contributions are warmly welcomed!  
Feel free to fork the repository, enhance the project, and submit a pull request with your improvements.
</p>

<hr>
