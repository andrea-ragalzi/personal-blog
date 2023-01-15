# personal-blog 
A blog made following pymike00's Flask course.

Repository link for the Flask course I took:  

https://github.com/pymike00/codingwiz-dev  


### Local installation instructions

git clone https://github.com/andrea-ragalzi/personal-blog.git  
cd  personal-blog  
python3 -m venv venv  
source venv/bin/activate  
pip install -r requirements.txt  
flask db upgrade  
flask shell  
from blog.models import User  
u = User(username="admin", email="email@provider.com")  
u.set_password_hash("your-secret-psw")  
db.session.add(u)  
db.session.commit()  
quit()  
flask run  
