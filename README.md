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
| $...x$ | intrinsic | extrinsic | how is this discussion _oriented_? |

One thing to note here is that the discussion category with $0$ is deliberated upon first, and the 
bit is "flipped" once the discourse naturally runs its course. This should also illustrate how a 
new feature or product will pass through the categories (ie, from $0000$ to $1111$)

#### $x...$ (The Phase)

| Mapping | $x=0$ | $x=1$ | Theme |
| :---: | --- | --- | --- |
| $x000$ | thought-bubble | incentive-design | |
| $x001$ | thought-bubble | experiment-design | |
| $x010$ | onboarding | user-experience | |
| $x011$ | context-switch | interface-design | |
| $x100$ | its-ethical-ethical | protocol-infra | |
| $x101$ | outsiders-forum | protocol-security | |
| $x110$ | marketing-stunts | doing-business | |
| $x111$ | thanks-obama | release-announcement | |

#### $.x..$ (The Tether)

| Mapping | $x=0$ | $x=1$ | Theme |
| :---: | --- | --- | --- |
| $0x00$ | thought-bubble | its-ethical-ethical | |
| $0x01$ | thought-bubble | outsiders-forum | |
| $0x10$ | onboarding | marketing-stunts | |
| $0x11$ | context-switch | thanks-obama | |
| $1x00$ | incentive-design | protocol-infra | |
| $1x01$ | experiment-design | protocol-security | |
| $1x10$ | user-experience | doing-business | |
| $1x11$ | interface-design | release-announcement | |

#### $..x.$ (The Layer)

| Mapping | $x=0$ | $x=1$ | Theme |
| :---: | --- | --- | --- |
| $00x0$ | thought-bubble | onboarding | |
| $00x1$ | thought-bubble | context-switch | |
| $01x0$ | its-ethical-ethical | marketing-stunts | |
| $01x1$ | outsiders-forum | thanks-obama | |
| $10x0$ | incentive-design | user-experience | |
| $10x1$ | experiment-design | interface-design | |
| $11x0$ | protocol-infra | doing-business | |
| $11x1$ | protocol-security | release-announcement | |

#### $...x$ (The State)

| Mapping | $x=0$ | $x=1$ | Theme |
| :---: | --- | --- | --- |
| $000x$ | thought-bubble | thought-bubble | |
| $001x$ | onboarding | context-switch | |
| $010x$ | its-ethical-ethical | outsiders-forum | |
| $011x$ | marketing-stunts | thanks-obama | |
| $100x$ | incentive-design | experiment-design | |
| $101x$ | user-experience | interface-design | |
| $110x$ | protocol-infra | protocol-security | |
| $111x$ | doing-business | release-announcement | |
