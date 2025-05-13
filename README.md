# inst326-exercise-6--enron-analysis-solved
**TO GET THIS SOLUTION VISIT:** [INST326 Exercise 6- Enron Analysis Solved](https://www.ankitcodinghub.com/product/inst326-exercise-6-enron-analysis-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93583&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;INST326 Exercise 6- Enron Analysis Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
# Background

For this homework assignment, you will parse through a set of 10,000 emails for the purpose of pre- analysis processing. These emails are a sample from a collection of around 500,000 emails known as the “Enron Email Dataset”. This dataset contains emails sent by employees of Enron after the collapse of the company. The entire dataset can be found here: https://www.kaggle.com/wcukierski/enron-email-dataset

In order to parse an email, you must first be familiar with the structure of emails. When we send emails we are not only sending heading and body content information, we are also sending metadata that describes the email structure in detail. This is known as the “header” and will contain data relating to the sender, receivers, CC information, routing information, etc. This header is formatted enough that we can use regular expressions in order to identify the information that we are interested in.

# Instructions

– Your script should be named enron.py.

– Your script should contain two classes, Server and Email. At the end of the script should be an if **__name__ == “__main__”:** statement. Specifications for each of these required program elements are given below. You may write additional classes, methods, and/or functions if you wish.

– The name of your files should consist exclusively of lower-case letters, numbers, and underscores, and the file extension .py. Your filename should not start with a number.

– Your script MUST contain docstrings.

– You should place the text file in the same directory as your python script.

# Server class

**Functionality**

– This class stores the data for all emails found in the dataset.

**Attributes**

– emails: A list of email objects where each object corresponds to one email.

**Methods**

– __init__()

– Parameters

– Self

– Path – The path to the file that we are going to read. In this case, the path we are passing in will be the __emails_10k.txt__ file, however, this should not be hardcoded in.

– Functionality

– The init method should open the file specified by the path for reading and set the emails attribute to a list containing Email objects. Each email instance should correspond to each individual email found in the text file.

&gt; HINT: In order to do this the first step is to create a list where each element in the list is an entire email. Take a look at the file and how the emails are separated from each other. You do not need to write any regular expressions in order to complete this part. Instead, you can use methods that are built into the string class. Once you have that list you can then iterate through the list and write regular expressions that will identify each of the elements of interest in each email(message id, date, subject, sender, receiver, and body text). You must use regular expressions in order to do this.Keep in mind that each of these elements will be represented by strings. However, none of these elements should contain information that does not pertain to it. For example, the date attribute of an email class should not contain anything in it that is not a date.

# Email class

**Functionality**

– This class stores the data related to individual email messages.

**Attributes**

– message_id: The message-id that is unique to each email message. Represented as a string.

– date: The date associated with each email message. This date does not need to be formatted in any way but it must contain only date or time information. Represented as a string.

– subject: The subject of each email message. Represented as a string.

– sender: The sender of each email message. Represented as a string.

– receiver: The receiver of each email message. Represented as a string.

– body: The body message of each email message. Represented as a string.

**Methods**

– __init__()

– Parameters

– self

– message_id – A string representing the message_id

– date – A string representing the date of the email.

– subject – A string representing the subject of the email.

– sender – A string representing the email address of the sender.

– receiver – A string representing the email address of the receiver.

– body – A string representing the body text of the email.

– Functionality

– Sets the parameters to the corresponding attributes.

# main()

**Parameters**

– Path, a string that represents the path of the text file that will be parsed.

**Functionality**

– Create an instance of server-class using the path that was passed in and save that to a variable.

**Returns**

– An integer, the length of the emails attribute of that instance.

# parse_args()

– Parse_args function

– Parameters

– args_list: a list of strings containing the command-line arguments for the program (when you call this program, you will pass sys.argv[1:] as the argument for this parameter)

– Functionality

– Create an instance of the ArgumentParser class from the argparse module

– Use the add_argument() method of your ArgumentParser instance to add the following arguments:

– Required arguments (i.e., the user can’t run the program without specifying these):

– the path to the text file (as a str)

&gt; NOTE: You will need to import argparse and sys, or at least parts of these modules, in order for this function to work properly. Remember, import statements belong at the top of your script, right after the script docstring.

– Returns

– The ArgumentParser object created.

# if __name__ == “__main__”:

– pass sys.argv[1:] to parse_args() and store the result in a variable

– call the main() function; pass in the path using the values extracted from the command line arguments by your parse_args() functionFor ease of use make sure that the text file is in the same directory as your script.

# Running your program

– Your program is designed to run from the terminal. To run it, open a terminal and ensure you are in the directory where your script is saved.

– The program takes at least one command-line argument: the name of the text files (which are books) that you want to process using your script. Below are some examples of how to use the program. The examples assume you are using a Unix based OS (macOS, Linux) and your program is called enron.py. If you are using Windows, replace python3 with python.

&gt; NOTE: python3 enron.py enron_10k.txt
