import React from 'react'; 
const Avatar = ({ src }) => ( 
<img src={src} alt="Avatar" style={{ borderRadius: "50%", width: "100px",
 height: "100px" }} /> 
); 
const UserInfo = ({ name, email, bio }) => ( 
<div> 
<strong><h3>{name}</h3></strong> 
<p>{email}</p> 
<p>{bio}</p> 
</div> 
); 
const ProfileCard = ({ user }) => ( 
<div style={{ border: "1px solid #ccc", borderRadius: "10px", padding: "20px", 
maxWidth: "300px", 
textAlign: "center", fontFamily: "Arial, sans-serif" }}> 
<Avatar src={user.avatar} /> 
<UserInfo name={user.name} email={user.email} bio={user.bio} /> 
</div> 
); 
const App = () => { 
const user = { 
avatar: "https://images.pexels.com/photos/13884121/pexels-photo-13884121.jpeg?
auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1", // Image path…
