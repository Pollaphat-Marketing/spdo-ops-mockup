# SPDO Ops — Interactive Prototype

Clickable UI prototype for a **last-mile delivery operations & billing system** — a proposed replacement for a monthly Excel workbook used by a parcel-delivery sub-contractor (Shopee SPX / Lazada LEX).

> ตัวอย่างหน้าจอระบบ (mockup) สำหรับนำเสนอ — ข้อมูลในไฟล์เป็น **ตัวอย่างที่ผ่านการ anonymize แล้ว** (ชื่อคนรถถูกแทนด้วยรหัส, ไม่มีข้อมูลส่วนบุคคลจริง)

## Screens

| Screen | Description |
|---|---|
| แดชบอร์ด | ภาพรวมรายรับ–ต้นทุน–กำไร ต่อ Hub + แจ้งเตือนความผิดปกติ |
| ใบคุมเที่ยว | สรุปยอดทุกคนอัตโนมัติ (แทนชีตสรุปเดิม) |
| บันทึกรายวัน | กรอกงานรายวัน + คิดเงิน SPX/SPDO เรียลไทม์ + ฟอร์มบน LINE |
| กระทบยอด | เทียบยอดที่ระบบคิด vs เงินที่แพลตฟอร์มโอนจริง (Settlement) |
| ใบจ่ายคนรถ | สลิปจ่ายต่อคนต่อรอบบิล ส่งเข้า LINE |

## Run locally

It's a single static file — just open it:

```bash
open index.html
```

## Deploy

Static site, no build step. On Vercel: import the repo, framework preset **Other**, output = repo root. `index.html` is served at `/`.

Navigate between screens via the left sidebar, or by URL hash: `#dash`, `#summary`, `#entry`, `#reco`, `#slip`.
