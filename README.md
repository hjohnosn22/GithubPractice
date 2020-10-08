# GithubPractice
Q1 - What does clone set the variable origin to represent?

It sets the variable origin to represent main.

Q2 - What does the command git push --set-upstream origin master do? What does remote tracking mean in this context?

It sets the main branch as the upstream branch (--set-upstream is the same as -u). Remote tracking means...

Q3 - Explain and illustrate what's happening in the commit tree when this command executes.

Q4 - Are your commits overwritten by the remote master?

Q5 - Is this a merge or a rebase?

Q6 - Person B: checkout the local master branch. Is it updated as well, or still behind remote master?

Q7 - Run git branch. Did your local copy of your branch delete when Person A deleted the remote branch?

Yes.

Q8 - Use git log --graph --all to view the branching structure and copy and paste the result into the README.md formatted as a code segment (see markdown cheatsheet).


Results of git log --graph --all (some of it, it was very very long)

```
*   commit 12c82b1c1c7b6d90d709a8b373264dad48556594 (HEAD -> main, origin/main, origin/HEAD)
|\  Merge: 3112386 a873203
| | Author: Henry Johnson <46233024+HunkyHank1@users.noreply.github.com>
| | Date:   Thu Oct 8 10:17:47 2020 -0600
| | 
| |     Resolve merge conflict.
| |   
| *   commit a873203d791b6ed0f9183fc806683a8d225056d7
| |\  Merge: 781633f 1505548
| | | Author: MDerv <dsharma21@kentdenver.org>
| | | Date:   Thu Oct 8 10:13:27 2020 -0600
| | | 
| | |     Q1 done
| | | 
| * | commit 781633ffab87f315d7c9ab9e6291f29cd5e6c797
| | | Author: MDerv <dsharma21@kentdenver.org>
| | | Date:   Thu Oct 8 10:12:54 2020 -0600
| | | 
| | |     Q1 done
| | |   
* | |   commit 3112386a602d78d65fd28a639a89359fcce34d62
|\ \ \  Merge: 1505548 151fc9a
| |_|/  Author: Henry Johnson <46233024+HunkyHank1@users.noreply.github.com>
|/| |   Date:   Thu Oct 8 10:15:47 2020 -0600
| | |   
| | |       Resolved merge conflict w/ text.txt
| | | 
| * | commit 151fc9a00e423cf518ba22cda539140672fb1af7 (origin/feature2)
| | | Author: Henry Johnson <46233024+HunkyHank1@users.noreply.github.com>
| | | Date:   Thu Oct 8 10:03:15 2020 -0600
| | | 
| | |     text.lame
| | |   
* | |   commit 150554876f2db1459b1d2c80cb6fa2a8f211ac27
|\ \ \  Merge: b8f904a 7d1665b
| | |/  Author: Addison Hoff <addisonhoff@addisons-air.kentdenver.org>
| |/|   Date:   Thu Oct 8 10:07:12 2020 -0600
| | |   
| | |       changed text in text.txt
| | | 
| * | commit 7d1665b94f7b90e0a57555cea69049d061f61c87
| | | Author: MDerv <dsharma21@kentdenver.org>
| | | Date:   Thu Oct 8 10:02:33 2020 -0600
| | | 
| | |     I added the questions
| | | 
* | | commit b8f904a9d32b006ad844fa189115adc920d0ecb0
|/ /  Author: Addison Hoff <addisonhoff@addisons-air.kentdenver.org>
| |   Date:   Thu Oct 8 10:04:47 2020 -0600
| |   
| |       edited text.txt
| |   
* |   commit 59ba928e960174207f4ec7919ea7a1fe4acdb16c
|\ \  Merge: 17b5888 5083939
| | | Author: MDerv <dsharma21@kentdenver.org>
| | | Date:   Thu Oct 8 09:55:49 2020 -0600
| | | 
| | |     Merge branch 'main' of https://github.com/hjohnosn22/GithubPractice into main
| | |   
| * |   commit 5083939d3d2421e6ca49d60166849b942254ffec
| |\ \  Merge: e59c3b7 9e9d6e6
| | |/  Author: hjohnosn22 <71099361+hjohnosn22@users.noreply.github.com>
| | |   Date:   Thu Oct 8 09:53:42 2020 -0600
| | |   
| | |       Merge pull request #2 from hjohnosn22/feature2
| | |       
| | |       Added text.txt
| | | 
| | * commit 9e9d6e69114ad05e05bb37cddbf3968c1ca81f91
| | | Author: Henry Johnson <46233024+HunkyHank1@users.noreply.github.com>
| | | Date:   Thu Oct 8 09:51:50 2020 -0600
| | | 
| | |     Added text.txt
| | |   
* | |   commit 17b5888b90b20a072f17d50e011f786f5cef4de5
|\ \ \  Merge: 1a779c6 e59c3b7
| |/ /  Author: MDerv <dsharma21@kentdenver.org>
| | |   Date:   Thu Oct 8 09:55:44 2020 -0600
| | |   
| | |       ANOTHER COMMIT POG
| | | 
| * | commit e59c3b78677621c5dc5212f6530745da8cb2a8b8
| | | Author: hjohnosn22 <71099361+hjohnosn22@users.noreply.github.com>
| | | Date:   Thu Oct 8 09:47:16 2020 -0600
| | | 
| | |     that branch was not the coolest
| | |   
| * |   commit 3e8efac9992279f8e4f21af5c850c1812ea31558
| |\ \  Merge: 737fa29 1350152
| | | | Author: hjohnosn22 <71099361+hjohnosn22@users.noreply.github.com>
| | | | Date:   Thu Oct 8 09:46:27 2020 -0600
| | | | 
| | | |     Merge pull request #1 from hjohnosn22/aBranch
| | | |     
| | | |     Added the coolest branch ever. You should definitely merge this branch!
| | | | 
| | * | commit 13501528f311cfaeb023e509912265cc1fd664f7 (origin/aBranch)
| |/ /  Author: Addison Hoff <addisonhoff@addisons-air.kentdenver.org>
| | |   Date:   Thu Oct 8 09:41:36 2020 -0600
| | |   
| | |       Added the coolest branch ever.
| | | 
* | | commit 1a779c6c58bcca6b18d5f9616066e1c0601d783d
|/ /  Author: MDerv <dsharma21@kentdenver.org>
| |   Date:   Thu Oct 8 09:48:31 2020 -0600
| |   
| |       WOW ANOTHER EDIT POG
```
