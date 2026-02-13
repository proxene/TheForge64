# 🎮 JoyForge64 – CJM Generator C64 Mini & Maxi

<br />

![CJM](https://img.shields.io/badge/output-.cjm%20generator-blue?style=for-the-badge)
![Platform](https://img.shields.io/badge/target-C64%20Mini%20%26%20Maxi-darkblue?style=for-the-badge)
![Contributions](https://img.shields.io/badge/contributions-open-brightgreen?style=for-the-badge)
![Data](https://img.shields.io/badge/Language-JSON-black?logo=json&style=for-the-badge)

<br />

This project is a software tool that allows users to generate **.cjm configuration files**  
for the **Commodore 64 Mini and Maxi joystick system**.

The generated `.cjm` files define custom joystick mappings and game configurations  
compatible with the C64 Mini & Maxi systems.

<br />

> [!IMPORTANT]
> 🚧 **Project Status: Work in Progress**
>  
> This software is still under development.  
> Breaking changes may occur before the first stable release.

<br />

<details>
<summary>📌 How to Request a New Game</summary>
    
<br>
    
If you would like to add a new game to the project:

1. Create a new **GitHub Issue**
5. One game per issue.
2. Add the label: would like to be added.
3. Include the completed JSON structure below inside the Issue description.
4. Make sure your JSON is valid.

⚠️ Submissions without the correct label or JSON format may be ignored.

<br />

### 📝 Required JSON Format

Copy, complete, and paste the following JSON into your Issue:

```json
{
    "Game Title": {
        "header": "Picture URL",
        "desc": "Game Description",
        "type": "Game Genre",
        "port": "2",
        "players": "1",
        "inputs": {
            "player-1": {
                "input-1": ["Move Up", "W", "JU"],
                "input-2": ["Move Down", "S", "JD"],
                "input-3": ["Move Left", "A", "JL"],
                "input-4": ["Move Right", "D", "JR"],
                "input-5": ["Fire", "LSHIFT", "JFR"]
            }
        }
    }
}
```

Multiplayer Example (Two Controllers)

```json
{
    "Example Multiplayer Game": {
        "header": "Picture URL",
        "desc": "Game description here.",
        "type": "Arcade",
        "port": "2",
        "players": "2",
        "inputs": {
            "player-1": {
                "input-1": ["Move Up", "W", "JU"],
                "input-2": ["Move Down", "S", "JD"],
                "input-3": ["Fire", "LSHIFT", "JFR"]
            },
            "player-2": {
                "input-1": ["Move Up", "I", "JU"],
                "input-2": ["Move Down", "K", "JD"],
                "input-3": ["Fire", "RSHIFT", "JFR"]
            }
        }
    }
}

```

<br />

### 📖 Field Explanation

- `Game Title` Name of the game.
- `header` URL to the game's main image.
- `desc` Short description of the game.
- `type` Game genre (Platformer, Shooter, Puzzle, etc.).
- `port` Joystick port used: `1` or `2`.
- `players` Must be either `1` or `2`.
- `inputs` Control mapping configuration for the game.

<br />

### 🕹️ C64 Slot (Mapping ID)
| ID   | Description      |
|-------|------------------|
| JU    | Joystick Up      |
| JD    | Joystick Down    |
| JL    | Joystick Left    |
| JR    | Joystick Right   |
| JFL   | Fire Left        |
| JFR   | Fire Right       |
| TL    | Top Left         |
| TR    | Top Right        |
| Y     | Bottom Button 1  |
| X     | Bottom Button 2  |
| A     | Bottom Button 3  |
| B     | Bottom Button 4  |
    
</details>

<br />

## 🙌 Contributions

Thank you for helping expand compatibility for the<br />
Commodore 64 Mini & Maxi CJM ecosystem!

Happy retro gaming 🚀
