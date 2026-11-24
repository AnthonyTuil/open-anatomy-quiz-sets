# Open anatomy quiz sets

Free, reusable anatomy quiz data: **254 structures** of the human body (136 muscles, 96 bones, 22 organs) with English names, Latin names from Terminologia Anatomica 2 where available, muscle actions, a one-line summary, and how they group into **17 study themes** at three levels.

It is the data behind the free 3D anatomy quiz at **https://anatomyatlas3d.app/quiz/**, where students find, name and type these structures on a 3D model of the body, in any browser, with no install and no ads.

Use it to build flashcards, Anki decks, worksheets, lab practical checklists, or your own quiz.

## Files

| File | What it holds |
|---|---|
| `data/structures.json` | One record per structure: `id`, `name`, `latin`, `kind` (muscle, bone, organ), `layer`, `actions`, `summary`, the `themes` and levels it belongs to, and a `page` with more detail |
| `data/structures.csv` | The same records as a spreadsheet |
| `data/themes.json` | The 17 themes, their three levels and the named groups (for example the rotator cuff muscles) |

## Themes

| Theme | Structures |
|---|---|
| [Shoulder](https://anatomyatlas3d.app/quiz/shoulder/) | 18 |
| [Arm and elbow](https://anatomyatlas3d.app/quiz/arm-and-elbow/) | 11 |
| [Forearm and hand](https://anatomyatlas3d.app/quiz/forearm-and-hand/) | 49 |
| [Thorax](https://anatomyatlas3d.app/quiz/thorax/) | 23 |
| [Back](https://anatomyatlas3d.app/quiz/back/) | 36 |
| [Abdomen](https://anatomyatlas3d.app/quiz/abdomen/) | 17 |
| [Pelvis](https://anatomyatlas3d.app/quiz/pelvis/) | 12 |
| [Hip and thigh](https://anatomyatlas3d.app/quiz/hip-and-thigh/) | 27 |
| [Leg and foot](https://anatomyatlas3d.app/quiz/leg-and-foot/) | 45 |
| [Head](https://anatomyatlas3d.app/quiz/head/) | 30 |
| [Neck](https://anatomyatlas3d.app/quiz/neck/) | 23 |
| [Skeleton](https://anatomyatlas3d.app/quiz/skeleton/) | 96 |
| [Upper limb muscles](https://anatomyatlas3d.app/quiz/upper-limb-muscles/) | 45 |
| [Lower limb muscles](https://anatomyatlas3d.app/quiz/lower-limb-muscles/) | 39 |
| [Trunk muscles](https://anatomyatlas3d.app/quiz/trunk-muscles/) | 23 |
| [Head and neck muscles](https://anatomyatlas3d.app/quiz/head-and-neck-muscles/) | 39 |
| [Organs](https://anatomyatlas3d.app/quiz/organs/) | 22 |

Level 1 holds the structures most courses start with, level 3 the deeper or smaller ones.

## Example

```json
{
  "id": "supraspinatus",
  "name": "Supraspinatus",
  "latin": "Musculus supraspinatus",
  "kind": "muscle",
  "themes": [{"theme": "shoulder", "level": 1}, {"theme": "upper-limb-muscles", "level": 2}],
  "page": "https://anatomyatlas3d.app/muscles/supraspinatus/"
}
```

## Sources and limits

- English and Latin names follow Terminologia Anatomica 2 (TA2). Some structures have no Latin name in this set yet (`latin` is `null`).
- Summaries were written for Anatomy Atlas 3D and checked against open references, including Z-Anatomy (CC BY-SA 4.0) and the OpenStax *Anatomy and Physiology* textbook.
- This repository holds no 3D models, meshes or images.
- For education only. It is not medical advice. If you find an error, open an issue.

## License

The data is shared under [Creative Commons Attribution-ShareAlike 4.0](LICENSE) (CC BY-SA 4.0). Credit "Open anatomy quiz sets, Anatomy Atlas 3D (https://anatomyatlas3d.app/)" and share changes under the same license.

## Links

- Free 3D anatomy quiz in the browser: https://anatomyatlas3d.app/quiz/
- Free 3D anatomy atlas for iPhone and iPad: https://apps.apple.com/us/app/anatomy-atlas-3d-human-body/id6812062444
- For instructors: https://anatomyatlas3d.app/instructors/
