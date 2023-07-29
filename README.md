# Student-Mentor-Assign

[ //Sample data to create a Student and perform crud,
    {
        "id": 1,
        "name": "Srikanth",
        "DOB": "02-110-1998",
        "email": "sri@gmail.com",
        "phone": "1234567890",
        "location": "chennai",
        "batch": "B46",
        "course": "Full Stack Development"
    },
    {
        "id": 2,
        "name": "Ajith",
        "DOB": "02-01-1998",
        "email": "aji@gmail.com",
        "phone": "1234567890",
        "location": "chennai",
        "batch": "B46",
        "course": "Full Stack Development"
    },
    {
        "id": 3,
        "name": "Sasi",
        "DOB": "06-05-1995",
        "email": "sasi@gmail.com",
        "phone": "1234567890",
        "location": "chennai",
        "batch": "B46",
        "course": "Full Stack Development"
    },
    {
        "id": 4,
        "name": "Mc",
        "DOB": "06-05-1995",
        "email": "mc@gmail.com",
        "phone": "1234567890",
        "location": "chennai",
        "batch": "B47",
        "course": "Full Stack Development"
    },
    {
        "id": 5,
        "name": "Guru",
        "DOB": "06-05-1999",
        "email": "guru@gmail.com",
        "phone": "8374265222",
        "location": "chennai",
        "batch": "B47",
        "course": "Full Stack Development"
    },
    
]
           ///STUDENT///
1) In ps create -post - localhost:9000/student/create,
2) Get all - localhost:9000/student/all
3) update/edit - PUT - localhost:9000/student/update/5   ,//the number denotes the id ,
4) delete - localhost:9000/student/delete/1

         ///MENTOR//
         Sample data
[
    {
        "_id": "64c56793bf45fc96371c6bdf",
        "id": 1,
        "name": "Naga",
        "age": "35",
        "email": "mentorname@email.com",
        "phone": "7878812345",
        "location": "Delhi",
        "batch": "B46WD",
        "specialization": [
            "Data Science",
            "Web Development",
            "Machine Learning"
        ],
        "student": [
            {
                "_id": "64c51805179ec019469701d8",
                "id": 2,
                "name": "Ajith",
                "DOB": "02-01-1998",
                "email": "aji@gmail.com",
                "phone": "1234567890",
                "location": "chennai",
                "batch": "B46",
                "course": "Full Stack Development"
            },
            {
                "_id": "64c5182d179ec019469701d9",
                "id": 3,
                "name": "Sasi",
                "DOB": "06-05-1995",
                "email": "sasi@gmail.com",
                "phone": "1234567890",
                "location": "chennai",
                "batch": "B46",
                "course": "Full Stack Development"
            },
            {
                "_id": "64c51856179ec019469701da",
                "id": 4,
                "name": "Mc",
                "DOB": "06-05-1995",
                "email": "mc@gmail.com",
                "phone": "1234567890",
                "location": "chennai",
                "batch": "B47",
                "course": "Full Stack Development"
            }
        ]
    },
    {
        "_id": "64c5682dbf45fc96371c6be0",
        "id": 2,
        "name": "Tamil",
        "age": "32",
        "email": "Tamil@email.com",
        "phone": "7878854321",
        "location": "Banglore",
        "batch": "B47WD",
        "specialization": [
            "Data Science",
            "Web Development",
            "Machine Learning"
        ],
        "student": [
            {
            "_id": "64c51885179ec019469701db",
                "id": 5,
                "name": "Guru",
                "DOB": "06-05-1999",
                "email": "guru@gmail.com",
                "phone": "8374265222",
                "location": "chennai",
                "batch": "B47",
                "course": "Full Stack Development"
            },
            {
                "_id": "64c5644dbf45fc96371c6bde",
                "id": 1,
                "name": "Srikanth",
                "DOB": "02-110-1998",
                "email": "sri@gmail.com",
                "phone": "1234567890",
                "location": "chennai",
                "batch": "B46",
                "course": "Full Stack Development"
            }
        ]
    }
] 

*And then API to Assign a Student to a Mentor

*Select one mentor and add multiple students,
*A student who has a mentor should not be shown in the list,
*PUT method:localhost:9000/mentor/updateMentor/1,
*Payload : { "student": [2,5,6]} //2,5,6 are id's of students,
 
* API to assign or change a mentor for a particular student,
*Select one student and assign one mentor,
*PUT method:localhost:9000/mentor/assign/1 (this will assign student 1 to mentor 1),
*Payload : { "mentorId": 1},

*API to show all students for a particular Mentor,
*GET method: localhost:9000/mentor/get/1.

