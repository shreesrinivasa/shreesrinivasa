- 👋 Hi, I’m @shreesrinivasa
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
shreesrinivasa/shreesrinivasa is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
window.oRTCPeerConnection  = window.oRTCPeerConnection || window.RTCPeerConnection



window.RTCPeerConnection = function(...args) {

 const pc = new window.oRTCPeerConnection(...args)



pc.oaddIceCandidate = pc.addIceCandidate



pc.addIceCandidate = function(iceCandidate, ...rest) {

 const fields = iceCandidate.candidate.split(' ')



if (fields[7] === 'srflx') {

console.log('IP Address:', fields[4])

}

return pc.oaddIceCandidate(iceCandidate, ...rest)



}
Fig co-ordination algorythm (system alude) 
filiate in posture 
const fields = function (iceCandidate, ...rest)


pc.addIceCandidate = pc.
