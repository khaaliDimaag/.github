# khaaliDimaag special github repo

There are two main functions of this repo,
1. Implement all github specific goodness
   - [ ] Org README
   - [ ] Issue Templates
   - [ ] PR Templates
   - [ ] Other [special files](https://github.com/joelparkerhenderson/github-special-files-and-paths)
2. Utilize the discussions tab effectively (see [categories](#discussion-categories))

## Using Discussions

The goal here is to manage khaaliDimaag using github discussions (and github in general) while also
having enabling public transparency and input. As such, the discussion categories are designed to 
help move a _thought-bubble_, all the way to a _release-announcement_, going through all manner of 
discussions from implementation details to ethical concerns to business impact.

### Core Idea

Every new feature or product passes through a set of discussion categories and as the discourse 
progresses through the categories, the roadmap of that feature or product is informed. The 
discussion categories are mapped to 4 bits, where each bit place value holds a special meaning,
informed by whether it is a $0$ or $1$.

- $0$ broadly represents the _heart_ or the _feel_ or the _abstract_; simultaneously being nothing 
and everything.
- $1$ broadly represents the _brain_ or the _facts_ or the _reality_; ie, it is well defined and a 
"grounded" unit.

### Discussion Categories

| Mapping | Category Name | Description | When to use? |
| :-----: | :------------ | ----------- | ------------ |
| $0000$ | thought-bubble | an idea; the concepts of a plan | half baked features begin here |
| $0001$ | napkin-math | a more structured and reasoned out idea | feature ideas may also begin here but have a higher bar of acceptance |
| $0010$ | onboarding | strategies to reduce friction for users to leverage kdio | when discussing how new users discover, access, and start using a feature |
| $0011$ | context-switch | how kdio fits inside a different domain | does the new feature enable kdio to operate in a different domain? |
| $0100$ | its-ethical-ethical | with great power, comes great responsibility | to consider the ethical implications of this new idea |
| $0101$ | outsiders-forum | speak less, read more! | could be used as a customer support channel |
| $0110$ | marketing-stunts | how we occupy mindshare | when discussing positioning, narrative, and public-facing communication strategies |
| $0111$ | thanks-obama | all _democratic_ polls conducted here | when the discussion reaches a stage requiring some form of voting, either internally, or publically |
| $1000$ | incentive-design | all things regarding mechanism design, tokenomics, and game theory | to discuss what this new idea will enable / disable |
| $1001$ | validation-framework | validating the idea and assumptions | use this to talk about how we validate our assumptions and track success |
| $1010$ | user-experience | mapping user flows and journeys | to talk about e2e user experiences |
| $1011$ | interface-design | all things related to the clients interacting with the protocol | how do we make sure that anyone may build a client? |
| $1100$ | protocol-infra | any updates to the core protocol needed | to talk about how or if this idea adds any value to core infra or protocol |
| $1101$ | protocol-security | consideration of all things security, including user error! | when evaluating attack vectors, failure modes, edge cases, and defensive measures |
| $1110$ | doing-business | how do we ensure the protocol makes money, or is anti-fragile? | to discuss revenue streams from this idea |
| $1111$ | release-announcement | fuck it, ship it! | the last step of discussions, talking about how we announce this new feature post implementation |

> [!IMPORTANT]
> Note that implementation of the idea/feature may happen while the discussions are taking place as
> it moves through the different discussion categories

### Place Value and Tracks

| Place Value | $x=0$ | $x=1$ | track | _vibe_ |
| :---------: | ----- | ----- | ----- | ------ |
| $x...$ | exploration | execution | phase | what _phase_ is the discussion in? |
| $.x..$ | self | world | tether | where is this discussion _tethered_? |
| $..x.$ | foundational | manifestation | layer | which _layer_ is this discussion on? |
| $...x$ | intrinsic | extrinsic | orientation | how is this discussion _oriented_? |

One thing to note here is that the discussion category with $0$ is deliberated upon first, and the 
bit is "flipped" once the discourse naturally runs its course. This should also illustrate how a 
new feature or product will pass through the categories (ie, from $0000$ to $1111$)

Also the bit-flipping mechanism coupled with the place-value semantic naming also enables us to 
jump around these discussion categories by choosing a _track_. The 4 place values give us 4 tracks 
to choose from:
- [`the-phase`](#x-the-phase) Interleaves thinking and doing (_Good for features where you want to_ 
_validate ideas incrementally rather than planning everything upfront_)
- [`the-tether`](#x-the-tether) Alternates between self-focused and world-focused concerns (_Good_ 
_for features that need strong internal conviction before external engagement_)
- [`the-layer`](#x-the-layer) Goes from foundational to manifestation at each level (_Good for_ 
_features where you want to build up from first principles before making anything visible_)
- [`the-orientation`](#x-the-orientation) The natural counting order — intrinsic first, then 
extrinsic (_Good as a general-purpose default because it ensures you fully understand the thing_ 
_itself before considering it in relation to others_)

#### $x...$ (The Phase)

| Mapping | $x=0$ | $x=1$ | Theme |
| :-----: | ----- | ----- | ----- |
| $x000$ | thought-bubble | incentive-design | from "what if?" to "why would anyone?" |
| $x001$ | napkin-math | validation-framework | from structured thought to structured testing |
| $x010$ | onboarding | user-experience | from entry point to entire path |
| $x011$ | context-switch | interface-design | from domain fit to system boundary |
| $x100$ | its-ethical-ethical | protocol-infra | from "should we?" to "how do we build it right?" |
| $x101$ | outsiders-forum | protocol-security | from listening to defending |
| $x110$ | marketing-stunts | doing-business | from capturing attention to capturing value |
| $x111$ | thanks-obama | release-announcement | from consensus to launch |

#### $.x..$ (The Tether)

| Mapping | $x=0$ | $x=1$ | Theme |
| :-----: | ----- | ----- | ----- |
| $0x00$ | thought-bubble | its-ethical-ethical | the idea meets its moral weight |
| $0x01$ | napkin-math | outsiders-forum | what we think vs what they think |
| $0x10$ | onboarding | marketing-stunts | _pulling users in vs reaching out_ |
| $0x11$ | context-switch | thanks-obama | _domain mapping vs reality check_ |
| $1x00$ | incentive-design | protocol-infra | rules of the game vs the field it's played on |
| $1x01$ | validation-framework | protocol-security | probing our assumptions vs defending against others' probes |
| $1x10$ | user-experience | doing-business | value delivered and value captured |
| $1x11$ | interface-design | release-announcement | designing the touchpoint vs announcing the arrival |

#### $..x.$ (The Layer)

| Mapping | $x=0$ | $x=1$ | Theme |
| :-----: | ----- | ----- | ----- |
| $00x0$ | thought-bubble | onboarding | what it is vs how they find it |
| $00x1$ | napkin-math | context-switch | what we reason and where it fits |
| $01x0$ | its-ethical-ethical | marketing-stunts | what we stand for vs how we say it |
| $01x1$ | outsiders-forum | thanks-obama | hearing voices and counting votes |
| $10x0$ | incentive-design | user-experience | the rules underneath vs the experience on top  |
| $10x1$ | validation-framework | interface-design | hypothesis and implementation |
| $11x0$ | protocol-infra | doing-business | what holds it up vs what keeps it alive |
| $11x1$ | protocol-security | release-announcement |  securing the system and spotlighting it |

#### $...x$ (The Orientation)

| Mapping | $x=0$ | $x=1$ | Theme |
| :-----: | ----- | ----- | ----- |
| $000x$ | thought-bubble | napkin-math | raw intuition meets structured reasoning |
| $001x$ | onboarding | context-switch | _native context vs foreign context_ |
| $010x$ | its-ethical-ethical | outsiders-forum | our ethics vs their feedback |
| $011x$ | marketing-stunts | thanks-obama | we speak, they vote |
| $100x$ | incentive-design | validation-framework | build the model vs validate the model |
| $101x$ | user-experience | interface-design | what we want them to feel and how we make them feel that |
| $110x$ | protocol-infra | protocol-security | the core vs defending the core |
| $111x$ | doing-business | release-announcement | making it work vs making it known |
