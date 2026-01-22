# TikTok Video Upload - Test Cases

## Test Case 1
**Test Case ID:** TC_Video_Length_Short_001
**Title:** Video_Length_Too_Short_Test
**Requirement:** Invalid: Video_Length < 3 Sec
**Test Type:** Negative 
**Preconditions:** User is logged in and has filmed a video
**Test Steps:** Step 1: Check the video length to see if it is less than 3 seconds.
**Test Data:** The video length
**Expected Result:** The video doesnt upload and displays a video too short message.
**Priority:** High

## Test Case 2
**Test Case ID:** TC_Video_Length_In_Range_002
**Title:** Video_Length_Range_Test
**Requirement:** Valid: 3 sec ≤ Video_Length ≤ 600 sec
**Test Type:** Boundary
**Preconditions:** User is logged in and has filmed a video
**Test Steps:** Step 1: Check the video length to see if is 3 seconds or more. Step 2: Check the video length to see if is 600 seconds or less. 
**Test Data:** The video length
**Expected Result:** The video uploads and displays a message confirmation of upload. 
**Priority:** High

## Test Case 3
**Test Case ID:** TC_Video_Length_Long_003
**Title:** Video_Length_Too_Long_Test
**Requirement:** Invalid: Video_Length > 600 sec
**Test Type:** Negative
**Preconditions:** User is logged in and has filmed a video
**Test Steps:** Step 1: Check the video length to see if it is more than 600 seconds. 
**Test Data:** The video length
**Expected Result:** The video does not upload and displays a message stating the video is too long. 
**Priority:** High

## Test Case 4
**Test Case ID:** TC_File_Correct_Format_004
**Title:** File_Correct_Format
**Requirement:** Valid: File_Type in MP4
**Test Type:** Positive 
**Preconditions:** User is logged in and has filmed a video of acceptable length 
**Test Steps:** Step 1: Check the files type format is of the acceptable file format.
**Test Data:** The files format type 
**Expected Result:**  The video uploads and displays a message confirmation of upload. 
**Priority:** High

## Test Case 5
**Test Case ID:** TC_File_Size_005
**Title:** File_Size_Min_Test
**Requirement:** Valid: 1 byte ≤ File_Size
**Test Type:**  Boundary
**Preconditions:** User is logged in and has filmed a video of acceptable length and format
**Test Steps:** Step 1: Check the files type format is or above the file size minimum. 
**Test Data:** The file size
**Expected Result:** The video uploads and displays a message confirmation of upload. 
**Priority:** High

## Test Case 6
**Test Case ID:** TC_File_Empty_Caption_006
**Title:** Video_Empty_Caption_Test
**Requirement:** Captions are optional for videos
**Test Type:**  Edge
**Preconditions:** User is logged in and uploading a valid video
**Test Steps:** Step 1: Check the videos caption to see if there is anything.
**Test Data:** The caption length 
**Expected Result:** The video uploads and displays a message confirmation of upload. 
**Priority:** Low

## Test Case 7
**Test Case ID:** TC_File_Corrupted_007
**Title:** File_Corrupted_Test
**Requirement:** File integrity validation
**Test Type:** Edge
**Preconditions:** User is logged in and has filmed a video of acceptable length, format, and size
**Test Steps:** Step 1: Checking that the video is showing a preview 
**Test Data:** File Integrity
**Expected Result:** The video upload fails and is unable to processed showing an error message
**Priority:** High

## Test Case 8
**Test Case ID:** TC_Video_Privacy_Settings_008
**Title:** Video_Privacy_Test
**Requirement:** Checks to see if the video is private (only the user can see the video)
**Test Type:**  Black Box
**Preconditions:** User is logged in and is uploading a valid video in the correct format, length, and size
**Test Steps:** Step 1: Check to see if the user made the video priavte as in only accessable to them
**Test Data:** The users privacy settings on the video
**Expected Result:** The video uploads priavtely where only the user access to it
**Priority:** High

## Test Case 9
**Test Case ID:** TC_Video_Comment_Permissions_009
**Title:** Video_Comment_Permissions
**Requirement:** Checks to see if comments are allowed on the post
**Test Type:**  Black Box
**Preconditions:** User is logged in and has uploaded a valid video in the correct format, length, and size
**Test Steps:** Step 1: Check the users settings for the video to see if the user allowed comments on it
**Test Data:** The videos comments
**Expected Result:** The video uploads but does not allow other users to comment on the video.
**Priority:** Meduim

## Test Case 10
**Test Case ID:** TC_Video_Correct_Aspect_Ratio_010
**Title:** Video_Aspect_Ratio_Test
**Requirement:** Valid: Aspect ratio is 9:16
**Test Type:** Positive
**Preconditions:** User is logged in and has filmed a video of acceptable length, format, and size
**Test Steps:** Step 1: Check the aspect ratio of the video 
**Test Data:** Aspect ratio of the video
**Expected Result:** The video uploads and displays a confirmation message
**Priority:** Meduim