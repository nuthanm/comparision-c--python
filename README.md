# Comparision cheat sheet between CSharp and Python object
In this repository, you will find the comparison sheet for c# and Python objects,

The below table difference is based on using **Python 3.10 and c# 7.0,**

| Object      | Python Syntax     | CSharp Syntax                    | Description                    | Python Example                   | CSharp Example |
| :---        | :----:            |    :---:                         |       :---:                    | :---:                            | :--:           |
| Empty List  | object = []       | var type = new List<DataType>()  | Empty list creation            | todos = []                       | var todos = new List<string>()|
| Type Checking| type(variable)   | typeof(variable)                 | Checking type of the variable  | name = "nani" print(type(name))  | var name="nani"; Console.WriteLine(typeOf(name));|
| Increment | variable = variable + 1 | var++ or var = var + 1  | Increment by 1| i = 0 \\n i = i + 1 | var i = 0; i++; or i = i+1|
| Conditional | match <user_action>: case "action": <logic> | switch(user_action){ case "action": "logic"; break;} Note: Switch expression is another approach where we define switch | Alternative to if else implementation |user_action = input("Todo app - add, show, exit: ") match  user_action: | var user_action = Console.ReadLine(); switch(user_action) { case "add": "add an item"; break; } |
| remove space | using strip() | using Trim() or TrimEnd() |remove space from a string end | user_action = input("enter a string :") user_action = user_action.strip() | var user_action = Console.ReadLine(); user_action = user_action.TrimEnd(); |
| 'r' or '@' | file = open(r'absolutepath','r') | var fileStream = new StreamReader(@'abolsutepath');| If path contains any special characters like \t or \n then it converts into normal character | file = open(r"d:\todos.txt",'r') | var stream = new StreamReader(@"d:\todos.txt");|
| string interpolation | using 'f' | using $"" | Instead of index we interpolate with variable directly |print(f'name:  {user_input}')| Console.WriteLine($"name: {user_input}");|
|Dipose automatically|with open('<file>','w/r') as file: file.readlines()| using(var reader = new StreamReader('filepath')){ reader.ReadLine();} | Dispose object automatically and file handling properly does| with open('todos.txt','r') as file: file.readlines() | using(var reader = new StreamReader('todos.txt')){ reader.ReadLine();}|
