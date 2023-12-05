# databases-and-networks-assignment

CREATE Database Databases_and_Networks_assignment;

FIRST NF TABLE


CREATE TABLE first_normal_form 
(
    User_ID	VARCHAR(512) NOT NULL,
    Login_ID	VARCHAR(512) NOT NULL,
    Forename	VARCHAR(512) NOT NULL,
    Surename	VARCHAR(512) NULL ,
    Title	VARCHAR(512) NULL ,
    Position	VARCHAR(512) NULL,
    Email	VARCHAR(512) NOT NULL,
    Phone	INT NOT NULL,
    Location	VARCHAR(512) NULL

);

INSERT INTO first_normal_form (User_ID, Login_ID, Forename, Surename, Title, Position, Email, Phone, Location) VALUES ('202248657', 'COMPSCI', 'BLESSING', 'COXE', 'STUDENT', '2ND YEAR', 'B.COXE-2022@HULL.AC.UK', '987536543', 'Libaray');

INSERT INTO first_normal_form (User_ID, Login_ID, Forename, Surename, Title, Position, Email, Phone, Location) VALUES ('202248658', 'MATHS ', 'SIMION', 'GREY', 'TEACHER', 'PHD', 'S.G-2020@HULL.AC.UK', '806547698', 'RBB');

INSERT INTO first_normal_form (User_ID, Login_ID, Forename, Surename, Title, Position, Email, Phone, Location) VALUES ('202248659', 'ENGLISH', 'ERIKA', 'SIMMION', 'STUDENT', '1ST YR', 'E.S-2021@HULL.AC.UK', '123456789', 'Libaray');

INSERT INTO first_normal_form (User_ID, Login_ID, Forename, Surename, Title, Position, Email, Phone, Location) VALUES ('202248660', 'DRAMA', 'SARAH', 'BAYA', 'STUDENT', '2ND YEAR', 'S.B-2022@HULL.AC.UK', '795011457', 'Libaray');

INSERT INTO first_normal_form (User_ID, Login_ID, Forename, Surename, Title, Position, Email, Phone, Location) VALUES ('202248661', 'DESIGN', 'FLORA', 'GRACE', 'PROFESSOR', 'MASTERS', 'F.G-HULL@HULL.AC.UK', '98765432', 'Venn');

INSERT INTO first_normal_form (User_ID, Login_ID, Forename, Surename, Title, Position, Email, Phone, Location) VALUES ('202248662', 'MATHS  CHANGE TO BU', 'JACK', 'TAYLOR', 'STUDENT', '3RD YR', 'J.T-2011@HULL.AC.UK', '876543876', 'Libaray');

INSERT INTO first_normal_form (User_ID, Login_ID, Forename, Surename, Title, Position, Email, Phone, Location) VALUES ('202248663', 'MEDICENCE', 'PERRI', 'MIX', 'PROFESSOR', 'DR', 'P.M-HULL@.C.UK', '564328', 'Venn');

INSERT INTO first_normal_form (User_ID, Login_ID, Forename, Surename, Title, Position, Email, Phone, Location) VALUES ('202248664', 'LAW', 'SHANDY', 'ROYALE', 'TEACHER', '4YR', 'S.H-2120@HULL.AC.UK', '3463398', 'RBB');

INSERT INTO first_normal_form (User_ID, Login_ID, Forename, Surename, Title, Position, Email, Phone, Location) VALUES ('202248665', 'HISORY', 'ELIJAH', 'JAMES', 'PROFESSOR', 'PHD', 'E.J-2349@HULL.AC.UK', '987475', 'Venn');

INSERT INTO first_normal_form (User_ID, Login_ID, Forename, Surename, Title, Position, Email, Phone, Location) VALUES ('202248666', 'SPAINISH', 'RAUL', 'LUANDA', 'TEACHER', 'MASTERS', 'R.L-2324@HULL.AC.UK', '87794568', 'RBB');


2ND NF - NF_UserAccount 

CREATE TABLE secound_NF_UserAccount 
(
    User_ID 	VARCHAR(512) NOT NULL ,
    Forename	VARCHAR(512) NOT NULL,
    Surename	VARCHAR(512) NULL ,
    Position	VARCHAR(512) NULL ,
    Email	VARCHAR(512) NOT NULL ,
    Phone	INT NOT NULL
);


INSERT INTO secound_NF_UserAccount (User_ID , Forename, Surename, Position, Email, Phone) VALUES ('202248657', 'BLESSING', 'COXE', '2ND YEAR', 'B.COXE-2022@HULL.AC.UK', '987536543');

INSERT INTO secound_NF_UserAccount (User_ID , Forename, Surename, Position, Email, Phone) VALUES ('202248658', 'SIMION', 'GREY', 'PHD', 'S.G-2020@HULL.AC.UK', '806547698');

INSERT INTO secound_NF_UserAccount (User_ID , Forename, Surename, Position, Email, Phone) VALUES ('202248659', 'ERIKA', 'SIMMION', '1ST YR', 'E.S-2021@HULL.AC.UK', '123456789');

