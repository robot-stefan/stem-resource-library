# :book: Book List - College Teams :book:

*Note: Resources with a :mag: have an online option either the current edition or an older edition*

### Outline
1. [Mechanical](#mechanical)
2. [Electrical](#electrical)
3. [Software](#software)
4. [Systems](#systems)
5. [Career](#career)

### Mechanical

#### [Engineering Statics](https://engineeringstatics.org/) & [Mechanics Map](https://mechanicsmap.org/) :mag:
Two web resources on mechanics.

#### Mechanics Part I - Statics ([open library](https://openlibrary.org/books/OL51747106M/Mechanics_-_Part_1))
An older textbook that hits directly into the topic of statics. If you find the primary text a bit long this is to the point and has some clear examples. This book does have some plain and clear diagrams and starts off simple such that some of the intro could be used to explore forces acting on a robot for a high school team. 

#### Mechanics Part II - Dynamics ([open library](https://openlibrary.org/books/OL61418287M/Mechanics_Part_II_Dynamics))
Similar to part 1 but covers dynamics. 

#### Standard Handbook of Machine Design ([open library](https://openlibrary.org/books/OL2536253M/Standard_handbook_of_machine_design) - ISBN: 0-07-056892-8)
Covers a very wide set of mechanical engineering concepts with applications in the style of a reference handbook.

#### Mechanical Engineering Design ([open library](https://openlibrary.org/books/OL2036508M/Mechanical_engineering_design) - ISBN: 0-07-056899-5)

#### TM 1-420 Lathes ([internet archive](https://archive.org/details/TM1-420/mode/2up)) :mag:
Technical Manual produced by the War Department and Army Aviation in the 1940s covers using engine lathes, setting them up, and use of different tooling to create parts.

*Public Domain Note: This is a work of the federal government and is in the public domain mirrored on the internet archive.*

#### TM 1-421 Milling Machines, Shapers, and Planers ([internet archive](https://archive.org/details/TM1-421/mode/2up)) :mag:
Technical Manual produced by the War Department and Army Aviation in the 1940s covers using knee mills, shapers, and planers. My shop in college contained a few milling machines no too dissimilar than some shown. This goes into proper work setup, clamping, cutting gears, etc.

*Public Domain Note: This is a work of the federal government and is in the public domain mirrored on the internet archive.*

#### Machine Shop Operations by American Technical Society ([open library](https://openlibrary.org/works/OL7606852W/Machine_shop_operations_..))
A 1930s text with step by step work instructions and illustrations showing the use of engine lathes, knee mills, centerless grinders, etc. to do common manufacturing jobs. All manual with no automation. Illustrations are simple and direct. These can be used to also show tool access for needed machining operations. This aspect is still relevant today even in a CNC automation world and is a fundamental consideration of design for manufacturing. 

#### Foundations of Mechanical Accuracy ([open library](https://openlibrary.org/books/OL10237334M/Foundations_of_Mechanical_Accuracy))

#### Timken Engineering Manual ([timken website](https://engineering.timken.com/wp-content/uploads/2024/08/Timken-Engineering-Manual.pdf)) :mag:
Manual covering use of Timken bearing products and applications. 

### Electrical 

#### The Art of Electronics 3rd Ed.  ([open library](https://openlibrary.org/books/OL26462574M/The_art_of_electronics) - ISBN: 978-0521809269)
An accessible text book on electronics starting from the basics and moving toward much more advanced topics. There are follow on books covering lab exercises and additional technical content in this series. 

#### Troubleshooting Analog Circuits ([open library](https://openlibrary.org/books/OL1534119M/Troubleshooting_analog_circuits) - ISBN: 978-0750691840)

#### Designing Electronics That Work ([open library](https://openlibrary.org/books/OL50630058M/Designing_Electronics_That_Work) - ISBN: 978-1718503366)
Looks at building electronics in R&D / startup settings to go from 0 to 1 in electronics hardware. I worked with the author in college pulling quite a few all nighters building robots. A few of the lessons learned and failures mentioned I too experienced.  

#### The Book of I2C ([open library](https://openlibrary.org/books/OL38327873M/Book_of_I%C2%B2C) - ISBN: 978-1718502468)


### Software

#### Deep Learning with Python 3rd Ed. ([book website](https://deeplearningwithpython.io) - ISBN: 978-1633436589) :mag:
This book features an online option at [https://deeplearningwithpython.io/](https://deeplearningwithpython.io/) with jupyter notebooks. Note that for some options running these in the cloud with a service such as google colab might be the best route depending on your computers capabilities. 

#### Foundations of Computer Vision ([book website](https://visionbook.mit.edu/)) - ISBN: 978-0262048972) :mag:
This book features an online option at [https://visionbook.mit.edu/](https://visionbook.mit.edu/) with various code examples. It cover computer vision broadly and then dives into more and more complex aspects.  

#### The Missing README ([open library](https://openlibrary.org/books/OL32475987M/The_Missing_README) - ISBN: 978-1718501836)
A book on working in software team and building systems. A lot of this is also very applicable to hardware systems that are tightly couple with software. Some of the best practices and tips would be good to be adopted by college robotics efforts.  

#### The Art of Clean Code ([open library](https://openlibrary.org/books/OL34988587M/Art_of_Clean_Code) - ISBN: 978-1718502185)
While this book covers programing, it has topics such as its chapter on the theme of premature optimization that are a universal thing to watch out for during development both in hardware and software.

#### Hardcore Programming for Mechanical Engineers ([open library](https://openlibrary.org/books/OL29881895M/Hardcore_Programming_for_Engineers) - ISBN: 978-1718500785)
A great jump into python. This book walks the reader through building a bridge truss simulator from scratch and covers many aspects of the python language and applies them to an engineering problem. Touches on numerical methods considerations, testing, and finite element work flows in a 2d truss. Covering virtual deformation, stiffness, etc. The text covers various testing concepts, software architecture considerations, and demonstrates object oriented applied to a relatively complex project compared to conventional python books.  

#### Modeling and Simulation in Python ([open library](https://openlibrary.org/works/OL25922755W/Modeling_and_Simulation_in_Python) - ISBN:  978-1718502161) :mag:
Covers various numerical methods for simulation in python. Book is also available for free in web form from the author's website at [https://greenteapress.com/wp/modsimpy/](https://greenteapress.com/wp/modsimpy/) & [https://allendowney.github.io/ModSimPy/](https://allendowney.github.io/ModSimPy/)


### Systems

#### NIST/SEMATECH e-Handbook of Statistical Methods ([website](https://www.itl.nist.gov/div898/handbook/)) :mag:
You can download a [PDF edition](https://www.itl.nist.gov/div898/handbook/toolaids/pff/E-Handbook.pdf) as well as use online. This walks through a lot of measurement concepts and methods around measurement and process. It’s highly relevant as robots use sensors to measure aspects of their environment and then perform some action based on those measurements. If we have faulty or unreliable measurements we have a bad robot.  

#### Poor Man's Explanation of Kalman Filtering or How I Stopped Worrying & Learned to Love Matrix Inversion 
A report by Roger M. du Plessis on actually implementing Kalman Filtering. 

#### NASA Task Load Index (TLX) ([NASA Human Systems Divison](https://www.nasa.gov/human-systems-integration-division/nasa-task-load-index-tlx/)) :mag:
Tools for looking at human component of systems. 

#### Just Enough Design ([open library](https://openlibrary.org/books/OL39710847M/Just_Enough_Design) - ISBN: 978-1797209906)
When designing and engineering systems can we leverage concepts of just enough to not only look at sustainability of the materials, but keep systems simple? Simple in maintenance, simple in assembly or manufacture?  

### Career

#### The Art of Doing Science and Engineering ([open library](https://openlibrary.org/books/OL28156535M/The_Art_of_Doing_Science_and_Engineering) - ISBN:  978-1732265172)
On being an engineer, solving problems and how technology and innovation are in a constant cycle.

#### Sunburst and Luminary ([open library](https://openlibrary.org/books/OL29463359M/Sunburst_and_Luminary) - ISBN: 978-0986385933)
Covers the post college journey of an engineer who wrote apollo guidance software. 

#### An Elegant Puzzle: Systems of Engineering Management ([open library](https://openlibrary.org/books/OL27905593M/An_Elegant_Puzzle) - ISBN: 978-1732265189)
Covers topics around managing engineering teams of various sizes at different types of companies from software and web lens.

#### The Innovators Dilemma ([open library](https://openlibrary.org/books/OL26432023M/The_Innovator's_Dilemma) - ISBN: 978-1633691780)
A classic book on how innovative market entrants can win against established players. 

#### Practical Doomsday ([open library](https://openlibrary.org/books/OL34988565M/Practical_Doomsday) - ISBN: 978-1718502123)
Covers preparing for everyday and prevention allowing road bumps to be minor time sinks. 
