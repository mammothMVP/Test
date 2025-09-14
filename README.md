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