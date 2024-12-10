# Routine_Manager
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Timetable Management System</title>
</head>
<body>
    <h1>Timetable Management System</h1>
    <h2>Introduction</h2>
    <p>The <strong>Timetable Management System</strong> is a Python project designed to help manage and organize class schedules. This project demonstrates a variety of Python concepts including data structures, functions, object-oriented programming (OOP), and the use of external libraries such as Pandas and NumPy.</p>
    <h2>Features</h2>
    <ul>
        <li><strong>User Authentication</strong>: Secure login system validating user section and role.</li>
        <li><strong>Timetable Generation</strong>: Automatically generates and manages timetables.</li>
        <li><strong>Class Management</strong>: Assign and remove classes from the timetable.</li>
        <li><strong>User Roles</strong>: Different access levels for Teachers, Teaching Assistants, and Students.</li>
        <li><strong>Data Manipulation</strong>: Utilizes Pandas and NumPy for efficient data handling.</li>
        <li><strong>Iterative Display</strong>: Displays timetable iteratively and converts it to a pandas DataFrame.</li>
    </ul>
    <h2>Concepts Covered</h2>
    <p>The project covers the following Python concepts:</p>
    <ol>
        <li><strong>Lists</strong>: Used to store days and time slots.</li>
        <li><strong>Tuples</strong>: Used in timetable schedules.</li>
        <li><strong>Sets</strong>: Used to manage unique class codes and titles.</li>
        <li><strong>Dictionaries</strong>: Used extensively for timetable management.</li>
        <li><strong>If-Else Statements</strong>: Used for conditional logic.</li>
        <li><strong>Loops</strong>: Used for iterating over collections.</li>
        <li><strong>Map Functions</strong>: Used for mapping timetable slots to statuses.</li>
        <li><strong>Lambda Functions</strong>: Used for concise functions in <code>TimetableLambda</code>.</li>
        <li><strong>Inheritance</strong>: Demonstrates single, multiple, and multilevel inheritance.</li>
        <li><strong>Iterators</strong>: Implements an iterator for the timetable.</li>
        <li><strong>Polymorphism</strong>: Demonstrates through method overriding.</li>
        <li><strong>Abstraction</strong>: Uses abstract base classes and methods.</li>
        <li><strong>Encapsulation</strong>: Encapsulates attributes and methods within classes.</li>
        <li><strong>Date Handling</strong>: Utilizes the <code>datetime</code> module.</li>
        <li><strong>Exception Handling</strong>: Uses try-except blocks.</li>
        <li><strong>Pandas Module</strong>: Converts timetable data to a DataFrame.</li>
        <li><strong>NumPy Module</strong>: Used for data manipulation.</li>
    </ol>
    <h2>Installation</h2>
    <p>To run this project, you'll need to have Python installed on your system along with the following libraries:</p>
    <ul>
        <li><code>datetime</code></li>
        <li><code>numpy</code></li>
        <li><code>pandas</code></li>
        <li><code>tabulate</code></li>
    </ul>
    <p>You can install the required libraries using pip:</p>
    <pre><code>pip install numpy pandas tabulate</code></pre>
    <h2>Usage</h2>
    <ol>
        <li>Clone the repository:</li>
        <pre><code>git clone https://github.com/yourusername/timetable-management-system.git
cd timetable-management-system</code></pre>
        <li>Run the main script:</li>
        <pre><code>python main.py</code></pre>
        <li>Follow the prompts to log in, manage classes, and view the timetable.</li>
    </ol>
    <h2>Classes and Methods</h2>
    <h3><code>TimetableGenerator</code></h3>
    <ul>
        <li><code>generate_timetable()</code>: Initializes the timetable with "Free" slots.</li>
        <li><code>timeTable_for_63_M()</code>: Sets a predefined schedule for section 63_M.</li>
        <li><code>display_day_routine(day)</code>: Displays the routine for a specific day.</li>
        <li><code>print_timetable()</code>: Prints the full timetable.</li>
        <li><code>display_timetable()</code>: Displays the timetable in a formatted table.</li>
        <li><code>convert_to_dataframe()</code>: Converts the timetable to a pandas DataFrame.</li>
    </ul>
    <h3><code>ClassSchedule</code></h3>
    <ul>
        <li><code>set_class(timetable, day, time_slot, course_code, course_title, teacher_name)</code>: Assigns a class to the timetable.</li>
    </ul>
    <h3><code>OnlineClass</code> (inherits from <code>ClassSchedule</code>)</h3>
    <ul>
        <li><code>get_class_info()</code>: Gets information about the class.</li>
    </ul>
    <h3><code>DateHelper</code></h3>
    <ul>
        <li><code>get_current_date()</code>: Returns the current date.</li>
    </ul>
    <h3><code>ClassInfo</code> (inherits from <code>TimetableGenerator</code>, <code>Day</code>, <code>DateHelper</code>)</h3>
    <ul>
        <li><code>display_info()</code>: Displays the timetable based on user choice.</li>
    </ul>
    <h3><code>TimetableIterator</code></h3>
    <ul>
        <li><code>__iter__()</code>: Returns the iterator object.</li>
        <li><code>__next__()</code>: Returns the next item from the timetable.</li>
    </ul>
    <h3><code>TimetableAnalysis</code></h3>
    <ul>
        <li><code>count_free_slots()</code>: Counts free slots in the timetable.</li>
        <li><code>free_slots_withNumpy()</code>: Uses NumPy to count free slots.</li>
    </ul>
    <h3><code>TimetableLambda</code></h3>
    <ul>
        <li><code>is_slot_available(day, slot)</code>: Checks if a slot is available using a lambda function.</li>
    </ul>
    <h3><code>ClassCodes</code></h3>
    <ul>
        <li><code>add_class(code, title)</code>: Adds a class code and title.</li>
        <li><code>get_all_classes()</code>: Returns all class codes and titles.</li>
        <li><code>update_class_codes(timetable)</code>: Updates class codes based on the timetable.</li>
    </ul>
    <h3><code>LoginSystem</code></h3>
    <ul>
        <li><code>validate_section(section)</code>: Validates the section format.</li>
        <li><code>ask_for_section()</code>: Prompts the user to enter their section.</li>
        <li><code>ask_for_role()</code>: Prompts the user to enter their role.</li>
    </ul>
    <h2>Example Usage</h2>
    <ol>
        <li><strong>Login</strong>: Enter your section and role.</li>
        <li><strong>Manage Timetable</strong>: Depending on your role, you can assign or remove classes.</li>
        <li><strong>View Timetable</strong>: Display the timetable in different formats and view it iteratively.</li>
        <li><strong>Data Analysis</strong>: Use Pandas and NumPy for timetable data manipulation.</li>
    </ol>
    <h2>Contributing</h2>
    <p>Feel free to contribute to this project by opening issues or submitting pull requests. Please ensure your contributions align with the project's overall goals and coding standards.</p>
    <h2>License</h2>
    <p>This project is licensed under the MIT License. See the <a href="LICENSE">LICENSE</a> file for more details.</p>
    <h2>Contact</h2>
    <p>For any inquiries or feedback, you can reach out to me at <a href="mailto:your.email@example.com">your.email@example.com</a>.</p>
</body>
</html>
