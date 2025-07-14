 C
Structure:
Data of different types can be grouped together under a single name using structures.
Declaration:
struct tagname
{
data type member1;
data type member2;
.................
data type member N;
};
Here tagname is the name of the structure. 
->The data type can be int, float, char, pointer ar another structure.
->Declaration of a structure won't create any space in memory.
->The memory is created only when the variables of the structure are declared.
->The member names inside a structure should be unique.
->The structure template can be declared globally or locally.
Declaring structure variables:
1.with structure declaration
struct student
{
int rollno;
char name[20];
float marks;
}var1,var2;
2.using structure tag
struct student
{
int rollno;
char name[20];
float marks;
};
struct student var1,var2;
Initialization of structure variables:
The syntax of initializing is similar to arrays.
struct student
{
int rollno;
char name[20];
float marks;
}var1={1,"Latha",70};
struct student var2={2,"Rani",67.5};
->we can't initialize members while defining a structure.
->If no.of initializers are less than the no.of members then the remaing are initialized with zero.
Accessing members of a structure:
->We can access the members of a structure using (.) operator.
->The dot operator is also called as period or membership operator.
->var1.rollno, var1.name,var1.marks.
Sizeof a structure:
sizeof(struct student);
sizeof(var1);
sizeof(var2);
->The size of structure is different based on the memory alignment restrictions on some computers.
struct s
{
char c;
int n;
}var1;
->Here the size of this structure is 8 bytes due to padding. 
->Means the size of the structure is not equal to the sum of the sizes of the members.
->Comparing of two structures is not allowed in c due to unused bytes present in a strucure.
