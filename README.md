# Guidelines I try to follow this designing/building/working on a project

plagiarized from daddy Elon musk. bias towards minimizing time to ship.

- first principles:  [https://www.youtube.com/watch?v=NV3sBlRgzTI](https://www.youtube.com/watch?v=54OSbbtXrdI)
    - imp to avoid the pitfalls of reasoning by analogy
- 5-step design process: [https://www.youtube.com/watch?v=t705r8ICkRw](https://www.youtube.com/watch?v=t705r8ICkRw) (starts from ~14th minute)
    - make the requirements less dumb: initial spec would prolly be dumb, there’s prolly a better way to do it
    - delete part or process: u wanna be adding back things at least 10% of the time; avoid ‘in case we need it’ arguments. question why we need each thing. for ex: I still find and delete patterns and pieces of code leftover from the `mtx-blockchain` repo that we didn’t need, but since I’ve been working on it for so long, my brain just assumed it to be necessary. Default to ‘not needed’. Add good comments with proper reasoning why something is needed.
    - simplify or optimize: pls don't ‘futureproof’, ‘optimize’, ‘make it robust’, ‘make it scalable’ before shipping v1. Ship first then worry about add-ons. The product is not the codebase, it is the UX. You’ll prolly spend way too long optimizing something that should not exist.
    - accelerate cycle time: finally! make the codebase nice now, make it such that adding/removing/editing new features takes as little time as possible. Bias towards shipping quickly, testing hypotheses about the user, validating through data, and making it fun.
    - automate: last step, do it manually until you hit a wall. it’s fine. Prolly doesn't take as much time as u think it does manually. don't be lazy.
    
- Magic box thinking: this is mostly for me, learn the bare minimum required to build the first iteration of something. Then focus on making it better, bias towards the speed of shipping. There is way too much to learn and finite time. For ex: learning nestjs, you ask ‘hm how does DI work, lets's research on that, u encounter 10 new terms, now u research those and suddenly it's been a week and you haven't shipped anything. Focus on the task at hand, the goal is not to make a pretty codebase, it is to solve the problem that the codebase exists for.
