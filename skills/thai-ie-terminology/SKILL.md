---
name: thai-ie-terminology
description: ค้นหา ตรวจสอบ และรวบรวมคำศัพท์ภาษาไทยของสาขาวิศวกรรมอุตสาหการ (Industrial Engineering) จากแหล่งที่น่าเชื่อถือ (ราชบัณฑิตยสภา ตำราและวิทยานิพนธ์ไทย มาตรฐาน/สมาคมวิชาชีพ และเว็บทั่วไป) แล้วเสนอคำแปลที่ควรใช้พร้อมเหตุผลและแหล่งอ้างอิง. Use this skill whenever the user is writing a Thai textbook, thesis, paper, or lecture notes in industrial engineering and needs Thai equivalents or consistent terminology — operations research (OR), queueing, linear programming, simulation, ergonomics, safety, work study / time study, production planning, inventory, logistics, supply chain, quality control, SPC, DOE, reliability, statistics — or asks "คำนี้ภาษาไทยใช้ว่าอะไร", "ศัพท์บัญญัติ", "แปลศัพท์วิศวกรรม", "ทับศัพท์หรือแปล", or to build a glossary/อภิธานศัพท์, even if they never say "terminology".
---

# Thai Industrial Engineering Terminology

Help authors and researchers choose Thai terms for industrial engineering (IE) that are defensible: backed by sources, consistent across a document, and honest about uncertainty. A wrong or invented "official" term in a textbook gets copied by students for years, so the goal is evidence first, recommendation second.

## Scope
Work across these areas (see `references/ie-topics.md` for sub-topic keywords to widen searches):
- วิจัยดำเนินงาน (Operations Research)
- การผลิต / โลจิสติกส์ / ซัพพลายเชน
- การควบคุมคุณภาพ / สถิติ
- การยศาสตร์ / ความปลอดภัย / การศึกษางาน

## Workflow

1. **Pin down the term list.** Take English terms from the user's request or attached text. If given a passage, extract candidate technical terms yourself and confirm only if the list is large or ambiguous. Note the context (book chapter, paper field), since the right Thai term sometimes depends on subfield (e.g. "stock" in finance vs. inventory).

2. **Search sources in tiers.** Go in this order and stop escalating once you have enough agreement, but always record what each tier said (see `references/sources.md` for sites and query patterns):
   - Tier 1 – ราชบัณฑิตยสภา: ระบบสืบค้นศัพท์บัญญัติ, พจนานุกรมศัพท์วิศวกรรมศาสตร์ และคลังศัพท์ที่เกี่ยวข้อง. These are the closest thing to official coined terms.
   - Tier 2 – Thai textbooks, theses, journals (ThaiJO, TDC, university course documents, publisher catalogs): shows how the field really writes.
   - Tier 3 – Standards and professional bodies (สมอ./มอก., สภาวิศวกร, วสท., สมาคมวิชาชีพด้านอุตสาหการ/คุณภาพ, Thai ISO translations).
   - Tier 4 – General web (blogs, company pages, news): use only to show usage frequency, never as the sole basis.
   Run searches for independent terms in parallel. Search with both the English term and the candidate Thai term (e.g. `"queueing theory" ทฤษฎีแถวคอย`), because Thai variants only surface when you look for them.

3. **Compare candidates.** For each term collect every Thai variant seen, where it was seen, and whether it is a coined term (ศัพท์บัญญัติ), a transliteration (ทับศัพท์), or common usage. Different sources really do disagree (e.g. แถวคอย / การเข้าแถวคอย / คิว), so do not hide that.

4. **Recommend, with a reason.** Pick one term per entry using this priority: ราชบัณฑิตยสภา coined term → term most used in Thai IE textbooks/standards → clear transliteration. Say why in a few words. If the official term is rarely used in practice, say so and give both, since the author may reasonably prefer the one students recognise. Put the English in parentheses at first use in the document, which is standard Thai academic practice.

5. **Report in chat as a short table** (default; the user chose this format):

   | English | คำที่แนะนำ | ตัวเลือกอื่นที่พบ | ประเภท | แหล่งอ้างอิง / ระดับความมั่นใจ |
   |---|---|---|---|---|

   Keep the "เหตุผล/หมายเหตุ" to one short line per row (put it in the last column if needed). After the table, give a "Sources:" list with working links. Then ask once whether the user wants the results saved as a file (Excel/Sheet) or added to a running glossary for the project.

## Honesty rules (why they matter)
- Never present a term as ราชบัณฑิตยสภา-approved unless you actually saw it in a Tier 1 source this session. Memory of "I think it's official" is not evidence; label such terms "ยังไม่ยืนยันกับแหล่งทางการ".
- Use confidence labels: **สูง** (Tier 1 or ≥2 independent Tier 2/3 sources agree), **กลาง** (one good source or usage-only), **ต่ำ** (only general web or your own translation). If you had to coin a translation yourself, say so plainly and mark it ต่ำ.
- If a site cannot be fetched, say that rather than reconstructing its content. Do not work around blocked pages. The ราชบัณฑิตยสภา site is often unreachable from the search environment; when that happens, state it once at the top, mark every term as not confirmed against Tier 1, and invite the user to paste the result from the Royal Society coined-terms search (or a screenshot/PDF page) so you can upgrade the confidence.
- Separate what you found from what you recalled. A term you remember but could not find in any source this session (for example a "natural-sounding" Thai translation) goes in its own note labelled "นึกได้แต่ค้นไม่พบ", never in the recommended column as if it were established. Searching showed that such recalled translations can simply not exist in Thai literature.
- For terms with no Thai equivalent found, recommend ทับศัพท์ following ราชบัณฑิตยสภา's transliteration rules, and note it.

## Consistency across a long document
When the user is drafting multiple chapters, keep a running glossary in the conversation (or in a file if they ask) and reuse prior decisions instead of re-deciding. Flag any place where the same English term has been given two Thai terms, and point out near-synonym traps (e.g. variance/ความแปรปรวน vs. variation/การแปรผัน, reliability vs. availability, tolerance, capacity vs. capability) where a wrong choice changes meaning.

## Edge cases
- Abbreviations and eponyms (EOQ, MRP, Pareto, Gantt, Kanban): usually keep the original form; give the Thai explanation term once.
- Terms drawn from Japanese lean vocabulary (kaizen, poka-yoke, muda): note the Thai ทับศัพท์ habit and any translated variants.
- Very new terms (Industry 4.0, digital twin, ESG-related): expect weak Tier 1 coverage; lean on Tier 2–3 and say that.
- If the user wants definitions too, add a one-line Thai definition and cite where it came from; do not invent definitions.
