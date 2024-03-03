# How use it again

### Run following commands:
* git clone https://github.com/miromannino/Contributions-Importer-For-Github.git
* pipenv install
* pipenv shell

* Create run_script.py file in the Contributions-Importer-For-Github directory
Add this lines of codes:

import git

from src import *

repo = git.Repo("/var/www/link-cushion/")

mock_repo = git.Repo("/var/www/mock-repo")

importer = Importer([repo], mock_repo)
importer.set_author(['yuratadevosyan01@gmail.com', 'yuratadevosyan01@gmail.com'])
importer.import_repository()

* python3 run_script.py
* Delete Contributions-Importer-For-Github directory and push
