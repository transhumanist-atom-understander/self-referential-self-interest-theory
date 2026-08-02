A _logical decision theory_ [recommends that you choose as if deciding the output of your decision algorithm](https://www.lesswrong.com/w/logical-decision-theories?lens=introduction-to-logical-decision-theory-for-analytic#Logical_decision_theory).

The main difficulty in formulating a logical decision theory is how to define statements like: "If my algorithm outputs this, the result will be that".
These look like counterfactual implications, but counterfactuals describe possible worlds with different contingent facts, whereas here we are considering if a logical fact were different.
Much theoretical work has gone into elaborating this kind of _counterpossible_ implication, without, in my opinion, satisfactory results.

But what's the point of this theoretical work?
Do we really need LDT?

What's the difference between choosing the output of your decision algorithm and just making a choice?
There is no difference, as long as your choice is the only thing in the world that depends on your decision algorithm.
Substantial applications of LDT are games where the player's environment contains some other implementation of the algorithm.
The central example is Newcomb's problem.

But Newcomb's problem sounds like a science fiction story, and I'm not convinced by [the case that analogous problems are part of our normal social lives](https://www.lesswrong.com/posts/puutBJLWbg2sXpFbu/newcomblike-problems-are-the-norm).

That's the context for the observation I want to share: that I was reading Derek Parfit's _Reasons and Persons_, and LDT seemed like an important missing piece in one of his arguments.
It's not an application of LDT in real life, but it's an application to philosophical argumentation.

Derek Parfit's book describes a variety of theories of morality and rationality, and defines certain properties of these theories.
One property, the property of being "collectively self-defeating", is defined in terms of games where multiple players are deciding according to the same theory.
Because each player faces an "environment" (the other player) which depends on the same theory they are using to decide, a philosophical move inspired by LDT yields interesting results.

## The claim: S is collectively self-defeating

The argument I'm going to repeat concerns the self-interest theory ($S$), which Parfit says is a theory of rationality.
(Since this is LessWrong, I must add that he doesn't mean [what Yudkowsky means by "rationality"](https://www.lesswrong.com/posts/HcCpvYLoSFP4iAqSz/rationality-appreciating-cognitive-algorithms), but I don't think that's important for this argument.)

What we need to know about $S$ is that it prescribes an aim, which is that your life go as well as possible, as well as what I'll call a policy: it recommends taking the actions that make your life go as well as possible, among the available alternatives.

Parfit argues that $S$ has the property of being _collectively self-defeating_: that is, if we all follow $S$, then we will do worse by our $S$-given aim than if we had all taken other actions.

We shouldn't exaggerate the significance of this conclusion in the book: Parfit does not say that you should reject theories for being collectively self-defeating.
What's special about this argument is that it is the first argument in the book—not the most important one—where an LDT-inspired move went somewhere interesting.

## The argument: S in the prisoner's dilemma

The argument that $S$ is collectively self-defeating begins by considering two $S$ theorists in a prisoner's dilemma, with which I assume you are familiar.

$S$ recommends defection, since you cannot affect what your opponent does, and regardless of what they do, it is better to defect.

Therefore both players defect, and each player is worse off than they would have been if they had both cooperated.

$S$ is collectively self-defeating, since by following $S$'s recommendation to defect, both players have done worse by their $S$-given aim than if they had both cooperated.

Is it so clear that they both defect?
Let's concede that they do.
I'm going to try to apply the basic principle of LDT not by disputing this argument about $S$, but by proposing a new theory, a modification of $S$.

## The self-referential self-interest theory S²

The new theory, $S^2$, gives you the same aim as $S$, but a different policy.
It recommends taking the action that it would be best for you for $S^2$ to recommend.

I call this the self-referential self-interest theory.
We could abbreviate that to $SS$.
Thus the cutesy name $S^2$, even though the $S$'s don't stand for the same thing.

Let's consider a prisoner's dilemma between $S^2$ theorists, and assume that they have common knowledge that they are both $S^2$ theorists.
What does $S^2$ recommend?

Let's suppose, now, that if $S^2$ recommends an action, then both players will take that action.
I would like to say that this follows from the definition of $S^2$ and the symmetry of the prisoner's dilemma: that is, that the game looks the same from the perspective of each player.
It is at this point that I have to admit that because I have no logically consistent formal theory, I cannot logically show that this follows.
I can only say that this is how we want $S^2$ to behave, and leave it to the future to fully specify a theory with this behavior.

Assuming, then, that whatever $S^2$ recommends both players will do, it is better for you for $S^2$ to recommend cooperation, because if both players cooperate, that's better for you than if they both defect.
Therefore $S^2$ recommends that you cooperate.

The same reasoning applies to the other player, so if both are $S^2$ theorists, the outcome is mutual cooperation.
Parfit's argument that $S$ is collectively self-defeating does not go through for $S^2$.

## How the theoretical issues with counterpossibles show up

The problematic counterpossible implication in this scenario is: "if $S^2$ had recommended defection, then both players would have defected."

We can't avoid this statement.
That $S^2$ recommending defection would lead to mutual defection is why it recommends cooperation.

But it's problematic because, if $S^2$'s recommendation is a logical consequence of its definition, then it is contradictory to assume a different recommendation.

To see the contradiction clearly, first, let's assume that we have some valid argument $A$ that $S^2$ recommends cooperation.
Now, imagine another argument $B$ beginning with the premise of our problematic counterpossible: that $S^2$ recommends defection.
Insert after that premise all the steps of argument $A$, ending with the statement that $S^2$ recommends cooperation.
Now, together with our premise, we have that $S^2$ recommends defection and that it recommends cooperation.
$B$, then, is a valid argument from the premise to a contradiction.

How, then, can we have any implication with the premise "If $S^2$ had recommended defection..."?
A counterpossible like this presents more serious issues than an ordinary counterfactual, since there is not just a fact but a logical argument contradicting the premise.

## Conclusion

I am hopeful that it is possible to formulate $S^2$ to the level of formality that we can consistently derive, from a description of the situation, that whatever $S^2$ recommends, both players would do.
This is a hope I share with others who have worked on formal versions of the basic idea of LDT.

I haven't really gotten far enough in the book to say the ultimate consequences of this LDT-inspired move for Parfit's central points.
But in any case, this was an application of LDT not to Newcomb's problem or the body of decision theory literature provoked by it, but to an argument from philosophy of independent interest.