INSERT INTO secound_NF_UserAccount (User_ID , Forename, Surename, Position, Email, Phone) VALUES ('202248660', 'SARAH', 'BAYA', '2ND YEAR', 'S.B-2022@HULL.AC.UK', '795011457');

INSERT INTO secound_NF_UserAccount (User_ID , Forename, Surename, Position, Email, Phone) VALUES ('202248661', 'FLORA', 'GRACE', 'MASTERS', 'F.G-HULL@HULL.AC.UK', '98765432');

INSERT INTO secound_NF_UserAccount (User_ID , Forename, Surename, Position, Email, Phone) VALUES ('202248662', 'JACK', 'TAYLOR', '3RD YR', 'J.T-2011@HULL.AC.UK', '876543876');

INSERT INTO secound_NF_UserAccount (User_ID , Forename, Surename, Position, Email, Phone) VALUES ('202248663', 'PERRI', 'MIX', 'DR', 'P.M-HULL@.C.UK', '564328');

INSERT INTO secound_NF_UserAccount (User_ID , Forename, Surename, Position, Email, Phone) VALUES ('202248664', 'SHANDY', 'ROYALE', '4YR', 'S.H-2120@HULL.AC.UK', '3463398');

INSERT INTO secound_NF_UserAccount (User_ID , Forename, Surename, Position, Email, Phone) VALUES ('202248665', 'ELIJAH', 'JAMES', 'PHD', 'E.J-2349@HULL.AC.UK', '987475');

INSERT INTO secound_NF_UserAccount (User_ID , Forename, Surename, Position, Email, Phone) VALUES ('202248666', 'RAUL', 'LUANDA', 'MASTERS', 'R.L-2324@HULL.AC.UK', '87794568');


2ND NF – COMPUTER USER

CREATE TABLE secound_NF_COMPUTER_USERS
(
    Login_ID 	VARCHAR(512) NOT NULL ,
     Title	VARCHAR(512) NULL ,
     Location	VARCHAR(512) NULL
);

INSERT INTO secound_NF_COMPUTER_USERS (Login_ID , Title, Location) VALUES ('COMPSCI', 'STUDENT', 'Libaray');

INSERT INTO secound_NF_COMPUTER_USERS (Login_ID , Title, Location) VALUES ('MATHS ', 'TEACHER', 'RBB');

INSERT INTO secound_NF_COMPUTER_USERS (Login_ID , Title, Location) VALUES ('ENGLISH', 'STUDENT', 'Libaray');

INSERT INTO secound_NF_COMPUTER_USERS (Login_ID , Title, Location) VALUES ('DRAMA', 'STUDENT', 'Libaray');

INSERT INTO secound_NF_COMPUTER_USERS (Login_ID , Title, Location) VALUES ('DESIGN', 'PROFESSOR', 'Venn');

INSERT INTO secound_NF_COMPUTER_USERS (Login_ID , Title, Location) VALUES ('BUSINESS', 'STUDENT', 'Libaray');

INSERT INTO secound_NF_COMPUTER_USERS (Login_ID , Title, Location) VALUES ('MEDICENCE', 'PROFESSOR', 'Venn');

INSERT INTO secound_NF_COMPUTER_USERS (Login_ID , Title, Location) VALUES ('LAW', 'TEACHER', 'RBB');

INSERT INTO secound_NF_COMPUTER_USERS (Login_ID , Title, Location) VALUES ('HISORY', 'PROFESSOR', 'Venn');

INSERT INTO secound_NF_COMPUTER_USERS (Login_ID , Title, Location) VALUES ('SPAINISH', 'TEACHER', 'RBB');

 
 3RD NF 

CREATE TABLE THIRD_NF 
(
    User_ID 	VARCHAR(512) NOT NULL ,
    Login_ID	VARCHAR(512) NOT NULL
);


INSERT INTO THIRD_NF (User_ID , Login_ID) VALUES ('202248657', 'COMPSCI');

INSERT INTO THIRD_NF (User_ID , Login_ID) VALUES ('202248658', 'MATHS ');

INSERT INTO THIRD_NF (User_ID , Login_ID) VALUES ('202248659', 'ENGLISH');

INSERT INTO THIRD_NF (User_ID , Login_ID) VALUES ('202248660', 'DRAMA');

INSERT INTO THIRD_NF (User_ID , Login_ID) VALUES ('202248661', 'DESIGN');

INSERT INTO THIRD_NF (User_ID , Login_ID) VALUES ('202248662', 'BUSINESS');

INSERT INTO THIRD_NF (User_ID , Login_ID) VALUES ('202248663', 'MEDICENCE');

INSERT INTO THIRD_NF (User_ID , Login_ID) VALUES ('202248664', 'LAW');

INSERT INTO THIRD_NF (User_ID , Login_ID) VALUES ('202248665', 'HISORY');

INSERT INTO THIRD_NF (User_ID , Login_ID) VALUES ('202248666', 'SPAINISH');


