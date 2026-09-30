# Dermly Design System — extracted from Mobbin best-in-class

Source apps studied (iOS): Lovi, Yuka, Hims, Hers, Shop, Amazon, Finch, Anything, Me+, Atoms, Noom, Lifesum, Bevel, Alan, Superpower, Wysa, WHOOP, Bloom, MacroFactor, Future Pro, Hevy, 5-Minute Journal, Lifesum reminders, Linear notifications.

## Tokens (in `styles.css`)
`--bg #FFF`, `--layer-1 #F7F7F7`, `--layer-2 #EFEFEF`, `--accent-1 #564CD8`, `--accent-1-bg #ECEBFF`, `--text-primary #252525`, `--text-secondary #515151`, `--green #1A9E6B / bg #E3F5EC`, `--amber #B7791F / bg #FFF3D6`, `--red #C0392B / bg #FDECEA`, radius 18/12, shadow soft.

Masculine-minimal, coach tone. Light mode default.

## Primitives (atoms)
- **Pill / Badge**: fit score, Verified, streak. Variants: accent/green/amber/red/ink. Seen in [Lovi](https://mobbin.com/screens/a41314ee-2647-4e99-b980-0a8d3f9202c8), [Shop](https://mobbin.com/screens/ef10e023-4549-43cf-a7f3-31ff7a52ae56)
- **Progress bar**: thin 8px, accent fill. Seen in [Anything](https://mobbin.com/screens/5d0e3b4b-a4a5-4e4d-b969-7577157db613), [Life Reset](https://mobbin.com/screens/bb668112-fb6b-45f4-887a-6020a472836e)
- **Match Ring**: conic 0-100, color green≥85 amber≥70 red<70. Derived from [Yuka](https://mobbin.com/flows/3c3ef945-4b30-4ce6-9484-547831d37c0d) 18/100 + Eight Sleep score pattern.
- **Toggle**: 48×28, green on. Seen in [Linear](https://mobbin.com/screens/ce91edc6-fa41-4569-9b98-cd74393be1ff), [Whering](https://mobbin.com/screens/7bd14b82-6a82-4bfc-a3fe-665ddf14b8c4)
- **DayDots**: S M T W T F S circles, black on. Seen in [Linear](https://mobbin.com/screens/ce91edc6-fa41-4569-9b98-cd74393be1ff), [Lifesum](https://mobbin.com/screens/3c87d41c-24b9-4c79-bf2a-9f0d9e1dfb32), [Beside](https://mobbin.com/screens/9c8b3f33-0677-449d-86ba-6414ef1f940e)
- **Radio / Check circle**: 22px, accent fill + ✓. Seen in Lovi quiz.
- **Chat bubbles**: AI grey left, user accent right + suggestion pills. Seen in [Lovi Assistant](https://mobbin.com/screens/0b005810-b6a0-43e9-91db-7bf275f2b9d6), [Noom](https://mobbin.com/screens/07534750-301d-447f-be43-b8e0fcb429bc), [WHOOP](https://mobbin.com/screens/be86b426-71e2-4e2a-adea-a5bc28a2de15), [Bevel](https://mobbin.com/screens/adaa1131-21f2-4250-96e4-4ba69b799acf)
- **Vendor row**: dot + name + rating + price + ship/return. Distinct product-score vs seller-trust. Seen in [Amazon](https://mobbin.com/screens/e9f86b85-52b8-4e65-8f73-85f30af019a8), [Target](https://mobbin.com/screens/16dd9f33-86d3-430e-ad06-2896b0e1713e)
- **Timeline cards**: W1/W4/W8 + Before/After. Seen in [MacroFactor](https://mobbin.com/screens/43d26ac6-2fb3-4158-9936-079dd1f81278), [Future Pro](https://mobbin.com/screens/1f3ee51f-cbcc-4fcd-8648-24546d890ce2), [Yazio](https://mobbin.com/screens/7f05927d-90a9-4fc4-be2b-633648fb1664)

## Domain-specific components
- `ScanFrame`: dark visual + oval + animated line + Barcode/Ingredients chips. From Yuka + Lovi face scan.
- `QuizCard`: single-Q, illustrated rows, 1/5 progress. From Lovi + Amazon quiz.
- `RoutineStep`: num tile + AM/PM pill + Done/Skip + tap → RoutineDetail (What/Why/How/When/Frequency/Not-combine). From Lovi routine + Me+ + Finch.
- `ProductCard`: brand+name + fit pill + cat·price·when. From Shop/CVS/Hers.
- `TierGroup`: Best/Budget/Premium/Alternative left-border. From Yuka Recommendations + Amazon Best Seller.
- `StreakCluster`: 🔥 days + AM% + PM% + week dots. From Bloom, pushr, Anything.
- `MoodDiary`: 5 emoji buttons. From Lovi Skin Diary.
- `ReminderRow`: Morning/Evening + time select + days. From Lifesum + 5-Min Journal + stoic.

## Standard components with Dermly variants
- Buttons: primary accent, ink (tracker), ghost layer-1. Full-width 15px padding, 16px radius.
- Accordion (`How to use`, `Product details`): from [Hers](https://mobbin.com/screens/3dcab988-67bb-407d-834f-8b3defb967f3)
- Search + Scan split button: from Amazon lens/barcode pattern.
- Bottom tabbar 5: Today/Routine/Scan-fab/Coach/You. Badges from Lovi tabbar.

## Usage rules
- Score always paired with reason (never number alone). Green/amber/red + text Yes/Maybe/Not.
- Every AI result ends with action: Add to routine / Where to buy / Set reminder / Track.
- Safety microcopy on scan + analysis + assistant: “estimate, cosmetic only”.
- Sponsored labeled; scores not buyable.
