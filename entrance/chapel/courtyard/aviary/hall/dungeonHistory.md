   28  cd 301
   29  git clone https://github.com/data301-2020-winter2/data301-lab2-Ogo-O.git
   30  ls
   31  cd data301-lab2-Ogo-O
   32  ls
   33  cd entrance
   34  ls
   35  cat scroll
   36  ls
   37  cat scroll
   38  cat scroll
   39  git add breadcrumps.txt
   40  nano breadcrumps.txt
   41  cd 301
   42  ls
   43  cd data301-lab2-Ogo-O
   44  ls
   45  cd entrance
   46  ls
   47  cat scroll
   48  echo "Ogo, been here" >> breadcrumps.txt
   49  git add breadcrumps.txt
   50  git commit -m "Wubba Lubba Dub Dub"
   51  git push
   52  cd cellar
   53  ls
   54  cat scroll
   55  alias ls='ls -F'
   56  ls
   57  cat treasure
   58  cd armoury
   59  ls
   60  cat scroll
   61  ./treasure
   62  export I=sword,$I
   63  echo $I
   64  echo "Ogo, been here" >> breadcrumps.txt
   65  git add breadcrumps.txt
   66  git commit -m "Picked up sword"
   67  git push
   68  cd ..
   69  ls
   70  ./treasure
   71  export I=amulet,$I
   72  echo $I
   73  cd armoury
   74  ls
   75  ./potion
   76  export HP=15
   77  echo $HP
   78  ls
   79  cd chamber
   80  ls
   81  cat scroll
   82  pwd
   83  ./spell
   84  ln -fs ../../../chapel/courtyard/aviary/hall portal
   85  ls
   86  ./treasure
   87  export I=coins,$I
   88  echo $I
   89  ./statue
   90* echo  breadcrumps.txt
   91  echo "Ogo has been here" > breadcrumps.txt
   92  git add breadcrumps.txt
   93  git commit -m "This is where we encounter the chamber"
   94  git push
   95  ls
   96  ./statue
   97  ls
   98  cd portal
   99  ls
  100  cd library
  101  ls
  102  cat scroll
  103  ls
  104  ./tome
  105  ls
  106  cd..
  107  cd ..
  108  git add breadcrumps.txt
  109  echo "Ogo has been here." > breadcrumps.txt
  110  git add breadcrumps.txt
  111  git commit -m "About to fight boss after entering portal"
  112  git push
  113  ls
  114  ./monster
  115  ls
  116  ./carcass
  117  ./treasure
  118  export I=crown,$I
  119  echo $I
  120  echo "Ogo has been here" > breadcrumps.txt
  121  git add breadcrumps.txt
  122  git commit -m "I have slain the beast and have the crown"
  123  git push
  124  git add .
  125  git commit -m "Finished playing with the dungeon"
  126  git push
  127  history 100 > dungeonHistory.md
