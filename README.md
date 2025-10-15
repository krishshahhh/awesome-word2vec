# Awesome [Word2vec](https://en.wikipedia.org/wiki/Word2vec) [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

<p align="center">
    <a href="https://github.com/cybersecurity-dev/"><img height="25" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/github.svg" alt="GitHub"></a>
    &nbsp;
    <a href="https://www.youtube.com/@CyberThreatDefence"><img height="25" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/youtube.svg" alt="YouTube"></a>
    &nbsp;
    <a href="https://cyberthreatdefence.com/my_awesome_lists"><img height="20" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/blog.svg" alt="My Awesome Lists"></a>
    <img src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/bar.gif">
</p>

---
---

## 📖 Contents
- [CBOW](#continuous-bag-of-words-cbow)
- [Skip-gram](#skip-gram)
- [My Other Awesome Lists](#my-other-awesome-lists)
- [Contributing](#contributing)
- [Contributors](#contributors)


## Continuous [bag-of-words](https://en.wikipedia.org/wiki/Bag-of-words_model) (CBOW)

```mermaid
flowchart LR
 subgraph Input["INPUT"]
        A1["w(t-2)"]
        A2["w(t-1)"]
        A3["w(t+1)"]
        A4["w(t+2)"]
  end
 subgraph Projection["PROJECTION"]
        SUM["SUM"]
  end
 subgraph Output["OUTPUT"]
        OUT["w(t)"]
  end
    A1 --> SUM
    A2 --> SUM
    A3 --> SUM
    A4 --> SUM
    SUM --> OUT

    style Input color:#000000,fill:#FFF9C4
    style Projection color:#000000,fill:#BBDEFB
    style Output color:#000000,fill:#FFCDD2
```

---
---

## Skip-gram

```mermaid
flowchart LR
 subgraph INPUT["INPUT"]
        x_wt["w(t)"]
  end
 subgraph PROJECTION["PROJECTION"]
        x_proj["Projection"]
  end
 subgraph OUTPUT["OUTPUT"]
        x_wtm2["w(t-2)"]
        x_wtm1["w(t-1)"]
        x_wtp1["w(t+1)"]
        x_wtp2["w(t+2)"]
  end
    x_wt --> x_proj
    x_proj --> x_wtm2 & x_wtm1 & x_wtp1 & x_wtp2
    classDef label fill:none,stroke:none,color:#666
    style PROJECTION fill:#BBDEFB,color:#000000
    style INPUT color:#000000,fill:#FFF9C4
    style OUTPUT fill:#FFCDD2,color:#000000
```




##

### My Other Awesome Lists
You can access the my other awesome lists [here](https://cyberthreatdefence.com/my_awesome_lists)

### Contributing
[Contributions of any kind welcome, just follow the guidelines](contributing.md)!

### Contributors
[Thanks goes to these contributors](https://github.com/cybersecurity-dev/awesome-word2vec/graphs/contributors)!

[🔼 Back to top](#awesome-word2vec-)
