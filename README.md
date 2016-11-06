# ใบงานที่ 1 เรื่อง การเขียนโปรแกรม Win32 ด้วยภาษา C

#include <windows.h>

int WINAPI
WinMain(HINSTANCE hInst, HINSTANCE hPrev, LPSTR  lpCmdLine, int nCmdshow)
{
    MessageBox(NULL, "Hello World! This is my first win32 program!",
	"Lesson1", MB_OK);
    return 0;
}
```
## บันทึกผลการทดลอง

  จากการทดลองเมื่อเขียนโปรแกรมเสร็จและทำการรันจะได้กล่องข้อความตอบสนองดังรูปภาพโดยเมื่อกดปุ่ม OK จะทำกล่องข้อความตอบสนองหายไป
  
  
  <img src="https://github.com/est160/LAB-01/blob/master/imgs/1.png?raw=true">

## คำถาม 
1. นักศึกษาพบปัญหาในการคอมไพล์โปรแกรมหรือไม่ ถ้าเจอให้บอกที่ผิดและแนวทางการแก้ไข

   ไม่พบปัญหาในการคอมไพล์
   
2. ให้ทดลองแก้ไข <code> MessageBox(...) </code> โดยการเปลี่ยน <code> MB_OK </code> เป็นค่าอื่นๆ [ดูได้จากอ้างอิงตามลิงค์นี้](https://github.com/Desktop-Programming-Lab-2559/LAB-01/blob/master/message-box.md)


MessageBox(NULL, "Hello World! This is my first win32 program!",
		 "Lesson1", MB_ABORTRETRYIGNORE);
		 
  		
   <img src="https://github.com/est160/LAB-01/blob/master/imgs/2.png?raw=true">


MessageBox(NULL, "Hello World! This is my first win32 program!",
		"Lesson1", MB_CANCELTRYCONTINUE);
		
		
    <img src="https://github.com/est160/LAB-01/blob/master/imgs/3.png?raw=true">
    
    
MessageBox(NULL, "Hello World! This is my first win32 program!",
		"Lesson1", MB_RETRYCANCEL);
		
		
    <img src="https://github.com/est160/LAB-01/blob/master/imgs/4.png?raw=true">
   

MessageBox(NULL, "Hello World! This is my first win32 program!",
		"Lesson1", MB_ICONWARNING);
		
		
    <img src="https://github.com/est160/LAB-01/blob/master/imgs/5.png?raw=true">
