# AI-BASED-RECOMMENDATION-SYSTEM

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: KAUSHIK PAUL

*INTERN ID*: CTIS8066

*DOMAIN*: JAVA PROGRAMMING

*DURATION*: 6 WEEKS

*MENTOR*: NEELA SANTHOSH KUMAR


# AI-Based Recommendation System (Java + Apache Mahout)

## Introduction

This project is a simple implementation of a recommendation system using Java. The goal was to understand how platforms like Netflix or Amazon suggest items based on user behavior.
Instead of using complex datasets, a small CSV file is used to simulate user ratings, and Apache Mahout is used to generate recommendations.

---

## What This Project Does

The system takes user ratings as input and suggests new items that the user might like.
It works by comparing users with similar tastes and recommending items that similar users have already liked.

---

## How It Works (In Simple Terms)

* Each user gives ratings to some items
* The system finds users with similar rating patterns
* It checks what those similar users liked
* It recommends those items to the current user

This approach is called **user-based collaborative filtering**

---

## Technologies Used

* Java
* Apache Mahout
* Maven
* CSV file for storing data

---

## Project Structure

```text
RecommendationSystem/
│
├── pom.xml
├── data.csv
└── src/
    └── main/
        └── java/
            └── RecommendationSystem.java
```

---

## Dataset Format

The dataset is stored in `data.csv` and follows this format:

```text
UserID, ItemID, Rating
```

Example:

```text
1,101,5
1,102,3
2,101,2
3,104,4
```

This means:

* User 1 rated item 101 as 5
* User 2 rated item 101 as 2

---

## How to Run the Project

1. Open terminal inside the project folder

2. Compile the project

```bash
mvn clean compile
```

3. Run the program

```bash
mvn exec:java "-Dexec.mainClass=RecommendationSystem"
```

---

## Sample Output

```text
Enter User ID: 1

Recommendations for User 1:
Item ID: 104 | Rating: 4.5
```

---

## Things I Noticed While Testing

* If the dataset is small, sometimes only one recommendation appears
* If a user has already rated most items, fewer suggestions are generated
* Changing the dataset changes the output immediately

---

## Limitations

* Works on a small dataset only
* No user interface (console-based)
* Item names are not shown, only IDs
* New users with no data cannot get recommendations (cold start problem)

---

## Possible Improvements

* Add item names instead of IDs
* Use a larger dataset (like MovieLens)
* Build a GUI for better interaction
* Store data in a database instead of CSV
* Combine with content-based filtering

---

## Conclusion

This project helped in understanding the basic idea behind recommendation systems. Even with a small dataset, it shows how user preferences can be used to generate meaningful suggestions. It also gives a good starting point for building more advanced systems.

---
# OUTPUT

<img width="1098" height="641" alt="Image" src="https://github.com/user-attachments/assets/6b25e9e3-fae9-4566-bdcc-a139e1bf71ba" />
<img width="1132" height="577" alt="Image" src="https://github.com/user-attachments/assets/3ea79235-d495-4633-8656-646f9008e8dd" />
