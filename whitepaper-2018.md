# Meta

## Ownership and License

This is a work product of the [CompK](http://compk.stanford.edu/) working group of Stanford's [CodeX Center for Legal Informatics](http://codex.stanford.edu/).

This paper may be destined for academic publication. Contributors will be credited accordingly.

### To contribute text to this document,

- if you are a member of the organization: commit changes directly to master
- if you are diffident: make a personal branch and commit changes there; then pull request
- if you are not a member: fork and pull request.

This repository may go private in the future.

## Format

This is formatted in Markdown, which is described [here](https://daringfireball.net/projects/markdown/syntax).

## Context

A small group of interested individuals and organizations met at Stanford in September 2017 to plan a way forward around realizing the vision of computable contracts (and law).

## See Also

- [Meng's book chapter](https://github.com/legalese/legalese-compiler/blob/master/doc/chapter-201707.org "Computable Contracts: from Academia to Industry")
- [Accord Project](https://github.com/accordproject/)'s [working groups](https://github.com/accordproject/working-groups)

# Our First Whitepaper

A White Paper Outline on the CodeX CompK Legal Specification Protocol

from CodeX CompK call 2017-12-06: Goodenough, Grosof, Salkind, Surden, Waltl, Wong

deadline: be nice to have some draft presentable by April for FutureLaw

## Ten Challenges

Contracts need to serve this requirement and that requirement and the other thing. Being Satoshi-level geniuses we hereby enumerate the problems and show how they are trivially solved as a side-effect of our breakthrough contribution. And we’ll do it in 8 pages, one shorter than Bitcoin.

### a life-cycle approach:

motivation for contracts: ever since the invention of writing people have wanted to have things in black and white because memories are fallible and social systems want to get conflicts resolved with a minimum of spilled blood
- derivation from a library, vs de novo drafting
- negotiation
- execution
- runtime
- revision / novation
- termination / expiration / renewal
- integration with enterprise systems

### Explainability

- What needs to be explained: The rules vs. the features (reason for a clause)
- The execution: paths (eg. abstract syntax tree)
- Openness
- What are criteria for open-texturedness: Conditions vs. phrases & terms
- Clauses that allowed to contain vague terms (eg hybrid contracts)
- Defeasibility (non-monotonic logics). As distinct from ambiguity. “conflict handling” is the KRR term. deliberate vs unintentional ambiguity. In a rule-based system, precedence resolves conflicts. In a case-based system, precedents resolve conflicts, ha ha.
- interoperability and transmissibility
- Negotiation (are the rules negotiated or the features of the contract?)
- rule ambiguity/conflicts of resolution: questions of law. how do we apply given rules to answer a question? appeal courts consider questions of law and not questions of fact.
- feature extraction: questions of fact. does a state of the world exist or not; do the parties agree on this state? what was the history? what actually happened?
- the legal fiction of a meeting of minds and common intent: sophisticated parties are always preparing for litigation and laying traps for the other

### “Captured Legal Assertion”

having a human in the loop

the party which asserts that “best efforts” have been made. is this a judge? or an arbitrator? or an expert witness? what are the marginal costs of making these assessments on an ongoing basis? often the costs are high enough to only make those assessments in the context of dispute resolution.

there are a class of computer APIs which call out to a human: CAPTCHA, data-gathering questionnaire, Mechanical Turk. what user is authorized to make the determination? This is Nobel-Prize-level work: “allocation of decision rights in incomplete contracts.”

what is the marginal value of making an ongoing assessment if every assessment is preliminary and defeasible? it can always be reversed in the light of later events that such-and-such incident is part of a larger pattern of behavior what demonstrates that one party was not acting in good faith.

## What we’ve learned from centuries of legal history

- How Contracts Are Used In The Real World
- Generic Archetypes for Contracts
 - this aligns with the Use Cases work product
- Recent Research
- Legal Ontologies


# Meeting Minutes

Notes from call 20171206

Benj:  points of agreement fm workshop breakout, including a few basic
approaches and use cases.  
what is same vs. difft fm other semantic interoperability;
what's difft includes need for logical expressiveness
to represent semantics of NL and handle argumentation w/ priorities;
pointing at use cases including smart contracts, SLAs for telecomm,
(and maybe a few other apps);
open IP of the effort, but use proprietary ecosystem components, while
making it so no one proprietary is dominating, 
independent of contract execution platform, have an understandable and
explainable contract terms; 
need logic, and rules specifically, to represent the contingent character of
contract provisions and related law, regulation, policy.
Harry:  we want to layout several sub-problems, only working on some of those
initially.
Harry:  lay out the overall steps of contracting today, where we fit;
top 10-20 types of contracts and top 10-20 terms in contracts.
what is needed, what electronic contracts bring.
Oliver:  that could be the test suite, in a sense.
%%%%%%%%% notes taken by Benjamin

% notes from mtg on LSP planning 12/5/17 10a PST
% notes by Benj

%%%%%%%% on technical white paper:

participants:
Susan Salkind
Oliver Goodenough
Benjamin Grosof
Meng Weng Wong
Harry Surden
Bernard Waltl
Mark Flood

%%%% before the mtg:

from Mark Flood:
FYI, I met with Houman Shadab yesterday. He is helping to coordinate the Accord Project, which seems to be getting some traction. Would it make sense to involve him (or other Accord members) in the CompK discussions?  

https://www.accordproject.org/

%%%%

Susan and Oliver discussed some overall organizing vision

Benj: we need to focus, not tackle too much initially, say 1-5 pages of 
relatively high level vision.  
Bernard:  yes.
Harry:  yes, e.g., kinda like an early Bitcoin document by Satoshi.  9 pages,
rigorous yet simple manner.  10 major challenges of a crypto currency netwk,
how to address each.
Oliver:  bit less high level than what we've already done, step toward
spec'ing it out.
Benj:  points of agreement fm workshop breakout, including a few basic
approaches and use cases.  
what is same vs. difft fm other semantic interoperability;
what's difft includes need for logical expressiveness
to represent semantics of NL and handle argumentation w/ priorities;
pointing at use cases including smart contracts, SLAs for telecomm,
(and maybe a few other apps);
open IP of the effort, but use proprietary ecosystem components, while
making it so no one proprietary is dominating, 
independent of contract execution platform, have an understandable and
explainable contract terms; 
need logic, and rules specifically, to represent the contingent character of
contract provisions and related law, regulation, policy.
Harry:  we want to layout several sub-problems, only working on some of those
initially.
Harry:  lay out the overall steps of contracting today, where we fit;
top 10-20 types of contracts and top 10-20 terms in contracts.
what is needed, what electronic contracts bring.
Oliver:  that could be the test suite, in a sense.

%%%% fm the mtg chat:  more notes by others / all 

Benj:  points of agreement fm workshop breakout, including a few basic
approaches and use cases.  
what is same vs. difft fm other semantic interoperability;
what's difft includes need for logical expressiveness
to represent semantics of NL and handle argumentation w/ priorities;
pointing at use cases including smart contracts, SLAs for telecomm,
(and maybe a few other apps);
open IP of the effort, but use proprietary ecosystem components, while
making it so no one proprietary is dominating, 
independent of contract execution platform, have an understandable and
explainable contract terms; 
need logic, and rules specifically, to represent the contingent character of
contract provisions and related law, regulation, policy.
Harry:  we want to layout several sub-problems, only working on some of those
initially.
Harry:  lay out the overall steps of contracting today, where we fit;
top 10-20 types of contracts and top 10-20 terms in contracts.
what is needed, what electronic contracts bring.
Oliver:  that could be the test suite, in a sense.

Benj:  examples of precedence:  more recent, higher authority, more specific.

Oliver:  rule ambiguity vs. fact ambiguity, i.e., question of law vs. 
question of fact.  Start with fact ambiguity.  (ambiguity  here is in the legal
community terminology sense).

Benj:  I prefer to use the logical terminology of conflict, defeasibility,
prioritized argumentation.  

Oliver:  yes, that's better than talking about "ambiguity". 

Oliver:  As foci:  
1. Benj points he summarized -- he coord making a list of that.
2. Harry points he summarized -- he coord making a list of that.
3. in addition, talk about a human user interface.

Benj:  talk about requirements or desiderata for user interface, incl.
comprehensibility. but not get too specific yet.

Bernard:  yes, not get too concrete prematurely.  difft steps may need difft
UIs.

Meng has created a Google Doc.  

Susan: let's start incorporating work participants have already done, incl.
a bibliography.  

Oliver: let's keep the white paper document separate from the notes.

Harry or someone:  we can have links from the notes, etc., back and forth.

Oliver:  let's Benj and I do a phone call, maybe can come to Seattle the 
week of 1/8 or 1/15.

Benj:  we might want to use Microsoft Word for sake of its change tracking.

Meng and Oliver:  volunteered to take charge of documents.
Susan:  I  can support, tho' not be on point.

Meng:  will the white paper be an academic publication at some point?

Oliver:  yes, as working paper to start, e.g., up on Stanford website and 
cite it.

Mark:  at OFR, behind firewall, I cannot get to Google Docs!  nor
Google Drive.  let's think about
some system for version control.  can get to code repos eg subversion and 
probably github.

Meng:  we could do this as a text file on git.

Benj:  there's wiki.
Susan:  there's Sharepoint.  

Benj:  we need a convention on comments.  I propose  "[[MF: ....]]", where MF is the initials of the person making the comments.

we could also put MS Word docs into github.

Benj:  we can and should make the github private, via passwords.

we will try github.

%%%% fm chat:  notes by Meng Weng Wong and others




