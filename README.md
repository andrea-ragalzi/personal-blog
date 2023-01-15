# personal-blog 
A blog made following pymike00's Flask course.

Link repository del corso Flask che ho seguito:

https://github.com/pymike00/codingwiz-dev


### Istruzioni installazione 

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
