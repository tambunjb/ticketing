# Ticketing

I've developed a ticketing system with two versions: one for administrators and another for general users. Each version includes both web and mobile interfaces. This module enables general users to submit tickets to different operational units within an institution, like maintenance, IT, academics, and more.

Let's break down the data structure :
<p align="center">
<img width="60%" alt="bagian" src="https://github.com/tambunjb/ticketing/assets/22196181/66c3415c-39b0-4cde-a21c-507c723586ea">
</p>
1. complaint: Represents the tickets created by users.<br />
2. bagian: Represents the units where tickets are directed.<br />
3. user_has_bagian: Establishes a many-to-many connection between units and users, showing which users are responsible for specific units as administrators.<br />
4. status: Indicates the status of a complaint, whether it's resolved, rejected, in progress, or waiting.<br />
5. response: Contains feedback from administrators.<br />
<br />
Now, let's explore the web interface :
<br /><br />
Firstly, there's the unit management view, where administrators can perform CRUD operations.
<p align="center">
<img width="60%" alt="bagian" src="https://github.com/tambunjb/ticketing/assets/22196181/c6d29057-9cce-47df-87bf-848e41ddd0e4">
</p>
<br />
Next, there's a view to assign administrators by linking any user in the system to a specific unit.
<p align="center">
<img width="60%" alt="admin" src="https://github.com/tambunjb/ticketing/assets/22196181/c6bcfd5f-1876-45d2-8a3a-ddbf6ae7f7e7">
</p>
<br />
Then, there's a form for general users to submit tickets or complaints.
<p align="center">
<img width="60%" alt="complaint-add" src="https://github.com/tambunjb/ticketing/assets/22196181/6160a850-778b-4e88-b046-359f7d75b898">
</p>
<br />
Administrators have the ability to reassign a complaint to the correct unit if the user submits it to the wrong one.
<p align="center">
<img width="60%" alt="bagian-change" src="https://github.com/tambunjb/ticketing/assets/22196181/4c72f057-0900-4f5e-b6f7-d2833c81c414">
</p>
<br />
There's a form allowing administrators to change the status of a complaint to 'in progress' by specifying the expected resolution date.
<p align="center">
<img width="60%" alt="complaint-inprogress" src="https://github.com/tambunjb/ticketing/assets/22196181/ad119fe1-5720-4928-80dc-751b56db56fe">
</p>
<br />
Another form enables administrators to mark a complaint as 'rejected' or 'solved', providing comments and images if necessary.
<p align="center">
<img width="60%" alt="response-add" src="https://github.com/tambunjb/ticketing/assets/22196181/82962837-b8e8-4d9e-938a-4a2fdf35bbab">
</p>
<br />
There's a view for administrators to see a list of complaints created for their unit.
<p align="center">
<img width="60%" alt="complaint-index" src="https://github.com/tambunjb/ticketing/assets/22196181/0cf524da-e2f7-4e62-bb47-12434a583b56">
</p>
<br />
Additionally, there's a list of responses created by administrators.
<p align="center">
<img width="60%" alt="response-index" src="https://github.com/tambunjb/ticketing/assets/22196181/60785dde-224d-4bdf-ac60-a96a6a57fc2b">
</p>
<br />
Finally, there are two videos demonstrating the mobile app, which includes the same features as those found on the web :
<br /><br />
One for general users
<p align="left">
<img width="30%" alt="response-index" src="https://github.com/tambunjb/ticketing/assets/22196181/49c47f31-3db8-4732-b0c4-81af4023f9c7">
</p>
<br />
And the other for administrators.
<p align="left">
<img width="30%" alt="response-index" src="https://github.com/tambunjb/ticketing/assets/22196181/73b3a44f-88f5-4d9e-a0f4-359f114c313c">
</p>
<br />
That wraps up this module. It's straightforward and simple, yet extremely important for organizations seeking to manage their operations and ensure member satisfaction.

