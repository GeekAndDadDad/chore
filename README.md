# chore
Many hands make light work
Everything is a chore, but project management shouldn't be
If we make this a business, it'll probably be called the Choring Company
Our website is chore.us
Join the Chore Us!

Chore is a window into what we are already doing, plus annotation and structure.

The Chore Graph is a DAG.

Each Chore has:
  - chore name, ideally no more than three words lowercase, and three syllables max desirable
  - an ordered list of sub-chores
  - an ordered list of parent chores
  - a status: not yet started, started, complete

 Chores may also have such things as:
  - a link to the work product of the chore
  - a detailed description of the chore, purpose, and goal condition
  - a targeted start and/or completion date, either specified or derived
  - an estimated time of completion, either specified or derived
  - a list of chore dependency references (this chore can't start until dependencies are complete)
  - sections (chores that end in ':')
  - owner (responsible party)
  - executive champion
  - tags
  - watchers
  - ordered list of chore references
  - access rights (default to inherited)
  - budgets and anything else

The Chore Graph is the primary data structure of chore:
  - Every project is a chore
  - Every task is a chore
  - Every department is a chore
  - Every team is a chore
  - Every user is a chore
  - Every milestone is a chore
  - Every process is a template chore tree

Chore is currently envisiond as a single-screen web user interface divided into four quadrants: the Flag, the Stop, the Run, and the Kick.

Main screen: resizable four quadrant UI

The Flag:
  - The Flag is the Chore browser
  - Upper left quadrant
  - Flag explores a "root" chore
      - "Headline" is bubble buttons of root's parent chores' names "/" root chore name 
  - Key metaphor: entering a tree of chores should be as fast as writing a to-do list in TextEdit or NotePad
  - Chore broser is expandable tree of sub-chores
  - Standard list text entry
      - CR creates new chore below current chore line
      - Tab indents current chore to sub-chore of previous sibling chore
      - Shift-tab moves current chore out to sibling of parent chore in browser
      - "@username " assigns username chore as chore owner, erases "@username "
      - "#hashtag " adds hashtag to tag list, erases "#hashtag "
      - "chore name:" makes that chore a section grouping
  - Clicking a chore selects that chore, places its details in the Stop, and its work product in the Kick
  - Right click menu
      - open chore as root in new tab
      - copy chore
      - paste subchore
  - L/R arrow keys or clicking within a selected chore edits that chore name
  - shift-down/up arrow expand/collapse sub-chores
  - ctrl-down/up arrow moves currently selected chore down or up within parent's sub-chore list

The Stop:
  - The Stop displays and allows the editing of an individual chore's details

The Kick:
  - The kick is an iFrame for the work product link of the chore

The Run:
  - The Run is the history and conversation log of the chore. Think Slack channel on the root chore.
  - All changes in the stop logged
  - Text conversation about the root chore
  - At the top of the run is the chatter - think Clubhouse
      - Speaker/mic buttons, bubbles for all users currently on that chore root
  
