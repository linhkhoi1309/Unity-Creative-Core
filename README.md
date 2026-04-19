# Unity-Creative-Core

## Overview
---
## Notes

### Rendering

- is the process of taking three-dimensional (3D) data and using it to generate a two-dimensional (2D) image for a screen.

### Render Pipelines

- are different ways of getting from 3D data to 2D image.
- each have its own advantages and disadvantages

#### Choose a render pipeline

- Built-in Render Pipeline:
    - Pros:
        + works on all platforms
        + pretty reliable
        + easy to use
    - Cons: 
        + it’s not very customizable
        + isn’t the most efficient
- Universal Render Pipeline (URP)
    - Pros:
        + Ideal for mobile, web, and VR projects (highly optimized for performance)
        + more customizable than the Built-In Render Pipeline.
        + can produce pretty decent graphics.
    - Cons:
        + a bit more complex to configure
- High Definition Render Pipeline (HDRP):
    - Pros:
        + produce high-quality graphics for high-end platforms, like consoles or gaming computers
    - Cons: 
        + very complex to configure

- URP and HDRP are both Scriptable Render Pipelines (SRPs). SRPs are highly customizable and can even be written from scratch. Since writing a render pipeline is a big task, Unity provides these two SRPs as templates, which will handle most projects.

- URP Assets control many quality settings in your project – especially related to light and shadows – and can be found in the Project window just like any other asset.

### Copyright for creators

#### What is intellectual property?

- is intangible property that is generated from the human intellect
- is protected by law from unauthorized use by others.
- includes copyright, trademarks, patents, and trade secrets.
- in order for one party (an individual or company) to use intellectual property that belongs to another party, they must have permission and observe conditions that are set by the IP owner.
- a violation of these rules is known as **infringement** on the IP owner’s rights.

#### What is copyright?

- a bundle of rights, including the right to copy.

- you own the copyright to just about anything you put down on paper, in computer memory, or in a physical creation that expresses your creativity. Even programming code, including the overall design and architecture of an application, is copyrightable.

- gives you an exclusive bundle of rights concerning that work, including the right to copy, to distribute, to perform publicly, to display publicly, and to creative derivative works.

- you have the right to stop other people from copying your work without permission. That includes reusing it in their own works, publishing it on the internet, and distributing it to others, whether it is modified or used in its original form.

- your copyright applies to your expression of an idea rather than the idea itself (idea-expression distinction). This means that common conventions of a particular genre or medium can be used by lots of different creators, but specific depictions are protected by copyright.

##### How will you know if a work is copyrighted?
-  The copyright symbol (©) indicates that an owner is making their copyright known, but it is not necessary to display the symbol to claim copyright.

##### Who owns copyright?

- When you create a digital work, then you own it and its copyright, just like you would own anything else you make in the physical world. However:
    + If you create the work in collaboration with someone else, then you both share the copyright.
    + In some jurisdictions (geographic areas that are subject to their own sets of laws) including the US, if you were employed to create the work, then the employer typically owns the intellectual property, unless you make another legal arrangement.

##### How long does copyright last?

- When you create something, copyright attaches to it automatically at the time of creation — you don’t need to do anything to obtain copyright to your own works. 
- Copyright protection typically lasts for the lifetime of the author plus 50 to 70 years, depending on the laws of the country where it is created.
- Copyright does expire, and it can also be waived by the owner(s). Such works are said to be in the **public domain**, which means that the public owns the IP. These works are available for anyone to copy and adapt into other works.

##### Are there exceptions to copyright?
- **Fair use** allows free use of copyright-protected works for purposes such as news reporting, criticism, education, parody, and satire. It is a US standard that is not accepted in most other countries, and there is no clear rule for determining fair use — cases are often determined in court if the copyright holder takes objection to the use.
#### What is a license?

- A license to reuse copyright-protected work is permission to use it.
- When you license use of the work from the owner, the owner retains ownership but grants you permission to use it.
- A license agreement, including an end-user license agreement or EULA, sets forth the permissions you have to use a work, and the conditions you must meet in exchange.
- The permissions of the agreement may allow you to do any of the following:
    + Remix, edit, adapt, and build upon the original work if desired
    + Remix, edit, adapt, and build upon the original work in certain ways or under certain conditions (for example, the Unity Asset Store requires you to reuse assets in projects)
    + Copy and distribute the work unchanged
- The conditions of the license agreement are the terms you agree to in exchange for permission, which may include none, one, or more of the following:
    + Pay a running royalty (a fee to the owner) for each copy distributed
    + Pay a one-time fee
    + Give attribution (credit) to the creator, often with specific words or in a certain format that might include a hyperlink
    + Use the work for non-commercial purposes only
    + License your works under the same terms as the licensor
- If all uses are permitted and there are no conditions, then the work is in the public domain.

#### Consequences of breaking a license agreement

- If you are a student or aspiring professional, complying with license agreements demonstrates your digital citizenship to future employers, and protects you when you publish your portfolio and launch your career.

- If you are a freelancer, indie developer, company employee, company owner, or other creator who makes money by creating, then complying with license agreements protects you and your business from legal issues.

- Respecting everyone’s IP is a community effort — and your respect for others will be repaid as others respect you.

#### Reuse assets responsibly

##### Unity Asset Store

- makes it easy to reuse assets from other creators in your own projects because it handles most of the licensing concerns.
- are permitted to use most of these assets in your projects (even projects built in a different engine!), even for commercial use. 
- are not allowed to resell or redistribute these assets separately from your project.

