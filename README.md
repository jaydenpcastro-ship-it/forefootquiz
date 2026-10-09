# Forefoot Live

*Tarsometatarsal & metatarsophalangeal joints: bones, ligaments, muscles, nerves & arteries*

A live, Kahoot-style multiplayer quiz on the forefoot. Students join from their own phones
(no account, no sign-in, no app): open the link or scan the host's QR code, type a name, and answer.

- 10 multiple-choice questions
  - Q1-5, passive structures: TMT articulations (cuboid with MT4-5), Lisfranc ligament,
    2nd metatarsal "keystone", MTP joint classification, deep transverse metatarsal ligament
  - Q6-10, active structures: fibularis longus insertion, flexor hallucis brevis innervation,
    lumbrical origin, interossei innervation, deep plantar artery
- 5-second reading window on each question (answers locked, "Read 5s" countdown), then a
  20-second answer timer (configurable, 10-60s); speed-weighted scoring counts from when answers open
- Host-only Pause / Resume (button, or Space / P)
- Live leaderboard, final podium, automatic winner

Live site: <https://forefootquiz.vercel.app>

## Files

- `index.html`: the whole app (host + player screens)
- `questions.js`: the question set (`q`, `options`, `correct` = 0-based index)
- `config.js`: Supabase project URL + publishable key
- `schema.sql`: database tables and policies (run once in the Supabase SQL Editor)

Built from the same template as `khalilrehabquiz` / `aclquiz`; it uses the same Supabase
project as those quizzes (games are kept apart by their 4-letter room codes).
