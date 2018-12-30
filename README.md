# Certificate of Attendance Auto Generator

Automatically generates certificate image based on attendee names provided (reads from CSV file), and contains script that will automatically send the generated certificate to intended recipients using Outlook Application.

## Script Settings

Make sure that you update the script settings from [main.py](https://github.com/prtdomingo/certificate-of-attendance-auto-generator/blob/master/main.py) based on your needs:

```python
# Script Settings
isDebug = True # Setting this into True will prevent the script to send the actual email to intended recipients
attendee_list = csvr.read_csv("src/csv/ListOfAttendees-Test.csv") #
template_path = "src/template/example-template.png" # Specify email template path
imageWxH = (1360, 1024)
font = cv2.FONT_HERSHEY_SIMPLEX
fontScale = 2
fontColor = (0,0,0) # Black
lineType = 2
```

