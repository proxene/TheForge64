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

## 📌 How to Request a New Game

If you would like to add a new game to the project:

1. Create a new **GitHub Issue**
2. Add the label:
3. Include the completed JSON structure below inside the Issue description.

⚠️ Only issues containing the correct label and valid JSON will be reviewed.

<br />

## 📝 Required JSON Format

Copy, complete, and paste the following JSON into your Issue:

```json
{
    "Game Title": {
        "header": "Picture URL",
        "desc": "Game Description",
        "type": "Game Type",
        "players": "single or multi",
        "port": "Joystick port 1 or 2",
        "inputs": {
            "j-up": ["Move UP", "JU"],
            "j-down": ["Move Down", "JD"],
            "j-left": ["Move Left", "JL"],
            "j-right": ["Move Right", "JR"],
            "b-fire1": ["Fire 1", ""],
            "b-fire2": ["Fire 2", "JF"],
            "b-cornerleft": ["Top Left", ""],
            "b-cornerright": ["Top Right", ""],
            "b-bottom1": ["A", "F1"],
            "b-bottom2": ["B", "F3"],
            "b-bottom3": ["C", "F5"],
            "b-bottom4": ["Select", "F7"]
        }
    }
}
```

<br />

## 📖 Field Explanation

- `Game Title` Name of the game.
- `header` URL to the game's main image.
- `desc` Short description of the game.
- `type` Game genre (Platformer, Shooter, Puzzle, etc.).
- `players` Must be either `single` or `multi`.
- `port` Joystick port used: `1` or `2`.
- `inputs` Control mapping configuration for the game.

<br />

## ⚠️ Important Notes

Make sure your JSON is valid.<br />
Do not modify existing game entries.<br />
One game per issue.

Submissions without the correct label or JSON format may be ignored.

<br />

## 🙌 Contributions

Thank you for helping expand compatibility for the<br />
Commodore 64 Mini & Maxi CJM ecosystem!

Happy retro gaming 🚀
