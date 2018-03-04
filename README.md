# Designing iOS architecture.
## The checklist

List of questions one should ask while designing an architecture.

The article explaining the motivation is [here](https://medium.com/@borlov/e984e4ebba4a).

#### Is it scalable?
- [ ] Does it handle changing business requirements efficiently?
- [ ] Does it support gradual adoption in existing projects?
- [ ] Does it allow replacing third-party components easily?
- [ ] Does is encourage composition of small independent components?
- [ ] Does it allow adding UI to features later?
- [ ] Does it support breaking of retain cycles on integration rather than component level?
- [ ] Does it support people working simultaneously on different parts of a feature?
- [ ] Does it limit the use of event/notification systems to specific layers?
- [ ] Does it provide a strategy for cutting corners and tech debt?
    
#### Is it maintainable?
- [ ] Does it provide a tactic for fighting massive objects?
- [ ] Does it limit the number of dependencies for an object?
- [ ] Does it try to reduce the amount of boilerplate code?
- [ ] Does it minimize the number of different roles of components?
- [ ] Does it suggest project structure tolerant to changes?
- [ ] Does it feel right?
    
#### Is it prepared for navigation?
- [ ] Does it explain how to pass data between components?
- [ ] Does it allow describing and discovering app flow naturally?
- [ ] Does it avoid transient dependencies?
- [ ] Does it define how to store state?
- [ ] Does it minimize the amount of global state?
- [ ] Does it allow opening a stack of screens?
- [ ] Does it handle opening of a screen from a push notification?
    
#### Is it promoting quality?
- [ ] Does it maximize the amount of testable code?
- [ ] Does it encourages compile-time decisions over runtime decisions?
- [ ] Does it avoid force casting and unwrapping?
- [ ] Does it allow stubbing asynchronous code to run tests synchronously?
- [ ] Does it support testing of UI?
- [ ] Does it forgive mistakes?
