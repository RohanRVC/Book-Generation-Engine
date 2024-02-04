# Book-Generation-Engine

System Design Architecture -:
![image](https://github.com/RohanRVC/Book-Generation-Engine/assets/80825254/3113406a-0b57-4d6b-83b2-2fdbfc26fb47)

* Input  :
When the user logs into the application, they can make the following choices:

Genre: The genre of the book they wish to read (e.g., Romance, Mystery, Fantasy, etc.)
Language: The language in which they want the book (e.g., English, Spanish, etc.)
Title: An optional title they have in mind for the story.
Brief Description: A summarized storyline in 20 to 30 words, like "A boy and a girl fall in love despite their families being at odds."
Length of Book: The desired length of the book (e.g., Short, Medium, Long).
For example:

Genre: Romance
Language: English
Title: (if any or left blank)
Brief Description: "A boy and a girl fall in love despite coming from rival families."
Length of Book: Medium


* Output:
Initial Summary Generation:

Use abstractive summarization techniques to create a brief yet comprehensive initial summary based on the user-provided brief description.
E-Book Content Generation:

Utilize advanced text generation models like GPT-3 or fine-tuned LSTMs to produce high-quality text based on user-provided genre, language, and brief description.
Chapter and Section Division:

Implement NLP techniques to identify logical breaks in the narrative for chapter divisions.
Automated Title Generation:

A smaller text generation model can be used to generate a title based on the brief description provided by the user. The model can be trained on pairs of book summaries and titles to learn this specific task.
Formatting and Cover Page Design:

Utilize automated document formatting libraries to create the Table of Contents and layout. For cover page design, you can use pre-set templates and algorithms that arrange elements based on the genre and potential title.
Preview and Finalization:

The first chapter can be separated programmatically and presented to the user for a preview before downloading the entire e-book.
Download Options:

The formatted e-book can be converted into multiple formats like PDF, ePub, etc., using relevant libraries.
Feedback Loop:

Implement a simple star-rating and comment system that feeds back into a database for future model training and improvement.
