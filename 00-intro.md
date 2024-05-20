---
layout: two-cols-header
---
# About Me

::left::

![Picture Of Me](/me.png "Me"){width=300px}

::right::
```java {2-4|5-8|9-11|13-15}{lines:true}
Person me = new Person.Builder()
  .name("Mathias Ewald")
  .role("Solutions Architect")
  .company("GitLab")
  .contact(ContactDetails.Builder()
    .email("mewald@gitlab.com")
    .linkedin("mathias-ewald")
    .tel("+436641486171")
  ).skills(Set.of(
     "Developer Platforms", "DevSecOps",
     "SpringBoot", "Kubernetes", "AI/ML"
  ))
  .interests(Set.of("Basketball", "Running", "Smart Home")
  .pets(List.of("Dog", "Chicken"))
  .married(true).children(1)
  .build();
```

---
layout: image-left
image: /desk.jpg
---
# My Desk
- 2x Camera
- 2x Microphone
- <span v-mark="{ at: 1, color: 'yellow', type: 'circle' }">1x HDMI Switcher</span>
- 1x Audio Mixer
- 2x Keylight
- 1x Teleprompter
- 1x Monitoring Display
- 1x Video Player
- 2x Stream Deck