# Karabiner Elements Modifications

## Function keys

### Use F5 to change input language

On Windows keyboard, you don't get the `fn (globe)` key that modern macOS uses to change your input source language.
To get around that, I change the `F5` key—which usually starts dictation—to work as the `fn (globe)` key.

Change `f5` to: `Modifier keys` -> `fn (globe)`.

## Complex modifications

### Shift+Space -> Underscore

```json
{
    "description": "Shift+Space -> Underscore",
    "manipulators": [
        {
            "from": {
                "key_code": "spacebar",
                "modifiers": {
                    "mandatory": ["left_shift"],
                    "optional": ["any"]
                }
            },
            "to": [
                {
                    "key_code": "hyphen",
                    "modifiers": ["left_shift"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "spacebar",
                "modifiers": {
                    "mandatory": ["right_shift"],
                    "optional": ["any"]
                }
            },
            "to": [
                {
                    "key_code": "hyphen",
                    "modifiers": ["right_shift"]
                }
            ],
            "type": "basic"
        }
    ]
}
```