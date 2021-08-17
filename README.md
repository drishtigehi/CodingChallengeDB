## ReadMe

| **Components** | **Sub-Components** | **Description** | **Navigation** |
| --- | --- | --- | --- |
| Login Page | Login to portal | User can enter email to access the app | ChatBot |
| ChatBot RhEA | A radio button based MCQ for mood | Employee can interact with RhEA to record mood and describe reason along with # | MyMoodBoard |
| | Track previous response | Employee can access previous chats in a click |
| MyMoodBoard | Employee Response Statistics | Employee can view statistics of overall responses categorised as total, positive, okay and bad responses | Organisation MoodBoard, ChatBot and Login Page|
|| Graphical Representation | Employee can visualize the last 7 days&#39; responses using a graph |
|| Filter Responses | Employee can filter their responses categorised as total, positive, okay and bad responses |
| OrganizationMoodBoard | Organisation Response Statistics | Employee can view statistics of overall organisation responses categorised as total, positive, okay and bad responses | MyMoodBoard |
|| Graphical Representation | Employee can visualize the last 7 days&#39; organisation responses using a graph |

Libraries Used:

Front End

- React
- Material UI
- React Chart JS


Screenshots:

1. Login Page

![Login](/image001.jpg?raw=true)

2. RhEA ChatBot

![Chatbot](/image002.jpg?raw=true)

3. My MoodBoard

![](/image003.jpg?raw=true)

4. Organization MoodBoard


![](/image004.jpg?raw=true)

Demo Video Link
[http://bit.ly/teamUnityDemo](http://bit.ly/teamUnityDemo)

#### Backend

| **Page** | **API** | **Description** |
| --- | --- | --- |
| Login | addEmployee | Adds an employee in the database. Returns alreadyExists: true if employee is already present |
| Survey | submitSurvey | Sends entire information entered by the employee to the database. This includes:mood: {}timestamp: {}description: {}hashtags: {}user\_email: {}emp\_id: {} |
|| userStats | Displays statistics such as average mood, number of responses and most used hashtag for a particular employee |
|| previousResponses | Gives the timestamped previous responses for a week for a particular employee |
| Statistics | orgStats/{time\_period} | Returns weekly or monthly statistics for the entire organization as specified by the {time\_period} |
|| myStats/{time\_period} | Returns weekly or monthly statistics for an employee as specified by the {time\_period} |
|| org/count | Returns the total organizations total number of responses for each mood |
|| my/count | Returns the employees number of responses for each mood |


Technologies Used:

Backend End

- SQL
- Spring-Data-JPA
- Spring-Boot

