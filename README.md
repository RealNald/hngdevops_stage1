# hngdevops_stage1
devops stage1 personal api

A simple API deployed on a VPS with Nginx reverse proxy and systemd.

## for Local Setup
follow the guide below and u should be able to achieve the same results

git clone https://github.com/RealNald/hngdevops_stage1.git 
cd your-repo
python3 -m venv venv
source venv/bin/activate
pip install flask
python app.py

open a new terminal and paste these commands
curl http://localhost:5000/
curl http://localhost:5000/me
curl http://localhost:5000/health

to stop go back to the previous terminal and 
press control C to stop th python process.

to edit the app.py file
nano app.py and change the names to your desired state.
and you should have similar outputs.

**ENDPOINTS**
endpoints    method         response
    /	        GET       	{"message": "API is running"}
/health	      GET        	{"message": "healthy"}
/me	          GET       	{"name": "Your Name", "email": "you@example.com", "github": "https://github.com/yourusername"}
