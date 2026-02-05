# Content
- 🔧 MCP Servers in general
- 🏢 SAP MCP Server
 - 🧢 CAP
 - 🌺 Fiori
 - 5️⃣ UI5
 - 📱MDK
- 🛕 Community MCP Server
 - 📘Documentation
  - 💬 Chat
  - 💽 Servers
 - 📡 OData
 - 🧢 CAP
 - 🈷️ BTP
 - 🧑‍💻 ABAP

# 🔧 MCP Servers in general

[https://youtu.be/FLpS7OfD5-s](https://youtu.be/FLpS7OfD5-s)

# SAP TechEd Announcements
![[Pasted image 20260205180147.png]]
At **SAP TechEd 2025**, SAP positioned the [Model Context Protocol (MCP)](https://community.sap.com/t5/technology-blog-posts-by-members/unlocking-the-power-of-model-context-protocol-mcp-for-sap-business/ba-p/14258263) as the key standard for building its "Agentic Enterprise". 

**Core MCP Announcements**

- **Open-Sourced MCP Servers:** SAP released three primary [open-source MCP servers](https://community.sap.com/t5/sap-community/public-sap-open-source-webinar-open-sourced-mcp-servers-supporting-btp/ev-p/14250304) to provide domain-specific context to AI agents:
    - **CAP MCP Server:** Provides deep [context for the Cloud Application Programming Model](https://community.sap.com/t5/technology-blog-posts-by-sap/cap-highlights-from-teched-2025-and-devtoberfest-2025-a-recap/ba-p/14268014), including documentation and file structure, to help agents generate accurate code instead of "hallucinating" syntax.
    - **SAPUI5 & SAP Fiori Servers:** Enable agents to understand [UI elements and design systems](https://github.com/SAP-samples/teched2025-CA261), allowing them to create and modify frontend applications in a consistent enterprise style.
    - **LeanIX MCP Server:** A new server specifically for [LeanIX](https://github.com/SAP-samples/teched2025-BTM260), allowing AI agents to query IT landscape data and dependencies directly through the protocol.
- **MCP Support in SAP Build & VS Code:** The SAP Build extension for VS Code now supports MCP, enabling professional developers to use third-party AI assistants (like Cursor or Windsurf) alongside SAP-specific data tools.
- **SAP Integration Suite MCP Gateway:** Introduced to standardize how AI agents [consume custom APIs](https://news.sap.com/2025/11/new-agentic-capabilities-sap-btp-supercharge-developers/) and integration flows, centralizing security and governance.
- **Joule Studio Interoperability:** Custom agents built in Joule Studio can now be extended using [external MCP tools](https://superp.nl/en/sap-teched-2025-day-3-its-a-wrap/), allowing them to interact with third-party and legacy systems seamlessly.

At **SAP TechEd 2025**, the **Model Context Protocol (MCP)** was a primary focus, featuring prominently in hands-on workshops and developer-centric sessions focused on "Agentic AI." 

**Featured MCP Sessions**

- **BTM260: Building AI Agents on Your SAP LeanIX Solutions with MCP**  
    This hands-on workshop demonstrated how to use MCP to [bridge SAP LeanIX enterprise architecture data with AI agents](https://github.com/SAP-samples/teched2025-BTM260). It showed how to expose LeanIX APIs as "MCP tools" so a Large Language Model (LLM) can dynamically query IT landscapes and system dependencies.
- **CA261: Create Great UX with AI, SAP Design System, SAP Fiori Elements, and SAPUI5**  
    This session focused on [AI-assisted full-stack development](https://github.com/SAP-samples/teched2025-CA261). Participants used **MCP servers developed by SAP and Figma** to create and modify Fiori applications using AI coding assistants like **Cline** in VS Code.
- **Developer Keynote: Turning New Technology into Real-World Success**  
    The [Developer Keynote](https://www.youtube.com/watch?v=fWlfI7q7rgk) featured a live demonstration of **MCP AI Agents** in VS Code. It highlighted how these agents, powered by **SAP AI Core**, use SAP-delivered MCP servers to access domain-specific knowledge and data while staying within the [SAP BTP trust boundary](https://www.youtube.com/watch?v=-bOcGrnUfBI).
- **Agentic Coding with MCP: Extending CAP and Fiori Applications**  
    A targeted presentation showing how [MCP servers for CAP and SAPUI5](https://community.sap.com/t5/technology-blog-posts-by-sap/agentic-coding-with-mcp-extending-cap-and-fiori-applications/ba-p/14290686) provide the necessary context to AI agents to prevent code "hallucinations" and ensure generated code follows SAP best practices. 

**Strategic Mentions**

- **Keynote Highlights:** MCP was identified as the ["new kid on the block"](https://community.sap.com/t5/technology-blog-posts-by-members/sap-teched-2025-in-berlin-a-new-high/ba-p/14263493) and appeared on multiple architectural slides as the standardized way to expose SAP S/4HANA data to third-party AI agents.
- **SAP Community Talks:** Several sessions in the community track discussed the ["Agentic Platform"](https://www.youtube.com/watch?v=HZkAwM89BOg) shift, emphasizing openness and the use of MCP to connect data across the tech stack. 

These selected SAP TechEd 2025 links focus on demonstrations of MCP AI Agents, their integration with SAP AI Core, and their impact on collaborative development:

[](https://www.youtube.com/watch?v=-bOcGrnUfBI&t=43)

Developer Demo: MCP AI Agents | VS Code, AI Core & MCP ...

Nov 13, 2025 — IDE amazing amazing but also because the SAP business application studio is also based on the same framework the open source frame...

![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAMAAAD04JH5AAAAMFBMVEVHcEz/ADP/ADP/ADP/ADP/ADP/ADP/ADP/ADP/////ACf/hJP/2eD/UG3/sb7/KU5csRZJAAAACHRSTlMA5UvIcaIxGfHMYyEAAAKLSURBVHic7ZrreoMgDIYLAmKP93+3I2Bt1dqNJJJuy9d/e+ryFpLI4TscVCqVSqVSqVSfrx4UQPYuB5+Z8p8m5W/DY+iYEAz+r8/qssyo+EblG53JD5SHC19i+hlNb10J+E2kOgFUJnL2LUbwHWfYDRIftsJ3u8Z+UvcKofetwoP8aibCvkO/klkMgm0cPxFYyd+fCZ7GoG+Wfs/qHnngJOLH6CQnADRVo9AATEPQrgEtNWaBlYofo5WdgXEO2vbguXJH7oVqAJSTIMjFjzHI5mABEMzBkoWCOfgBAD4BCBZBKoMEIBk/GhzAkY8g9aH68JcLH0GP6EPH0/l640IIiD50PA3DcDryIFhEH8oAw/kiDDAMVw4ERwAYzid6KjhEI5wAAIFakp4GAPNAIyADDMSS9If6JfEcgDgPHQMAlCSagAcgpcINDVD/Nn4FkFojDsGwASC7AiNAbo3VCAaxHNgEQJUkKwDMQ+1bkhmgviTZAaAkaxB2AKhbKvADVGYiO0Dt6/FvVQGmGTJ3wmoxtmJMI+YEQC6RudYD6H0KDwBhZcoBQFwTklfFtN3Jb98X4EpvDkDbG9KiR9rmFL0U5wG48pwUWeQJCWEvtARAnRGRd+WTAu6UjCl6hFMyzIKA9ZxQ9qjWSAN0n3BaLn5fIHpjYqXvjKz0rdlH3BuK35yK3x3L357L+QfubiJpB4XYEDwcXdIuGqFKfPaTSUzC3FLX3kq0dLO1bshm7axsmol+FR6mwTcaBbNt6nR7m0rBUuq2wpdcsNnLy2urLababPF976p9YGRjcfEuv7AWb8cxo4F3YSrOtmK0y3n0VhdzdQIrn7XC3VINrursq+4PhKAqlUqlUqlU/0ZfsrVWKcUeiTwAAAAASUVORK5CYII=)

YouTube·SAP

![](data:image/jpeg;base64,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)

5:40

[](https://www.epiuselabs.com/sap-landscape-optimization-blog/sap-teched-berlin-2025-my-experience-and-highlights#:~:text=I'd%20have%20loved%20to,network%20and%20join%20some%20sessions.)

SAP TechEd Berlin 2025: My experience, and the highlights

Nov 21, 2025 — I'd have loved to see some sustainability or environmentally conscious messages in the opening, but that's not what we were there ...

![](data:image/png;base64,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)

EPI-USE Labs

![](data:image/jpeg;base64,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)

[](https://community.sap.com/t5/technology-blog-posts-by-members/sap-teched-2025-in-berlin-a-new-high/ba-p/14263493#:~:text=We%20had%20some%20fascinating%20discussions,thriving%20whenever%20we%20come%20together.)

SAP TechED 2025 in Berlin - a new high!

Nov 8, 2025 — We had some fascinating discussions with SAP and Microsoft during SAP TechEd about our Artificial Intelligence journey. Specifical...

![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAADoklEQVRYhe2XTWxUVRTHf+fNo0CnlGFaDW0pRRs7tGgtNqFG/MhLTCGU+C26MZJgN0aj0YVp3LjQjRtMal1g0p3RhIUEqkETEZG0EQReR5K2ArZ1TD+SOp2CTadvZt51MTN33kyH2h0L5yTz5px7zj3//znvzrkZUUpxJ8W4o+glAiUCJQKA2XRqRg8CpUAkX1dKIZnF3MwQIH9+iEjGLxk7nSMdJ/o7b10M20wsOXjDComs5vOSK4zzSjbOu9cA2/UZlqnijg7sqtqgQb6JxvOqzdUuHgtUjprn6e1QrvpsHp+I7RqGNX5oe8z0xRP07KrihbYgAb+pE/cBZ8ducuSnv6hZ52PgUKP2H/1xmr7rMfYFN9D3/D0rKh6dXqJ3aJbTc0tpcE+XDMR2DbHGj4RiAMarteW8tvfuPPCsuIkUvniCzur1ef7991Xiizu4TrJIw2FnzUY+6qxjl0/hW05gxh3MuINvOWEbiYR1IwMOYO6tr9Abvzg3zbejc9RUlPHovQH6L8/AssP+0JY8gOZtfpoMwEPgxC+zfDca5fDDNXSEAgQq1tG1vZJRe5rM4bOVIdbYO+0xby7TdXPv88DuKtyUy/HhGQbGoyggVF7GnqbNK6p8sbmKwRvz2p6OLnEmEsMv0BEKAKCSKcRJYiA2hli/93TECvMYx4ci2tiyqYxXrDpOvt1O/zMh2ivKeKy+Uvv7Tv6h9SdagqhkStttDZW81baVNzsb9NrNf5bBSdqpZMoaKQKebmfPGdX9yQUVvhZThTI5tagmpxa1ffDD8+r00JS2P/362oo9WYkuLCvrg3NXWt4/G1BKcbuP3P/u9/odPBAsp7N1K4cPNhYlOxieo656Iw21fgAmpxa1npX5BYcffp3hy8E/7bFbcevqx08WrzwjJokkA+89zqmfI4Qnogxf/xsoTuCR1uo82wve+9UIx4Ym04YhNmBdPbpvVXAA86mmu2io9fPGSztXDTx/aVbrLY0BgoH1+QGugmQqfdpdsX7rPfCf4ADm4qJDeCRKa3MwzzERucWO+k1af/3zC3qevPzQNnq6dxcQcBFX2SJY4c+61gQOIA92n9BnYE/tZhRwcWrhtnPde1sVxNhKxJJEcocgE1f6n11bBww3N8MvRuYREUTlJnwWUMjchpKZ7Sq9JiIosJVgDR97OgbYa60ewNQ/B5F0XqVQeK5gV5FxeR+569pVtkJZdv9za267V6T0v6BEoETgf0/gX7Y21Z2Twte2AAAAAElFTkSuQmCC)

SAP Community

[](https://github.com/SAP-samples/teched2025-CA261#:~:text=CA261%20%7C%20Create%20great%20UX%20with,steps%20in%20case%20of%20issues:)

SAP-samples/teched2025-CA261: Create great UX ... - GitHub

CA261 | Create great UX with AI, SAP Design System, SAP Fiori elements, and SAPUI5. Description. This repository contains the mate...

![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAMAAABEpIrGAAAAb1BMVEX///8kKS74+PgsMTY+Q0f8/Pzw8PGRk5ZNUVXr6+xDSEzCxMUpLjLV1tYuMzc/Q0i3ubuUl5lbX2NTV1uLjpFKTlKxs7Xh4uOFh4rn5+h3en1vcnZ9gIPc3d6/wcJzd3o3PECmqKpjZ2rOz9CfoaRP5W5KAAABU0lEQVQ4jW1T7aKCIAzdEEUTSUuzLMtuvf8zXtiQVDx/lJ3DvgEIEPU9l1rL/F4LiFEMCQYkj2JDC6VxhaRJl3x2xgin7MePMuYRD7cQftrjrcL7ELk9nNt8yXXtyRm5mquzXADKA6LpzgZRlgBPZ1WO7yn/yrmqyGdGn95Zjav2hbNghZHMV3uNG3DZCigEmhRq+pmyrUAcifj4CO+49xciWqAe6p3pCJrNH1ATp5gH6KghQLrDnoB8GxaYPYFkhpONipjrl+wI61hQ8tB5EvYb4eTL5Ebhd8u/2f4EYfhvvWJpw9ZJ0LQfb5uxbMKi3pp5xVp30miexZHbRriHvUnojrKt7isXqWRBFQQNF2w3aYCPUl8/EREWzxtuE+pVI/wbkSGp0a51Nyg1F+L5/nel56xXgt+zcMgeC0FK27gdTzVoPXtI9DBuO2tRhJj94m3/A1GiDZXoM3d5AAAAAElFTkSuQmCC)

GitHub

![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAMAAACdt4HsAAAAeFBMVEX////q6+z8/Pzu7/Dl5uj5+fnb3d/09PXV19rg4ePY2tzLzdHHyc29wMTR09bg4eGytLaGiYy2ur+Ul5mPkZTCw8R/gYRjZ2tFSlBTWF26vL2pqqxLUFaipKZrb3MlLTVbX2R1eHozOkA9QkkZIywJFyIACxosNDwjO4ThAAADJklEQVRYhe1WiZLbNgwF7wMUTUqirMOSrfWm/f8/LBQnWW+sZNJMptOmfh7TAAnC5AP5hgBPPPFvQZoZwAwwTWl3fPxscL87PkXegO08byFO5CsK8xyMhoOiVkEHzAFYgCJ2E7huEtCqhr4lKQNrKKlkOOKKHfSxg3yYp5Jxgml/BxLEkV/qga+pQBlNSYc0rrSeFhrIMB7aKY3RJxRhP0GZsSvIy9jc/DbMGY+ipckNnLYVuHksTcz7DBGYhW1zwtxc40FpYwRsn04aatlhI9B8K8H3sE/bLwabP1vLlzp3OL0Qgy+RL1c7X1+ohqCW86LgmIENvZT9YHgvPwavV2/XAHMnlqljJs8wtuvYwWtZzNnPbmjHwxaXO56T6F8g4ZgvJbHlwy1BWsR5/JDWmNZpbpd5mM/shJCPVJY/QPVjzqdxTHKIFDxPXQF5jtfuFODiPibA1byWpmlMXDzmgQ70lU7R0gHV8qxeC8xsykLyTOei9JdhObxGOB3mGYZbAvFnmPqsjteYPba6P5ruksfT8STyNZb+uMb+shWDd9dOX7g5NcOlcRQGi/wnavQ/gfpGP39nbh5X76NvEei1lMKJWgpuHZlaVkqjD8CkqLEYSCaAqyTqoLW2yIRzDKXmvpLbDa3AyjrWGKooKi9rrFFzja4GnFztvDVVQGDM1lWw3CsajwEjSsZYrLcdoFJSeCadYbUHt5mgmTCcCSWkMaQIwkIUypD4mmhojcLXUikVVfwVHHLDP/HBd8cV9SsFn9odBOaEZBqYsM54aaRxopKkZ8SsQhE9r3kgSqMtbDdBpWO0wUIdQxU0xjqSbz3ECol6xtASvz5yjG5flhkx7JgAuf0YqpEQzEmqpybPKuJUSQbKGur9GYqeeOK/D/H162D/vrNAwubK44DW3oHBu/n0GoP4JkKsrrbrhSkI4PNjdlJPBDW+dSRIHNLdUwmrbZYGyyCmR7WxTNKL404DbFWRfNxltPgw6R3+1v3f5+fH4R3JIsogDVlOvw1YKUkk75YSonZOP/yf05aU0AVrMVpfvRGiNQYMd69sUsxKh596Mz7x++IvEbErXmGAGN0AAAAASUVORK5CYII=)

[](https://www.linkedin.com/posts/praveen-sharma-1015592_github-sap-samplesteched2025-btm260-building-activity-7396389243356549120-CZXh#:~:text=Praveen%20Sharma's%20Post-,Praveen%20Sharma,Faster%20integration%20without%20custom%20coding.)

Praveen Sharma's Post - LinkedIn

Nov 17, 2025 — Praveen Sharma. 1mo. Unlocking SAP with MCP Architecture, Insights from TechEd 2025 At SAP TechEd 2025, one of the standout themes...

![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAADCUlEQVR4nO2bO2zaUBSGf1dFCh1CqDOkyUBaS+mQSDgrQ+Is2RDZyJg1nRjYgaEbA1Mzhm4ZG7FFlWKpEksqxZWaoZVcCUWlSxAxi5EY3KEFEWyIr2M4+PFNGN9rn/P5Pi2ZMwwDQeYZdQDUhAKoA6Dm+bgTXL5WBJADEJtZNNNBA1ABUDHK6fvRkyYBXL62BEAGkJx6aLMhBqAA4ACAOHrSqgvk4J/kh0n+b9UPGCfAr5hysxLg9T4/CVNu4SzgtKIk8JCEZQCArN5BVluuBTVLmAVIAo/q4TYS8ejgvwI20GjrODq79pwIpi4gCTwuj1MPku+TiEdxeZyCJPCuBTcLmARUD7ddKTNP2BYgCbzlkx8lEY96qhUwCFi2fVGWstQEfhq0LUBW72xflKUsNQwCWmi09UfLNdq6p6ZCpi5wdHbtSpl5gkmArLawd1K3bAmNto69k7qnnj7gYCUoqy2sv/8c3KVwH1lteTbpYRwLmDb9xZQkLENparjXewAApdkZ/HYDZgFGOT3xPJev2S5fuviJ4sWPwbEk8MjtvEFmc2XiPRptHdWrW1S+/HqyjLloAesvX6CaFbFrcwmdiEdR2N9Abuc1cuc3qF7dOr43uQBxdRHyuxRiCxHmurGFCE6z/95zOpVAuhQW15wnP8xpVnS8ASMVkNlceXLyfYr7bx3V881maFfgIa4uMtfzjQAAONh6xVyHfBAcRev2oPzuDI6XohEkbT5ZJ+PA3AjQur2xU5ok8Khkth4VIa55tAto3R6kD/WxU5mstmztMp0MqHMhIHd+A6XZmVhGaXbw8avzBc84yAX0l7V2GB4b3IJcwKfvf2yXVZqa6/cnF0C9pSYX4ObW1gnkAliYRmshFxD4LkBNKIA6AGpCAdQBUBMKoA6AmlAAdQDUhAKoA6CGG/1miMvXfP0RkVFOc8PHgW8BoQDqAKixEuD+i7f5wZSblYDKDAKhwpSbaRYAAC5fU+C/74a+GeW0rY+mAEACUII/uoMGoGSVPDCmBQSJcBagDoCawAv4CyJz5Ou100U7AAAAAElFTkSuQmCC)

LinkedIn

![](data:image/jpeg;base64,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)

[](https://www.youtube.com/watch?v=HZkAwM89BOg&t=6)

Keynote Highlights: AI, Agents, and More in 9 Minutes | SAP ...

Nov 6, 2025 — the question of how AI will impact development and developers is not a theoretical question anymore the truth is developers aren't...

![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAMAAAD04JH5AAAAMFBMVEVHcEz/ADP/ADP/ADP/ADP/ADP/ADP/ADP/ADP/////ACf/hJP/2eD/UG3/sb7/KU5csRZJAAAACHRSTlMA5UvIcaIxGfHMYyEAAAKLSURBVHic7ZrreoMgDIYLAmKP93+3I2Bt1dqNJJJuy9d/e+ryFpLI4TscVCqVSqVSqVSfrx4UQPYuB5+Z8p8m5W/DY+iYEAz+r8/qssyo+EblG53JD5SHC19i+hlNb10J+E2kOgFUJnL2LUbwHWfYDRIftsJ3u8Z+UvcKofetwoP8aibCvkO/klkMgm0cPxFYyd+fCZ7GoG+Wfs/qHnngJOLH6CQnADRVo9AATEPQrgEtNWaBlYofo5WdgXEO2vbguXJH7oVqAJSTIMjFjzHI5mABEMzBkoWCOfgBAD4BCBZBKoMEIBk/GhzAkY8g9aH68JcLH0GP6EPH0/l640IIiD50PA3DcDryIFhEH8oAw/kiDDAMVw4ERwAYzid6KjhEI5wAAIFakp4GAPNAIyADDMSS9If6JfEcgDgPHQMAlCSagAcgpcINDVD/Nn4FkFojDsGwASC7AiNAbo3VCAaxHNgEQJUkKwDMQ+1bkhmgviTZAaAkaxB2AKhbKvADVGYiO0Dt6/FvVQGmGTJ3wmoxtmJMI+YEQC6RudYD6H0KDwBhZcoBQFwTklfFtN3Jb98X4EpvDkDbG9KiR9rmFL0U5wG48pwUWeQJCWEvtARAnRGRd+WTAu6UjCl6hFMyzIKA9ZxQ9qjWSAN0n3BaLn5fIHpjYqXvjKz0rdlH3BuK35yK3x3L357L+QfubiJpB4XYEDwcXdIuGqFKfPaTSUzC3FLX3kq0dLO1bshm7axsmol+FR6mwTcaBbNt6nR7m0rBUuq2wpdcsNnLy2urLababPF976p9YGRjcfEuv7AWb8cxo4F3YSrOtmK0y3n0VhdzdQIrn7XC3VINrursq+4PhKAqlUqlUqlU/0ZfsrVWKcUeiTwAAAAASUVORK5CYII=)

YouTube·SAP

![](data:image/jpeg;base64,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)

8:54

[GitHub](https://github.com/) contains a growing ecosystem of SAP-related [Model Context Protocol (MCP)](https://community.sap.com/t5/technology-blog-posts-by-sap/mcp-a-comprehensive-guide/ba-p/14238053) projects, ranging from official SAP frameworks to community-led utilities for automation and data access.

**Official SAP & Core Framework Projects**

- **cap-js/mcp-server:** The [official MCP server for SAP CAP](https://github.com/cap-js/mcp-server) provides AI models with project-specific context, such as identifying CDS services, entity relationships, and helping with Node.js coding.
- **SAP/mdk-mcp-server:** An [official server for the Mobile Development Kit (MDK)](https://github.com/SAP/mdk-mcp-server) that facilitates creating and managing mobile applications via AI agents using Cloud Foundry and mobile metadata.
- **SAP-samples/ui5con-2026-fiori-mcp-server:** A [hands-on repository](https://github.com/SAP-samples/ui5con-2026-fiori-mcp-server) demonstrating how to use MCP to build and modify SAP Fiori applications with AI assistants like Cline. 

**Community & Developer Tooling**

- **mario-andreschak/mcp-abap-adt:** A [bridge for ABAP Development Tools (ADT)](https://github.com/mario-andreschak/mcp-abap-adt) that allows AI agents to interact with ABAP systems to retrieve source code and table structures.
- **marianfoo/mcp-sap-docs:** A [lightweight server](https://github.com/marianfoo/mcp-sap-docs) providing unified, full-text search access to official SAP documentation (UI5, CAP, ABAP) using BM25 and SQLite.
- **mario-andreschak/mcp-sap-gui:** An [automation server](https://github.com/mario-andreschak/mcp-sap-gui) designed for programmatic control and automation of SAP GUI transactions through MCP.
- **marianfoo/mcp-sap-notes:** A specialized tool for [searching SAP Notes and KB articles](https://glama.ai/mcp/servers/@marianfoo/mcp-sap-notes) using SAP Passport authentication and browser automation. 

**Integration & Database Access**

- **CostingGeek/sap-mcp:** Enables [bidirectional communication between Claude AI and SAP systems](https://github.com/CostingGeek/sap-mcp) via the SAP Graph API for real-time sales order and customer data retrieval.
- **HANA Cloud MCP Server (HatriGt_hana-mcp-server):** Implements MCP for [machine learning operations (MLOps) with SAP HANA Cloud](https://github.com/MCP-Mirror/HatriGt_hana-mcp-server), including model registry and context management.
- **CData/sap-hana-mcp-server:** A [read-only MCP server](https://github.com/CDataSoftware/sap-hana-mcp-server-by-cdata) that allows LLMs to query live SAP HANA data using natural language via JDBC.
- **gavdilabs/cap-mcp-plugin:** A plugin that [automatically generates MCP servers from CAP OData services](https://github.com/gavdilabs/cap-mcp-plugin) using simple annotations for AI-native data access.
Beyond the core framework releases, several specialized MCP projects have emerged to connect AI agents with broader SAP data landscapes and documentation. 

**Data & System Access**

- **SAP Datasphere MCP Server:** A [newly released open-source server](https://www.linkedin.com/posts/mario-de-felipe-103a762b_github-mariodefelipesap-datasphere-mcp-activity-7405324567688273920-lrC5) that allows AI agents to explore spaces, inspect assets, and run relational queries in **SAP Datasphere** using natural language.
- **SAP Automation Pilot MCP Server:** This [official server](https://help.sap.com/docs/automation-pilot/automation-pilot/mcp-server) exposes automation commands as tools, allowing AI agents to trigger and manage cloud operational tasks directly.
- **SAP ECC & S/4HANA ABAP Add-On:** A [community-developed server](https://community.sap.com/t5/technology-blog-posts-by-members/mcp-server-for-sap-ecc-amp-s-4hana-unlimited-abap-add-on-for-display-create/ba-p/14293485) designed for the "Unlimited ABAP Add-On," enabling agents to display, create, and update tools within traditional SAP environments.
- **K2view SAP MCP:** A commercial integration that [consolidates fragmented data](https://www.k2view.com/blog/sap-mcp/) from S/4HANA, HR, and Supply Chain modules into a single governed MCP server for AI consumption. 

**Documentation & Training**

- **SAP Documentation MCP Server:** A [fast, lightweight server](https://mcpservers.org/servers/marianfoo/mcp-sap-docs) by **marianfoo** that provides unified access to official guides for **SAPUI5**, **CAP**, and **wdi5** using intelligent full-text search.
- **ASUG AI163 Sample Repository:** A [hands-on resource](https://github.com/SAP-samples/ASUG-AI163) from **SAP-samples** that demonstrates how to interconnect custom AI agents with SAP Business Networks using pre-built action projects and destinations. 

**Developer Tooling Extensions**

- **Cline (VS Code Extension):** While [SAP AI Core](https://github.com/cline/cline/issues/7785) is still being integrated as a native provider, developers are already using this extension with local MCP servers to [automate SAP development workflows](https://github.com/SAP-samples/teched2025-IN161).
- **SAP Cloud SDK for AI:** SAP's official AI SDK for JavaScript/TypeScript is increasingly used as the base for building custom MCP servers that interact with the **Generative AI Hub**. 

Would you like to see a **sample configuration** for connecting one of these servers to **Claude Desktop** or **VS Code**?


# 🏢 SAP MCP Server

[SAP Build introduces new MCP Servers to enable age... - SAP Community](https://community.sap.com/t5/technology-blog-posts-by-sap/sap-build-introduces-new-mcp-servers-to-enable-agentic-development-for/ba-p/14205602)

## 🧢 CAP

[https://community.sap.com/t5/technology-blog-posts-by-sap/boost-your-cap-development-with-ai-introducing-the-mcp-server-for-cap/ba-p/14202849](https://community.sap.com/t5/technology-blog-posts-by-sap/boost-your-cap-development-with-ai-introducing-the-mcp-server-for-cap/ba-p/14202849)

### [https://github.com/cap-js/mcp-server](https://github.com/cap-js/mcp-server)

## 🌺 Fiori

  

[https://community.sap.com/t5/technology-blog-posts-by-sap/sap-fiori-tools-update-first-release-of-the-sap-fiori-mcp-server-for/ba-p/14204694](https://community.sap.com/t5/technology-blog-posts-by-sap/sap-fiori-tools-update-first-release-of-the-sap-fiori-mcp-server-for/ba-p/14204694)

[https://github.com/SAP/open-ux-tools/tree/main/packages/fiori-mcp-server](https://github.com/SAP/open-ux-tools/tree/main/packages/fiori-mcp-server)

[https://www.npmjs.com/package/@sap-ux/fiori-mcp-server](https://www.npmjs.com/package/@sap-ux/fiori-mcp-server)

## 5️⃣ UI5

[https://community.sap.com/t5/technology-blog-posts-by-sap/give-your-ai-agent-some-tools-introducing-the-ui5-mcp-server/ba-p/14200825](https://community.sap.com/t5/technology-blog-posts-by-sap/give-your-ai-agent-some-tools-introducing-the-ui5-mcp-server/ba-p/14200825)

[https://github.com/UI5/mcp-server#setup](https://github.com/UI5/mcp-server#setup)

## 📱MDK

[https://community.sap.com/t5/technology-blog-posts-by-sap/developing-mobile-apps-with-ai-agents-introducing-the-mcp-server-for-mobile/ba-p/14237709](https://community.sap.com/t5/technology-blog-posts-by-sap/developing-mobile-apps-with-ai-agents-introducing-the-mcp-server-for-mobile/ba-p/14237709)

[https://github.com/SAP/mdk-mcp-server](https://github.com/SAP/mdk-mcp-server)

# 🛕 Community MCP Server

Story / Explanation of a Custom SAP MCP Server:

[Product comparison from SAP against online sources using Artificial Intelligence and MCP](https://www.linkedin.com/pulse/product-comparison-from-sap-against-online-sources-using-tom-cenens-nemme/)

## 📘Documentation

### 💬 Chat

Local running (docker container) chat that brings the power of several MCP Servers to the local machine.

|Server|Purpose|Requires|
|---|---|---|
|SAP Docs ✅|Documentation & Community search|Nothing (always works)|
|SAP Notes|Official Knowledge Base search|S-User certificate|
|S4/HANA|OData services access|SAP system credentials|
|ABAP ADT|Direct SAP system access|SAP development system|

[Supercharged Local Open Source Joule for Consultants: Search Your Data & Code](https://www.linkedin.com/pulse/supercharged-local-open-source-joule-consultants-search-marian-zeis-gepbf/)

[GitHub - marianfoo/local-llm-client-for-sap-consultants-librechat: This is fork of LibreChat to showcase the usage with MCP Server for SAP Data](https://github.com/marianfoo/local-llm-client-for-sap-consultants-librechat/tree/main)

### 💽 Servers

[https://www.linkedin.com/pulse/ditch-joule-open-source-mcp-servers-btp-give-you-more-marian-zeis-wttpf](https://www.linkedin.com/pulse/ditch-joule-open-source-mcp-servers-btp-give-you-more-marian-zeis-wttpf)

[https://github.com/marianfoo/mcp-sap-docs](https://github.com/marianfoo/mcp-sap-docs)

[https://github.com/marianfoo/mcp-sap-notes](https://github.com/marianfoo/mcp-sap-notes)

[https://github.com/marianfoo/local-llm-client-for-sap-consultants-librechat](https://github.com/marianfoo/local-llm-client-for-sap-consultants-librechat)

[https://www.linkedin.com/pulse/supercharged-local-open-source-joule-consultants-search-marian-zeis-gepbf/](https://www.linkedin.com/pulse/supercharged-local-open-source-joule-consultants-search-marian-zeis-gepbf/)

## 📡 OData

[https://github.com/lemaiwo/btp-sap-odata-to-mcp-server](https://github.com/lemaiwo/btp-sap-odata-to-mcp-server)

  

[https://community.sap.com/t5/technology-blog-posts-by-members/universal-odata-mcp-bridge-or-how-i-accidentally-made-15-000-enterprise/ba-p/14134696](https://community.sap.com/t5/technology-blog-posts-by-members/universal-odata-mcp-bridge-or-how-i-accidentally-made-15-000-enterprise/ba-p/14134696)

[https://github.com/oisee/odata_mcp_go](https://github.com/oisee/odata_mcp_go)

## 🧢 CAP

[GitHub - gavdilabs/cap-mcp-plugin: MCP (Model Context Protocol) server plugin for CAP NodeJS](https://github.com/gavdilabs/cap-mcp-plugin)

  

## 🈷️ BTP

[https://www.denisreis.com/eigenen-mcp-server-auf-sap-btp-einrichten/](https://www.denisreis.com/eigenen-mcp-server-auf-sap-btp-einrichten/)

[https://dev.to/lechnerc77/test-drive-the-terraform-mcp-server-with-github-copilot-chat-3jf1](https://dev.to/lechnerc77/test-drive-the-terraform-mcp-server-with-github-copilot-chat-3jf1)

## 🧑‍💻 ABAP

[Finally: An MCP Server for ABAP](https://blog.zeis.de/posts/2026-02-04-abap-mcp-server/)