{
    // rectangle, square, circle, flex-center, absolute-center
    // transform, transition-hover
    // box-shadow-black, box-shadow-white
    // reset body, reset a
    // text-style, button-style
    // content, before-after
    // icon-style, icon-style-box
    // paste, bracket(f/j)
    // rem

    "rectangle": {
        "prefix": "rectangle",
        "body": [
            "width: ${1:1rem};",
            "height: ${2:1rem};",
            "background-color: #${3:000};",
            "border-radius: ${4:1rem};"
        ],
        "description": "make a rectangle"
    },
    "square": {
        "prefix": "square",
        "body": [
            "width: ${1:1rem};",
            "height: ${1:1rem};",
            "background-color: #${2:000};",
            "border-radius: ${3:1rem};"
        ],
        "description": "make a square"
    },
    "circle": {
        "prefix": "circle",
        "body": [
            "width: ${1:1rem};",
            "height: ${1:1rem};",
            "background-color: #${2:000};",
            "border-radius: 50%;"
        ],
        "description": "make a circle"
    },
    "flex center": {
        "prefix": "flex-center",
        "body": [
            "display: flex;",
            "justify-content: center;",
            "align-items: center;"
        ],
        "description": "flex center"
    },
    "absolute center": {
        "prefix": "absolute-center",
        "body": [
            "position: absolute;",
            "top: 50%;",
            "left: 50%;",
            "transform: translate(-50%, -50%);"
        ],
        "description": "absolute center"
    },
    "transform: translate rotateZ scale": {
        "prefix": "transform",
        "body": [
            "transform:${1: translate(${2:0}, ${3:0})}${4: rotateZ(${5:0}deg)}${6: scale(${7:1})};"
        ],
        "description": "transform: translate rotateZ scale"
    },
    "transition: hover": {
        "prefix": "transition-hover",
        "body": [
            "transition: ${1|ease,ease-in,ease-out,ease-in-out,linear|} ${2:0.3}s;"
        ],
        "description": "transition: hover"
    },
    "box shadow black": {
        "prefix": "box-shadow-black",
        "body": [
            "box-shadow: rgba(50, 50, 93, 0.25) 0 0.125rem 0.3125rem -0.0625rem,",
            "    rgba(0, 0, 0, 0.3) 0 0.0625rem 0.1875rem -0.0625rem;"
        ],
        "description": "box shadow black"
    },
    "box shadow white": {
        "prefix": "box-shadow-white",
        "body": [
            "box-shadow: rgba(205, 205, 162, 0.25) 0 0.125rem 0.3125rem -0.0625rem,",
            "    rgba(255, 255, 255, 0.3) 0 0.0625rem 0.1875rem -0.0625rem;"
        ],
        "description": "box shadow white"
    },
    "reset body": {
        "prefix": "reset-body",
        "body": ["box-sizing: border-box;", "margin: 0;", "padding: ${1:0};"],
        "description": "reset body"
    },
    "reset a": {
        "prefix": "reset-a",
        "body": ["text-decoration: none;", "color: #${1:000};"],
        "description": "reset a"
    },
    "text style": {
        "prefix": "text-style",
        "body": [
            "font-size: ${1:1rem};",
            "text-transform: ${2|uppercase,lowercase,capitalize|};",
            "letter-spacing: ${3:1rem};",
            "color: #${4:000};"
        ],
        "description": "text style"
    },
    "button style": {
        "prefix": "button-style",
        "body": [
            "font-size: ${1:1rem};",
            "text-transform: ${2|uppercase,lowercase,capitalize|};",
            "letter-spacing: ${3:1rem};",
            "color: $${4:$darkGrey};",
            "background-color: $${5:lightGrey};",
            "padding: ${6:1rem} ${7:2rem};",
            "border-radius: ${8:1rem};",
            "transition: ${9|ease,ease-in,ease-out,ease-in-out,linear|} ${10:0.3}s;",
            "box-shadow: rgba(50, 50, 93, 0.25) 0 0.125rem 0.3125rem -0.0625rem,",
            "    rgba(0, 0, 0, 0.3) 0 0.0625rem 0.1875rem -0.0625rem;",
            "cursor: pointer;",
            "",
            "&:hover {",
            "    color: $${11:lightGrey};",
            "    background-color: $${12|darkRed,darkGreen,darkBlue,darkOrange,darkYellow|};",
            "box-shadow: inset rgba(50, 50, 93, 0.25) 0 0.125rem 0.3125rem -0.0625rem,",
            "    inset rgba(0, 0, 0, 0.3) 0 0.0625rem 0.1875rem -0.0625rem;",
            "}"
        ],
        "description": "button style"
    },
    "content empty": {
        "prefix": "content",
        "body": ["content: \"\";"],
        "description": "content empty"
    },
    "before or after": {
        "prefix": "before-after",
        "body": [
            "position: relative;",
            "",
            "&::${1|before,after|} {",
            "    content: \"\";",
            "    width: ${2:1rem};",
            "    height: ${3:1rem};",
            "    background-color: #${4:fff};",
            "    border-radius: ${5:1rem};",
            "    position: absolute;",
            "    top: 50%;",
            "    left: 50%;",
            "    transform: translate(-50%, -50%);",
            "}"
        ],
        "description": "before or after"
    },
    "icon style": {
        "prefix": "icon-style",
        "body": [
            "font-size: ${1:1rem};",
            "color: $$darkGrey;",
            "cursor: pointer;",
            "transition: ${2|ease,ease-in,ease-out,ease-in-out,linear|} ${3:0.3}s;",
            "",
            "&:hover {",
            "    color: $${4|darkRed,darkGreen,darkBlue,darkOrange,darkYellow|};",
            "    transform: rotateZ(${5:10}deg) scale(${6:1.2});",
            "}"
        ],
        "description": "icon style"
    },
    "icon style box": {
        "prefix": "icon-style-box",
        "body": [
            "display: flex;",
            "align-items: center;",
            "font-size: ${1:1rem};",
            "padding: ${2:1rem};",
            "color: $$darkGrey;",
            "background-color: $$lightGrey;",
            "border-radius: ${3:1rem};",
            "transition: ${4|ease,ease-in,ease-out,ease-in-out,linear|} ${5:0.3}s;",
            "box-shadow: rgba(50, 50, 93, 0.25) 0 0.125rem 0.3125rem -0.0625rem,",
            "    rgba(0, 0, 0, 0.3) 0 0.0625rem 0.1875rem -0.0625rem;",
            "cursor: pointer;",
            "",
            "&:hover {",
            "    color: $$lightGrey;",
            "    background-color: $${6|darkRed,darkGreen,darkBlue,darkOrange,darkYellow|};;",
            "    box-shadow: inset rgba(50, 50, 93, 0.25) 0 0.125rem 0.3125rem -0.0625rem,",
            "        inset rgba(0, 0, 0, 0.3) 0 0.0625rem 0.1875rem -0.0625rem;",
            "}"
        ],
        "description": "icon style box"
    },
    "Clipboard to comment": {
        "prefix": "paste",
        "body": ["$BLOCK_COMMENT_START $CLIPBOARD $BLOCK_COMMENT_END"],
        "description": "Clipboard to comment"
    },
    "A new block": {
        "prefix": ["f", "j", "bracket"],
        "body": ["{", "\t$0", "}"],
        "description": "A new block"
    },
    "px to rem": {
        "prefix": "rem",
        "body": ["toRem($1)"],
        "description": "px to rem"
    }
}