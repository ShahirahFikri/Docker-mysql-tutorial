# CODES: 

CREATE TABLE ICTSS_Member
(StudentId int primary key,
StudentName VARCHAR(50),
Position_ICTSS VARCHAR(35),
Email VARCHAR(40),
PhoneNo VARCHAR(15),
ProgId VARCHAR(15)
);

CREATE TABLE New_Application
(StudentID VARCHAR2(10),
StudentName VARCHAR2(50),
Email VARCHAR2(40),
PhoneNo VARCHAR2(15),
ResumeTitle VARCHAR2(30),
Remarks VARCHAR2(20),
CONSTRAINT New_Application_StudentID_PK PRIMARY KEY (StudentID));

CREATE TABLE Program
(ProgId VARCHAR2(10),
ProgName VARCHAR2(50),
StudentId VARCHAR2(10),
CONSTRAINT Program_ProgId_PK PRIMARY KEY (ProgId),
CONSTRAINT Program_StudentId_FK FOREIGN KEY(StudentId)
REFERENCES ICTSS_Member);




INSERT INTO ICTSS_Member VALUES('1944','Aina Leya', 'President', 'aina@gmail.com', '0139944331', '45');
INSERT INTO ICTSS_Member VALUES('1966','Putra Jen', 'Vice President','putra@gmail.com',  '0133388717', '44');
INSERT INTO ICTSS_Member VALUES('1977','Mohd Dani', 'Secretary 1', 'dani@gmail.com', '0138844331', '43');
INSERT INTO ICTSS_Member VALUES('2073','Sofea Jun', 'Secretary 2', 'sofea@gmail.com',  '0132244331', '42');
INSERT INTO ICTSS_Member VALUES('2015','Ali Naufal', 'Treasurer', 'alinau@gmail.com', '0135544331', '41');
INSERT INTO ICTSS_Member VALUES('2190', 'Lisa Wan', 'Ordinary Member', 'lisaw@gmmail.com', '0131144331', '40');
INSERT INTO ICTSS_Member VALUES('2142', 'Iman Sufi', 'Ordinary Member', ' iman@gmail.com', '0130044331', '39');
INSERT INTO ICTSS_Member VALUES('2267', 'Hani Maria', 'Ordinary Member', 'hani@gmail.com', '0131188771', '38');
INSERT INTO ICTSS_Member VALUES('2201','Bada Leen', 'Ordinary Member', 'badal@gmail.com', '0139988771', '37');
INSERT INTO ICTSS_Member VALUES('2217','Kasih Iman', 'Ordinary Member','kasih@gmail.com', '0137888771', '36');

INSERT INTO New_Application VALUES('2201', 'Bada Leen', 'badal@gmail.com', '0139988771', 'S2201_bada.pdf', 'Approved');
INSERT INTO New_Application VALUES('2267', 'Hani Maria', 'hani@gmail.com', '0131188771', 'S2267_Hani.pdf', 'Approved');
INSERT INTO New_Application VALUES('2207', 'Darwina Syah', 'darwinnn@gmail.com', '0176798711', 'S2207_Darwina.pdf', 'Not Approved');
INSERT INTO New_Application VALUES('2270', 'Cellina Badrul', 'ccellin@gmail.com', '0154798711', 'S2270_Cellina.pdf', 'Not Approved');
INSERT INTO New_Application VALUES('2277', 'Bina Syafiq', 'binaa@gmail.com', '0132798721', 'S2277_Bina.pdf', 'Not Approved');
INSERT INTO New_Application VALUES('2251', 'Eisya Zarul', 'eisya@gmail.com', '0121798721', 'S2251_Eisya.pdf', 'Not Approved');
INSERT INTO New_Application VALUES('2241', 'Hairul Lutfi', 'hairul@gmail.com', '0170909091', 'S2241_Hairul.pdf', 'Not Approved');
INSERT INTO New_Application VALUES('2247', 'Ika Daman', 'ikadaman@gmail.com', 0170509091, 'S2247_Ika.pdf', 'Not Approved');
INSERT INTO New_Application VALUES('2231', 'Jamani Dam', 'jamani@gmail.com', '0170309091', 'S2231_Jamani.pdf', 'Not Approved');
INSERT INTO New_Application VALUES('2265', 'Sofea Anis', 'sofeanis@gmail.com', '0186635352', 'S2265_Sofeanis.pdf', 'Not Approved');

INSERT INTO PROGRAM VALUES('45', 'Kict 20th Anniversary', '1944');
INSERT INTO PROGRAM VALUES('44', 'Cybersecurity Talk 2022', '1966');
INSERT INTO PROGRAM VALUES('43', 'ICTSS 2021 Excellence celebration', '1977');
INSERT INTO PROGRAM VALUES('42', 'ICTSS Designing workshop', '2073');
INSERT INTO PROGRAM VALUES('41', 'ICTSS next mainboard election', '2015');
INSERT INTO PROGRAM VALUES('40', 'Mental health talk', '2190');
INSERT INTO PROGRAM VALUES('39', 'Zero Waste Talk', '2142');
INSERT INTO PROGRAM VALUES('38', 'Ramadan night talk part 2', '2267');
INSERT INTO PROGRAM VALUES('37', 'Ramadan night talk part 1', '2201');
INSERT INTO PROGRAM VALUES('36', 'Ict AI Quiz contest 202', '2217');




DROP TABLE ICTSS_Member cascade constraints;
DROP TABLE New_Application cascade constraints;
DROP TABLE Program cascade constraints;


# SAMPLE RUN



# COMMANDS:

**1) List all of the ICTSS Members.**

_SELECT * FROM ICTSS_Member;_

**2) List the studentId and studentName for the President position.**

_SELECT studentId, studentName_
_from ICTSS_Member_
_where position_ICTSS = 'President';_

**3) Remove the programId column from ICTSS Member.**

_ALTER TABLE ICTSS_Member_
_DROP COLUMN progId;_

**4) List the programId and programName for student with studentId ='1944'.**

_select ProgId, ProgName_
_from Program NATURAL JOIN ICTSS_Member_
_where ProgId = (select ProgId from ICTSS_Member where StudentId = '1944');_

**5) Insert the programId column into the ICTSS Member table.**

_ALTER TABLE ICTSS_Member ADD COLUMN ProgId int AFTER PhoneNo_

**6) Modify the program id of a student.**

_UPDATE ICTSS_Member SET ProgId = '45' WHERE StudentId = 1944_


