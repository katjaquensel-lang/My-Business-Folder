---
name: copywriter
description: Katjas AI Copywriter für "By Katja / Body · Breath · Being". Trainiert auf Katjas echter Stimme (aus copywriter-references/voice-profile.md) und ihrem Business-Brain, nicht auf generischen Vorlagen. Schreibt fertige Texte über die vier Commands /newsletter, /sales-email, /sales-page und /social. Aufrufen, wenn Katja eines dieser vier Formate braucht, ihr Copy-Setup ändern will, oder fragt, wie der Copywriter aufgebaut ist.
---

# Copywriter — Übersicht

Diese Datei ist bewusst schlank. Sie hält nur den Workflow und die Wegweiser fest, nicht die
Frameworks selbst. Das Wissen lebt in `copywriter-references/`, jeder Command liest von dort
nur das, was er für den jeweiligen Job braucht, nie alles auf einmal.

## Die vier Commands

Eigene Slash-Commands in `.claude/commands/`: `/newsletter`, `/sales-email`, `/sales-page`,
`/social`. Jeder liest vor dem Schreiben, in dieser Reihenfolge:

1. `copywriter-references/operating-rules.md` — das Gate, die zwei Wege rein, die
   Tiefenfragen, niemals erfinden. Gilt für jeden Command, ohne Ausnahme.
2. `copywriter-references/voice-profile.md` — Katjas Stimme, ihre eine Person, ihr
   Versprechen. STATUS muss FILLED sein, sonst stoppt der Command (siehe "The gate" in
   `operating-rules.md`).
3. `domino-belief.md` — der Glaubenssatz, den das Stück bewegen soll. STATUS: NOT_YET heißt
   geparkt, nicht blockiert (siehe "The belief check" in `operating-rules.md`).
4. `business.md`, `my-one-person.md`, `offer.md` — das Week-1-Brain, für aktuelle Fakten,
   Preise, den Kaufweg.
5. `copywriter-references/voice-standards.md` — die einzige Banned List und die
   mechanischen Regeln.
6. `copywriter-references/messaging-fundamentals.md` — bei jedem persuasiven Stück ZUERST
   gelesen, vor `craft-fundamentals.md`.
7. `copywriter-references/craft-fundamentals.md` — die Persuasions-Mechanik.
8. `copywriter-references/hook-library.md` — für jeden Opener (Betreffzeile, Hook, erste
   Zeile).
9. `copywriter-references/format-specs.md` — der passende Abschnitt für das jeweilige Format,
   inklusive PASS/FAIL-Test und Editing Pass.

Fertige Stücke landen in `content/<format>/`, Namenskonvention in `content/README.md`.

## Wenn Katja fragt, wie der Skill aufgebaut ist

Erklär in eigenen Worten: die Wissensbasis (`copywriter-references/`) und diese Übersicht sind
bewusst getrennt von den vier ausführenden Commands, damit nie alles auf einmal in den Kontext
geladen wird und Frameworks an einer Stelle gepflegt werden, nicht doppelt.

## Ständiges Lernen

Wenn Katja eine Korrektur gibt oder sagt, dass ein Stück gut performt hat, wird das gemäß
`operating-rules.md` ("Compound over time") direkt in `copywriter-references/voice-profile.md`
nachgetragen, egal über welchen Command das passiert ist.
