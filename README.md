# Translation repository for Internal Trainer - Resident Evil 4 UHD (Steam)

Thank you for helping with translations! This guide explains how to translate strings for the trainer.

## What You Need to Do

You will have access to the main localization file in English, being able to download or fork to make changes.

Your task is to translate these phrases to your language while following a few important rules.

## Translation Format

Each translation entry consists of two parts:
1. The original English text (used as a reference)
2. Your translation in your language

Example:
```
Original: English[TranslationKeys::PLAYER_INVINCIBLE] = "Player Invincible";
Translation: Spanish[TranslationKeys::PLAYER_INVINCIBLE] = "Jugador Invencible";
```

## Important Rules to Follow

1. **Keep Formatting Codes**: If you see percentage signs like %d, %.1f, these are formatting codes. Keep them in your translation.
   ```
   Original: English[TranslationKeys::CLEANUPS_IN_SESSION] = "Cleanings in this session: %d";
   Translation: Spanish[TranslationKeys::CLEANUPS_IN_SESSION] = "Limpieza en esta sesión: %d";
   ```

2. **Maintain Line Breaks**: If the original text has line breaks (shown as \n), keep them in your translation.
   ```
   Original: English[TranslationKeys::MONEY_HELPMARK] = "You can manipulate the amount of money that enemies can drop.\n\nTo avoid being so overpowered, not all money drops will be increased/decreased.";
   Translation: Spanish[TranslationKeys::MONEY_HELPMARK] = "Puedes modificar la cantidad de dinero que sueltan los enemigos.\n\nPara evitar estar demasiado sobrepoderado, no todas las monedas que caigan se verán aumentadas o disminuidas.";
   ```

3. **Keep Special Punctuation**: Maintain all punctuation marks (!, ?, :, etc.) in your translation.

4. **Some texts have intentional spaces at the beginning, for example:**
   ```
   English[TranslationKeys::HEALTH_THRESHOLDS] = " Health Thresholds:";
   -
   This is necessary to maintain the layout.
   ```

5. **Respect Text Length**: Try to keep translations similar in length to the originals when possible.

6. **Be Consistent**: Use the same translation for repeated terms throughout the file.

7. **Maintain Context**: Some strings might be part of the user interface - try to understand their context before translating.

## Special Cases

### Template Strings
Some strings are templates (like file formats). For these, only translate the visible text parts, not the structural elements:

```
Original:
"TITLE=\n"
"FILENAME=\n"
"URL=\n"
"START=0.0\n"
"\n"
"1.0|First lyric line\n"
"3.0|Second lyric line"

Translation:
"TITLE=\n"
"FILENAME=\n"
"URL=\n"
"START=0.0\n"
"\n"
"1.0|Primera línea de letra\n"
"3.0|Segunda línea de letra"
```

### Help Text
For longer help texts, ensure your translation captures the meaning while keeping any technical information intact.

## Example Translations

Original:
```
"Health restored!"
```

Spanish translation:
```
"¡Salud restaurada!"
```

Original:
```
"Your progress will be automatically saved in the last slot used.\n\nThere's no risk of data corruption, but since the system saves on its own, it might overwrite a slot you didn't want to change."
```

Spanish translation:
```
"Tu progreso se guardará automáticamente en el último espacio utilizado.\n\nNo hay riesgo de corrupción de datos, pero como el sistema guarda por sí solo, podría sobrescribir un espacio que no querías cambiar."
```

## How to Submit Your Translation

Once you've completed your translation:
1. Open a pull request or send it via email to (contact@kreedy.net) to be added in a future update.
2. Be available for any questions about your translation or incoming updates bringing new features.
3. Your name will be added to the Hall of Fame as a translator.

IMPORTANT: Russian language will NOT be accepted, do not insist, it has been banned for breach of trust.

## Thank You!

Your contribution helps make the trainer accessible to more players. Thank you for your time and effort!
