---
name: install-chiikawa
description: Install or activate the animated Chiikawa ChatGPT Work pet bundled with this plugin. Use only when the user explicitly asks to install, add, or select this bundled pet in ChatGPT Pets. Do not use for real pets, generic image generation, or pets in other apps.
---

# Install the bundled Chiikawa pet

Use the sprite sheet at `../../assets/chiikawa-spritesheet.png`, resolved from this `SKILL.md` file to an absolute path before calling tools.

## Requirements

- The user must have the ChatGPT Pets feature and its pet-management tools available.
- Installing this plugin alone does not grant Pets access or workspace permissions.
- Keep the bundled artwork unchanged during installation.

## Procedure

1. Treat an explicit request to install and select this bundled pet as authorization to create and activate a custom pet in the user's own Pets library.
2. If `list_pets` is available, page through the user's pets and check for a custom pet named `치이카와` with the description below. If one clearly matches, select it instead of creating a duplicate.
3. Call `validate_pet_spritesheet` with the bundled PNG. Continue only when it returns `valid: true`.
4. Call `prepare_pet_upload` for that exact validated PNG.
5. Call `create_pet` using the returned upload session with:
   - Name: `치이카와`
   - Description: `작고 하얗고 귀여운 치이카와. 수줍지만 씩씩하게 곁에서 함께해요.`
6. Call `select_pet` with the newly created stable pet ID.
7. Page through `list_pets` until that stable ID appears and verify that it is active, then report success concisely.

If a required Pets tool is unavailable, stop without fabricating a result and explain that the user must install or enable the official Pets plugin or feature first. Never reuse the original creator's pet ID, upload-session ID, or expiring download URL; each recipient must create a separate user-owned copy from the bundled sprite sheet.