- Unity Asset Store assets also have a license type, which indicates whether the asset must be purchased and managed per seat or per entity. Per seat means that the license and any fees apply to each person who uses the asset. An entity license applies to the entire company, and the fee is only paid once regardless of the number of individuals who use the asset.

- Larger companies may choose a multi-entity license, which will also cover your affiliates and subsidiaries.

##### Around the Internet

- It is important to understand who the licensor is in any context.

- On regular websites that are not intended to provide assets to creators, look for claims of copyright or references to license agreements either near the asset or in the footer of the site. 

-  If you don’t see a mention of copyright or licensing, do not assume that the asset is in the public domain — either contact the owner or publisher, or find a different asset.

##### Free asset sources

- **Pexels** provides free 2D images and videos. All assets on this site have the same license agreement: they are free to use, and payment and attribution are optional.
- **The Creative Commons search engine** lets you filter searches according to Creative Common licenses and sources. This site indexes image, audio, and video files.
- **Open Game Art** provides 2D and 3D art, textures, music, and sound effects. All assets are free; however, there are multiple different license types, so be sure to check whether you need to credit the creator per asset.

#### Give credit for the work of others

- Credit is typically noted in an attribution, which is a short blurb of text listing the title, creator’s name, source, and other information about the work.

- In some cases the exact text of the attribution is provided for you to copy into your work.

- A helpful resource for composing an appropriate attribution is on the Creative Commons wiki page (Best practices for attribution)

- In a real-time 3D project, attributions are typically listed in a page linked from the main menu of an application or game, or in the closing credits of a film or digital story.

##### Keep an assets list

- a simple log somewhere on your computer with the following information:
    + Name of the asset
    + URL where the asset is hosted
    + The creator of the asset
    + The license of the asset
    + Attribution you will add to your project (if any)

##### Help others in reviews and social media

- you can leave a review for assets you use. Although posting about another creator’s work is not a substitute for an attribution, leaving a review is an excellent way to help your fellow creators.

- giving a shout out on social media helps the artist gain a following.

#### Protect your own IP

- Is your work intended for others to reuse in their own works, or only to use as-is? If you do not want others to change your work, then you’ll want to specify that no derivative works are allowed.
- Are you building your own reputation or brand, and is getting credit for the work important to you? If so, you will want to require attribution and perhaps even require a link back to your website or online store.
- Is it important to you that no one makes money from your work? If so, you can stipulate that it must be used for non-commercial purposes only.

### Creative Commons Licenses 

#### Overview
- Creative Commons (CC) licenses are standardized tools that let creators share their work with specific permissions and restrictions.

- Provided by Creative Commons

- All CC licenses (except CC0) require:
    + BY (Attribution) → Credit must be given to the creator

#### CC0 (Public Domain Dedication)

##### Permissions
- Commercial use allowed
- Modification allowed
- Distribution allowed

##### Requirements
- No attribution required

##### Key Idea
- Creator waives all rights
- Work is effectively in the public domain

#### CC BY (Attribution)

##### Permissions
- Commercial use allowed
- Modify, remix, adapt allowed
- Distribution allowed

##### Requirements
- Must give credit

##### Key Idea
- Free use with attribution only

#### CC BY-SA (Attribution + ShareAlike)

##### Permissions
- Commercial use allowed
- Modify and remix allowed

##### Requirements
- Must give credit
- Must license derivatives under the same or compatible license

##### Key Idea
- Derivatives must remain open under the same terms

#### CC BY-ND (Attribution + NoDerivatives)

##### Permissions
- Commercial use allowed
- Redistribution allowed

##### Restrictions
- No modifications allowed

##### Requirements
- Must give credit

##### Key Idea
- Only original, unchanged work can be shared

#### CC BY-NC (Attribution + NonCommercial)

##### Permissions
- Modify and remix allowed
- Distribution allowed

##### Restrictions
- No commercial use

##### Requirements
- Must give credit

##### Key Idea
- Free for non-commercial use only

#### CC BY-NC-SA (Attribution + NonCommercial + ShareAlike)

##### Permissions
- Modify and remix allowed
- Distribution allowed

##### Restrictions
- No commercial use

##### Requirements
- Must give credit
- Must license derivatives under the same terms

##### Key Idea
- Non-commercial use with required open sharing

#### CC BY-NC-ND (Attribution + NonCommercial + NoDerivatives)

##### Permissions
- Redistribution allowed (unchanged only)

##### Restrictions
- No commercial use
- No modification allowed

##### Requirements
- Must give credit

##### Key Idea
- Most restrictive CC license

#### License Elements Explained

- BY (Attribution)  
  Credit must be given  

- SA (ShareAlike)  
  Derivatives must use the same license  

- ND (NoDerivatives)  
  No changes allowed  

- NC (NonCommercial)  
  No commercial use  

#### Comparison Table

| License         | Commercial | Modify | ShareAlike | Attribution |
|----------------|-----------|--------|------------|------------|
| CC0            | Yes       | Yes    | No         | No         |
| CC BY          | Yes       | Yes    | No         | Yes        |
| CC BY-SA       | Yes       | Yes    | Yes        | Yes        |
| CC BY-ND       | Yes       | No     | No         | Yes        |
| CC BY-NC       | No        | Yes    | No         | Yes        |
| CC BY-NC-SA    | No        | Yes    | Yes        | Yes        |
| CC BY-NC-ND    | No        | No     | No         | Yes        |

---
## References