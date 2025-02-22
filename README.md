# Studentmarks
let students = [];

function createStudent(name, age, mark) {
    return { name: name, age: age, mark: mark };
}

students.push(createStudent("sanaa", 20, 70));
students.push(createStudent("maryam", 19, 70));
students.push(createStudent("rana", 19, 70));
students.push(createStudent("yasmeen", 19, 40));
students.push(createStudent("sara", 19, 50));

let successStudents = [];
let failedStudents = [];

for (let i = 0; i < students.length; i++) {
    if (students[i].mark >= 50) {
        successStudents.push(students[i]);
    } else {
        failedStudents.push(students[i]);
    }
}

console.log("success students", successStudents);
console.log("failed students", failedStudents);