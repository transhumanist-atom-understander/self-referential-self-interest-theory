# An argument of Parfit's reconsidered with logical decision theory
A _logical decision theory_ [recommends that you choose as if deciding the output of your decision algorithm](https://www.lesswrong.com/w/logical-decision-theories?lens=introduction-to-logical-decision-theory-for-analytic#Logical_decision_theory).

The main difficulty in formulating a logical decision theory is how to define statements like: "If my algorithm outputs this, the result will be that".
These look like counterfactual implications, but counterfactuals describe possible worlds with different contingent facts.
What our decision algorithm outputs (with given input) is a logical fact, and it is not clear what it means to say what would happen if a logical fact were different.
Much theoretical work has gone into elaborating this kind of _counterpossible_ implication, without, in my opinion, satisfactory results.

But what's the point of this theoretical work?
Do we really need LDT?

What's the difference between choosing the output of your decision algorithm and just making a choice?
There is no difference, as long as your choice is the only thing in the world that depends on your decision algorithm.
The only substantial applications of LDT are games where the player's environment contains some other implementation of the algorithm.
The central example is Newcomb's problem.

But Newcomb's problem sounds like a science fiction story, and I'm not convinced by [the case that analogous problems are part of our normal social lives](https://www.lesswrong.com/posts/puutBJLWbg2sXpFbu/newcomblike-problems-are-the-norm).

But leaving aside the prospect of applying LDT to real life, I do think it's important in philosophy.
In this post I'm going to share an example that came up when I was reading Derek Parfit's _Reasons and Persons_.
It's an argument that Parfit makes where LDT seems conspicuously missing.
Like, if you were familiar with it, you would have gone in a different direction.

Derek Parfit's book introduces a zoo of theories of morality and rationality, which he refers to by single-letter acronyms.
In the first part of the book (all I've read to be honest), he describes how these theories can be self-defeating, introducing a taxonomy of the varieties of self-defeat.

The basic principle of LDT becomes applicable when Parfit introduces "collective self-defeat".
This variety of self-defeat depends on the outcome when multiple players are deciding according to the same theory.
Because you know the other players are deriving their decisions from the same theory as you are, a philosophical move inspired by LDT yields interesting results.

## Parfit's claim: S is collectively self-defeating

I'm going to use a single argument of Parfit's as an example.
The subject of the argument is the self-interest theory ($S$), which he says is a theory of rationality.
(Since this is LessWrong, I must add that he doesn't mean [what Yudkowsky means by "rationality"](https://www.lesswrong.com/posts/HcCpvYLoSFP4iAqSz/rationality-appreciating-cognitive-algorithms), but I don't think that's important for this argument.)

What we need to know about $S$ is that it prescribes an aim, which is that your life go as well as possible, as well as what I'll call a policy: it recommends taking the actions that make your life go as well as possible, among the available alternatives.

Parfit argues that $S$ has the property of being _collectively self-defeating_: that is, if we all follow $S$, then we will do worse by our $S$-given aim than if we had all taken other actions.

(Actually, _directly_ collectively self-defeating, but I'll skip Parfit's distinction between direct and indirect.)

Maybe being collectively self-defeating is fine—Parfit does not say it's grounds for rejecting $S$.
What's special about this argument is that it is the first argument in the book—not the most important one—where an LDT-inspired move goes somewhere interesting.

I'll begin by paraphrasing the argument, and then we'll reconsider from a perspective informed by LDT.

## Parfit's argument: S in the prisoner's dilemma

The argument that $S$ is collectively self-defeating begins by considering two $S$ theorists in a prisoner's dilemma, with which I assume you are familiar.

$S$ recommends defection, since you cannot affect what your opponent does, and regardless of what they do, it is better to defect.

Therefore both players defect, and each player is worse off than they would have been if they had both cooperated.

$S$ is collectively self-defeating, since by following $S$'s recommendation to defect, both players have done worse by their $S$-given aim than if they had both cooperated.

Is it so clear that they both defect?
Let's concede that they do.
I'm going to apply the basic principle of LDT not by disputing this argument about $S$, but by proposing a new theory, a modification of $S$.

## The self-referential self-interest theory S²

The new theory, $S^2$, gives you the same aim as $S$, but a different policy.
It recommends taking the action that it would be best for you for $S^2$ to recommend.

I call this the self-referential self-interest theory.
We could abbreviate that to $SS$.
Thus the cutesy name $S^2$, even though the $S$'s don't stand for the same thing.

Let's consider a prisoner's dilemma between $S^2$ theorists, and assume that they have common knowledge that they are both $S^2$ theorists.
What does $S^2$ recommend?

## S² recommends cooperation if we assume the right counterpossibles

Assume that for each action, if $S^2$ recommends that action, then both players will take it.
Or, if it _had_ recommended it, then both players _would_ have taken it.
These are the counterpossible implications we need for this problem.

If we have these counterpossibles, it's straightforward to derive $S^2$'s recommendation.
If $S^2$ recommends that you defect, then both players defect.
Whereas if $S^2$ recommends that you cooperate, then both players cooperate.
This is better for you than if both players defect, so $S^2$ recommends that you cooperate.

Therefore the outcome is mutual cooperation, and Parfit's argument that $S$ is collectively self-defeating doesn't go through for $S^2$.

## Where can we get S²'s counterpossibles?

But why assume that whatever $S^2$ recommends, both players will do (and that if it had recommended otherwise, then both players would have done that instead)?
Because the prisoner's dilemma is symmetrical: it looks the same from the perspective of each player.
So both players should get the same recommendation from $S^2$.
And since they're both $S^2$ theorists, they both follow that recommendation.

We want that reasoning to go through, but it seems hard for any formal theory to work like that.
Let's see how the theoretical difficulty with counterpossibles manifests in this problem.

## The problematic counterpossible for S² in the prisoner's dilemma

The problematic counterpossible implication in this scenario is the statement: "if $S^2$ had recommended defection, then both players would have defected."

We can't do without this statement.
It's why $S^2$ recommends cooperation.

But it's problematic because if cooperation logically follows from our assumptions about the prisoner's dilemma and $S^2$, then we cannot consistently reason from the premise that $S^2$ recommends defection.

To see the inconsistency clearly: first, assume that you have some valid argument $A$ that $S^2$ recommends cooperation.
Now, imagine another argument $B$ which begins with the premise that $S^2$ recommends defection.
Insert after that premise all the steps of argument $A$, ending with the statement that $S^2$ recommends cooperation.
With that in conjunction with the premise, $B$ concludes that $S^2$ recommends defection and that it recommends cooperation.
$B$, then, is a valid argument from its premise to a contradiction.

If we cannot consistently reason from the premise that $S^2$ recommends defection, how can we assert what would happen in that case?
Or, considering the principle of explosion, how can we avoid asserting everything: that if $S^2$ recommends defection then both players defect, and they cooperate, and get invitation letters from Hogwarts?

That's why counterpossibles present more serious issues than ordinary counterfactuals.
There is not just a fact but a logical argument contradicting the premise.

## Conclusion

One might wonder, can you just ignore Newcomb's problem and the whole body of decision theory literature that it spawned?
I think the answer is no.
The kind of situations that logical decision theory is supposed to address come up naturally in the course of philosophical arguments.

When reading _Reasons and Persons_, the argument above was the first place in the book where, being familiar with LDT, I saw an important unexplored path that seemed to undermine the conclusion.
There are more cases like that in the book, although I haven't read far enough into it to judge what that ultimately means for Parfit's main theses.

But I hope I've also communicated to you why logical decision theory is at best a work in progress, and why some would consider it just nonsense.
Theories in the LDT family include [timeless decision theory](https://intelligence.org/files/TDT.pdf) and [functional decision theory](https://arxiv.org/abs/1710.05060), and as I understand it, both of these put in the counterpossibles by hand the same way I did in this post.
I won't really be satisfied with arguments like the one in this post until I can follow the logic step by step in a consistent formal theory, all the way from the assumptions about the game to the conclusion about the theory's recommendation.
