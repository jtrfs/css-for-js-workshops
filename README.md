# About the workshops | MAIN BRANCH

#### Josh says:

> _Workshops are **real-world-inspired problems**. The project and its goals are described in depth in the project's README file, though you'll be given the gist of the project here in the course materials. You might not be able to solve the workshop, and that's OK. Some workshops are super challenging. **It's about the journey, not the destination**._

#### Here's the recommended path:

1. If you get stuck or don't know how to proceed, you can **review the lessons** in this module.
2. Spend up to **2 hours working on the problem**. If you get discouraged or frustrated, you can stop earlier!
3. After you've invested a good chunk of time into the problem, **watch the solution video** (embedded in the next lesson). I'll show you how I'd approach this problem.

> _Note that there are **many valid solutions** for most workshops; your solution might look quite different than mine, but that doesn't mean you did it wrong! As we went over in the onboarding video, though, you don't have to follow this approach! If you'd prefer, you can code along with the video. Or you can bounce between coding and watching the solution. This **course is for you**._

> _Once you're finished with the workshop (regardless of whether you've completed the exercises or not), you can **submit the link** to your solution. This is mainly to serve as an accountability tool. On occasion, I'll go through the submissions to see broadly where people are struggling, but **I don't offer individual reviews**._

## WORKSHOPS

| No. | Workshop's Name  | Status | My Branch            | Solution |
| :-: | :--------------- | :----: | :------------------- | :------- |
|  1  | Huckleberry      |   ✅   | [hucklebery]()       |          |
|  2  | Create Character |   ✏️   | [create-character]() |          |
|  3  |                  |        |                      |          |
|  4  |                  |        |                      |          |
|  5  |                  |        |                      |          |

---

## Structure of my repo/workflow

#### 1 Connecting local & remote repositories

I am creating one repository, done locally and then remotely through [gh cli](https://github.com/cli/cli). The idea is to have only one repo and then several different branches, each for individual workshop. I am also using`oh-my-zsh` (omz).

- **`take css-for-js-workshops`** ...create the folder and cd into it (omz)
- **`git init`** ... local git repository initialised
- **`gh repo create`** ...create a remote repo and add an 'origin' remote to my local repository
- now, I have to create some content, eg _README_ and _.gitignore_ files
- **`git add --all`** and **`git commit -m "some_message"`** or with the help of omz git plugin I just type: **`gaa`** and **`gcmsg "some_message"`**
- **`git push -u origin main`** ...the local and remote are 'connected'

#### 2 Cloning Josh's repos

I am going to **clone** one repo/task/project/workshop at a time.

- **`git clone <repo_url>`** ... cloning the repo

#### 3 Changing the repo's url

Then I have to change the repo's remote url for my own remote url.

- **`git remote`** ... checking the remote's name (usually 'origin')
- **`git remote remove origin`** ... the remote removed
- **`git remote add origin <new_url>`** ... the new remote added

#### 4 Coding ... at last 🤪

Now, I can start working on the projects/tasks ... it means **`npm install`** and then possibly **`npm start`**.
Don't forget about regular **`git add`**, **`git commit`**, **`git push`**. Everything must by committed, especially if you are working on multiple branches.
Also remember to add _.gitignore_ file, node_modules folder is not necessary since we can always use **`npm install`** command.
