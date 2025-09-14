ตั้งค่า Git ก่อนใช้งาน
ตั้งค่า ชื่อ อีเมล ที่ใช้งาน
git config --global user.name <name>
git config --global user.email <email>

Git Commits:บันทึกการเปลี่ยนเเลง
    Staged Changes ---> Writing Commint Massage ---> Commit
        -ตรวจสอบให้เเน่ใจทุกครั้งว่าไฟล์ที่ต้องการอยุ่บนStaged ที่ถูกต้อง
        -เขียน (Commit Message) ผ่าน Vscode Source Contral
        -Contentional Commits เเนวทางเขียน Commit ให้มีความหมาย
        - ทำการ commit บนvscode สามารถกดคียลัด ctrl + enter
        -หรือใช้คำสั่ง git commit -m <massege>

Git Remote: เชื่อมต่อกับ Git Provider
                Locak Repository
    Commit 1 ---> commit 2 ---> commit 3

        - เข้าสู่ระบบ GitHub จากนั้นสร้าง (Remote Repository)
        - ตั้งค่าการเชื่อมต่อระหว่าง (Local Repository) ไปยัง (Remote Repository)
        -โดยกำหนด(git URL) ผ่านฟันเฟือง
        -หรือคำสั่ง git remote add <name> <url>
        -ส่วนมาก <name> จะใช้เป็นชื่อorigin

Git Clone : clone repository ของคนอื่น 
    วิธีทำ คือ (window) cmd ตั้งcd เตรียมไฟล์ที่เราจะใส่ลงไป
    Ex. git clone https://github.com/nicknochnack/Llama2RAG
    repository ก็จะมาเเล้ว

Semantic Version:
    ง่ายๆ คือ ตัวอย่าง 3.12.5
        - มีการเปลี่ยนเเปลงครั้งใหญ่ 3 ครั้ง
        - มีการเพิ่มคุณสมบัติใหม่มาเเล้ว 12 ครั้ง
        - เวอร์ชั่น3.12 โดยเเก้ไขมาเเล้ว5ครั้ง
    หรือ ใช้คำสั่ง git tag <name>
    เราควร (push tag remote) เพื่อทำให้remote มีเเท็คเดียวกัน
    สามารถใช้คำสั่ง git push origin <tag> หรือ git push --tags
    เพื่อส่งtag ไปยังlocal remoteทั้งหมด
    **กรณีใช้gi

Git Branches: เเบ่งสาขาการพัฒนา
-เเบ่งสาขา เพื่อเเยกชุดโค๊ดตามปัจจัย
    -main หรือ master สาขาหลักเสถียรสุด
    -develop สาขาระหว่างพัฒนา ยังไม่พร้อมใช้จริง
    -feature/* สาขาปลีกย่อย
-สร้าง branch ใหม่ด้วยคำสั่ง git branch <name>
-สลับไปยัง branch (chechout) ด้วยคำสั่ง git checkout <name>

Git Merge : รวมสาขาการพัฒนา
    -เมื่อโค๊ดพร้อมใช้งาน รวมbranch(Merge) ด้วยคำสั่ง  git merge <branch>
    - ก่อนmerge ทุกครั้งต้องcheck outไปยังbranch หลักที่จะรวมของครอื่นก่อน
    ** มีโอกาสเกิด (Corflict)ได้ 