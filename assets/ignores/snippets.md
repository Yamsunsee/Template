{
// rectangle, square, circle
// flex-center, flex-center-column, absolute-center
// transform, transition-hover
// box-shadow-black, box-shadow-white
// reset body, reset a
// text-style, button-style
// content, before-after
// icon-style, icon-style-box
// paste, bracket(f/j)
// rem
// color-board

    "rectangle": {
        "prefix": "rectangle",
        "body": [
            "width: ${1:1rem};",
            "height: ${2:1rem};",
            "background-color: ${3:#000};",
            "border-radius: ${4:1rem};"
        ],
        "description": "make a rectangle"
    },
    "square": {
        "prefix": "square",
        "body": [
            "width: ${1:1rem};",
            "height: ${1:1rem};",
            "background-color: ${2:#000};",
            "border-radius: ${3:1rem};"
        ],
        "description": "make a square"
    },
    "circle": {
        "prefix": "circle",
        "body": [
            "width: ${1:1rem};",
            "height: ${1:1rem};",
            "background-color: ${2:#000};",
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
    "flex center column direction": {
        "prefix": "flex-center-column",
        "body": [
            "display: flex;",
            "flex-direction: column;",
            "justify-content: center;",
            "align-items: center;"
        ],
        "description": "flex center column direction"
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
            "box-shadow: rgba(50, 50, 93, 0.25) 0 2px 5px -1px,",
            "    rgba(0, 0, 0, 0.3) 0 1px 3px -1px;"
        ],
        "description": "box shadow black"
    },
    "box shadow white": {
        "prefix": "box-shadow-white",
        "body": [
            "box-shadow: rgba(205, 205, 162, 0.25) 0 2px 5px -1px,",
            "    rgba(255, 255, 255, 0.3) 0 1px 3px -1px;"
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
        "body": ["text-decoration: none;", "color: ${1:#000};"],
        "description": "reset a"
    },
    "text style": {
        "prefix": "text-style",
        "body": [
            "font-size: ${1:1rem};",
            "text-transform: ${2|uppercase,lowercase,capitalize|};",
            "letter-spacing: ${3:1rem};",
            "color: ${4:#000};"
        ],
        "description": "text style"
    },
    "button style": {
        "prefix": "button-style",
        "body": [
            "font-size: ${1:1rem};",
            "text-transform: ${2|uppercase,lowercase,capitalize|};",
            "letter-spacing: ${3:1rem};",
            "color: ${4:#7f8c8d};",
            "background-color: ${5:#ecf0f1};",
            "padding: ${6:1rem} ${7:2rem};",
            "border-radius: ${8:1rem};",
            "transition: ${9|ease,ease-in,ease-out,ease-in-out,linear|} ${10:0.3}s;",
            "box-shadow: rgba(50, 50, 93, 0.25) 0 2px 5px -1px,",
            "    rgba(0, 0, 0, 0.3) 0 1px 3px -1px;",
            "cursor: pointer;",
            "",
            "&:hover {",
            "    color: ${11:#ecf0f1};",
            "    background-color: ${12|#eb4d4b|};",
            "    box-shadow: inset rgba(50, 50, 93, 0.25) 0 2px 5px -1px,",
            "        inset rgba(0, 0, 0, 0.3) 0 1px 3px -1px;",
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
            "    background-color: ${4:#fff};",
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
            "color: #7f8c8d;",
            "cursor: pointer;",
            "transition: ${2|ease,ease-in,ease-out,ease-in-out,linear|} ${3:0.3}s;",
            "",
            "&:hover {",
            "    color: ${4|#eb4d4b|};",
            "    transform: rotateZ(${5:-10}deg) scale(${6:1.2});",
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
            "color: #7f8c8d;",
            "background-color: #ecf0f1;",
            "border-radius: ${3:1rem};",
            "transition: ${4|ease,ease-in,ease-out,ease-in-out,linear|} ${5:0.3}s;",
            "box-shadow: rgba(50, 50, 93, 0.25) 0 2px 5px -1px,",
            "    rgba(0, 0, 0, 0.3) 0 1px 3px -1px;",
            "cursor: pointer;",
            "",
            "&:hover {",
            "    color: #ecf0f1;",
            "    background-color: ${6|#eb4d4b|};",
            "    box-shadow: inset rgba(50, 50, 93, 0.25) 0 2px 5px -1px,",
            "        inset rgba(0, 0, 0, 0.3) 0 1px 3px -1px;",
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
    },
    "color board": {
        "prefix": "color-board",
        "body": [
            "${1|#ff7979 /*Light Red*/,#eb4d4b /*Dark Red*/,#badc58 /*Light Green*/,#6ab04c /*Dark Green*/,#686de0 /*Light Blue*/,#4834d4 /*Dark Blue*/,#30336b /*Shallow Blue*/,#130f40 /*Deep Blue*/,#f6e58d /*Light Yellow*/,#f9ca24 /*Dark Yellow*/,#ffbe76 /*Light Orange*/,#f0932b /*Dark Orange*/,#ecf0f1 /*Light Grey*/,#7f8c8d /*Dark Grey*/|}"
        ],
        "description": "color board"
    }

}
