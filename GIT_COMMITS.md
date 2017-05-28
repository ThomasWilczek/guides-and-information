# Commiting correctly

The naming scheme should be "TAG: MESSAGE (#ISSUE)", and the commits should contain
everything that's logically connected to itself. So group the changes according to that.

*For example, all tests for a feature in **one** commit.*

But: when you have a large commit, that is meant to close an issue, write a longer
commit message. List the changes and why you made them. This isn't meant as documentation, it's meant
to be an overview. So don't write an essay, write a table of contents with quick summarys.
Also, the why is more important than the how when you write a commit message.

If you are making any style changes or rename variables, turning it into a "fixup" commit for
the part you corrected would prevent our commit history from bloating up with minor changes.

So, what should you do if you already f'ed up?  
Well, there's two scenarios:

## Scenario 1 -- Local fu*k up

When you f up on your local system it's not that bad, for example, you can just
`git rebase -i HEAD~1` to drop, rename or change your last commit.
When you f'ed up earlier than that just change the number to include more commits.
This way you can for example reorder the commits, squash them or use them as a fixup.

## Scenario 2 -- Pushed fu*k ups

Well, you f'ed it up hard now, didn't you? Probably already opened a pr?
Dude, that's not cool. Now let me show you how to solve this problem!

When you don't care about anything, close the pr, rebase locally and then force
push the corrected commits. So, pretty simple, just like above only that you're
going to give me a headache.

You could also open another branch, cherry-pick the commits you want and then
push again and open a new pr. All valid options.

## Conclusion

Well, try not to fu\*k up please. Commit is not a random word chosen for the code piles you throw at us.
You **commit** to the code. When you commit you tell everyone that you are sure it's correct.
So please, don't just commit because you can, but because you are sure of what you did.

But then again, you can always squash...
