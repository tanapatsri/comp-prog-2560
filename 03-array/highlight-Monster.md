โจทย์ปัญหาเรื่อง Highlight Monster

    ไคบะ เซโตะ กำลังจัดงานแข่งขัน Kaiba Corporation Cup 2018 ในการแข่งขันนี้ไคบะต้องการให้ในระหว่าง
การแข่งขันมีการแสดง Highlight Monster ในสนามของผู้เข้าแข่งขันแต่ละฝั่ง จึงได้จ้างให้เขียนโปรแกรมนี้ขึ้น
Input
	-จำนวนมอนสเตอร์ของผู้เข้าแข่งขันฝั่ง RED และ ฝั่ง BLUE
	-ชื่อของมอนสเตอร์
	-ระดับดาว
	-ค่า ATK / DEF
Process
	การเลือก Highlight Monster มีสูตรดังนี้
	มอนสเตอร์ที่ ATK>=DEF
		Highlight Monster = (ระดับดาว*10)^2 + (ATK*1.75) + (DEF*1.25)
	มอนสเตอร์ที่ DEF>ATK
		Highlight Monster = (ระดับดาว*10)^2 + (ATK*1.25) + (DEF*1.75)
Output
	แสดงชื่อของ Highlight Monster ระดับดาว ATK / DEF ของแต่ละฝั่ง
*หมายเหตุ หากมีมอนสเตอร์ที่มีค่า Highlight Monster เท่ากันก็จะแสดงออกมาทั้งสองตัว กำหนดให้รับค่าตัวอักษร
ในชื่อได้ 30 ตัวอักษรต่อ 1 ชื่อ สมมุติว่าการinputเป็นค่าตามที่ โดยที่ มอนสเตอร์บนสนามต้องมี 1-5 ตัวชื่อรับได้ 
30 ตัวอักษร ระดับดาว (1-12)ATK (0-9999) DEF (0-9999)

ตัวอย่าง Input Output
Ex 1.
*****Welcome to KAIBA CORPORATION  CUP 2018*****
Contestants RED
The monsters on the field ?(1-5): 3
Name Monsters: DarkHorus
Monsters Level (1-12): 8
ATK (0-9999): 3000
DEF (0-9999): 1800
Name Monsters: TyrantDragon
Monsters Level (1-12): 8
ATK (0-9999): 2900
DEF (0-9999): 2500
Name Monsters: FelgrandDragon
Monsters Level (1-12): 8
ATK (0-9999): 2800
DEF (0-9999): 2800
Contestants BLUE
The monsters on the field ?(1-5): 2
Name Monsters: SilentMagicianLv8
Monsters Level (1-12): 8
ATK (0-9999): 3500
DEF (0-9999): 1000
Name Monsters: DarkPaladin
Monsters Level (1-12): 8
ATK (0-9999): 2900
DEF (0-9999): 2400
Contestants RED Highlight Monster is FelgrandDragon Level 8 ATK 2800 / DEF 2800
Contestants BLUE Highlight Monster is DarkPaladin Level 8 ATK 2900 / DEF 2400