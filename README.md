# secure-s3-lab

Created public bucket, removed access and tested files before and after
<img width="954" height="576" alt="image" src="https://github.com/user-attachments/assets/26b70b00-a776-4834-8503-806be098e557" />
Initial creation of bucket above^
Removing and readding access easy enough, both processes acted as should have. SC of both attatched below 
<img width="641" height="298" alt="image" src="https://github.com/user-attachments/assets/017dadb3-f40c-4259-9d0b-52cd744fc1ac" />
Permissions ON, all access blocked. Resulting in following when trying to open simple link 
<img width="958" height="152" alt="image" src="https://github.com/user-attachments/assets/ccca45ab-9871-4193-ba8e-ba4ff1788767" />
Now turning permissions OFF, public access allowed
<img width="640" height="289" alt="image" src="https://github.com/user-attachments/assets/8a9285d2-1f69-46ef-b07b-5b258115d800" />
Now link is able to be opened, resulting in file opening without access denied 
<img width="956" height="112" alt="image" src="https://github.com/user-attachments/assets/b35b7ccd-15d4-4e54-b897-39f8cbd7d053" />
Made sure to check encryption on bucket, default is set to SSE-S3. No further changes to be made 
<img width="954" height="514" alt="image" src="https://github.com/user-attachments/assets/3300ddab-dace-4b9a-a425-11d59143c30a" />
Began the process for adding log checking by first creating a bucket where the logs would be stored 
<img width="1081" height="233" alt="image" src="https://github.com/user-attachments/assets/0ab3801a-1ee6-4056-b110-f41b938f30ad" />
Configured original bucket to log these files in the NEW bucket that was created
<img width="1596" height="380" alt="image" src="https://github.com/user-attachments/assets/76271b16-5c71-4d1f-9447-ff5dd887810a" />
After creating log bucket, turned off public access and tried to open simple text document to replicate someone unwanted trying to access the document. From here, i searched through the .JSON file for "AccessDenied" to see if this was logged
<img width="1920" height="940" alt="image" src="https://github.com/user-attachments/assets/b8666574-63ef-4898-9115-f1e88753f581" />
To be thorough, i also did the same after setting the access to public to see what the files looked like when someone had access. I found this by searching for "GetObject"
<img width="1920" height="939" alt="image" src="https://github.com/user-attachments/assets/1234891e-f47d-4405-b297-e1a46bb7ed9c" />
After setting up, curiosity got the better of me and i learnt how to configure an alarm in the event someone tried to access the file, so that you wouldn't need to manually search through the .JSON docs
<img width="827" height="544" alt="image" src="https://github.com/user-attachments/assets/bc2191ac-d6b0-45a8-940a-2a78f6111184" />

