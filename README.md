# FreeBSD vs Linux: An Interactive Virtual Exhibit
CSARCH2 - S01 Project Proposal
Group 2: Justin Ice David, Gian Lorenzo Ortha, Linus Carl Perdon, Neil Justine Tan, Khyle Villorente

## Complete Theme Discussion

### What is FreeBSD?
This section will discuss FreeBSD, touching on both FreeBSD as a piece of software, and touch on the ecosystem surrounding it, such as its open source nature, or the community behind the FreeBSD project. A subsection will also briefly discuss the history of FreeBSD to give the readers an idea of the background of FreeBSD.

### What Does FreeBSD Have to Offer?
This section will go over a few of the features of FreeBSD and detail how they work, that these features do, and what these features can do. This includes, but is not limited to: ZFS, which is the filesystem that FreeBSD used; jails, which work like containers to isolate running processes; and ports and packages, which are two distinct methods that FreeBSD uses to distribute applications.

### FreeBSD vs Linux
This section will mostly be an interactive venn diagram that will show the similarities and differences between FreeBSD and Linux. With their similarities, some people may think that FreeBSD is a Linux distro, when it is not. The venn diagram will have clickable nodes inside each circle and in the middle as well. The node will have text that succinctly describes the similarity or difference. For instance, a node may be called “Unix-based systems”  and be put in the middle. When the user clicks one of these nodes, a pop-up modal will appear to give more details about the specific similarity or difference the node is pertaining to. 

### Where Can We Find FreeBSD Today?
This section will discuss where FreeBSD is often used today. More than just providing a general answer, such as how FreeBSD is well-suited for server environments, we can provide a specific, real-life example when applicable. For example, in terms of server environments, we can cite Netflix as an example that uses FreeBSD for their content delivery network (FreeBSD Foundation, 2024).

| **Project Component** | **Technology** | **Version**                                    | **Application & Justification**                                                                                                                                          |
| :-------------------- | :------------- | :--------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Runtime Environment   | Node.js        | v26.0.0<br>(Required)                          | Required by the project specifications. Node.js serves as the foundation for running Astro and all tools during development and build.                                   |
| Web Framework         | Astro          | v6.0<br>(Required)                             | Required by the project specifications. Allows for fast loading of static content and hydrates the interactive components.                                               |
| Content Format        | MDX            | Managed<br>using<br>@astrojs/mdx<br>(Required) | Required by the project specifications. MDX allows the exhibit's written content to be in Markdown while embedding the React components directly inline within the page. |
| Component Framework   | React          | v19.2<br>Managed<br>using<br>@astrojs/react    | React manages component state such as the venn diagrams and handles clicks and controlling modal visibility dynamically without requiring a full page reload.            |
| Styling               | Tailwind CSS   | v4.3                                           | Tailwind CSS provides utility-first classes that streamline the styling of the components, animations, and overall exhibit layout with minimal custom CSS.               |
| Version Control       | Github         | -                                              | Hosts the project repository forked from the provided astro.build template.                                                                                              |

Following the Tech Stack Plan, our Proposed Interactive Element is an Architectural Venn Diagram comparing FreeBSD with Linux. The planned User Experience (UX) and Technical Implementation of the interactive element is as follows:

- Rendering: The interactive venn diagram is rendered directly in the MDX page. It is built as a separate component and is imported in the .mdx file of the virtual exhibit.
- State Management: The venn diagram will feature clear labels and clickable items within the individual circles featuring the unique traits of FreeBSD and Linux while the intersection contains the shared traits of the two systems. When items in either the circles or the intersection are clicked, a modal/pop-up window including a detailed explanation on the specific trait will appear. React will be used for state management to dynamically manage the modal and the visibility of contents when a clickable item is triggered by the user or when it is closed.
- Styling: Tailwind CSS will be utilized for styling of the venn diagram, positioning, animations and other design elements that will be utilized in the development of the overall virtual exhibit.

### Tentative Style Guide Snapshot

![1](https://raw.githubusercontent.com/notgian/csarch2-freebsd/refs/heads/main/imgs/1.png)
![2](https://raw.githubusercontent.com/notgian/csarch2-freebsd/refs/heads/main/imgs/2.png)
![3](https://raw.githubusercontent.com/notgian/csarch2-freebsd/refs/heads/main/imgs/3.png)
![4](https://raw.githubusercontent.com/notgian/csarch2-freebsd/refs/heads/main/imgs/4.png)
![5](https://raw.githubusercontent.com/notgian/csarch2-freebsd/refs/heads/main/imgs/5.png)
![6](https://raw.githubusercontent.com/notgian/csarch2-freebsd/refs/heads/main/imgs/6.png)

