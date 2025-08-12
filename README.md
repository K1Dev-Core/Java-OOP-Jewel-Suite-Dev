
<div align="center">
  <h3>ระบบจำลองการกระจายตัวของแก๊ส</h3>
</div>

## 🚀 การติดตั้งและรัน

## 💻 การใช้งานใน IntelliJ IDEA

1. เปิดโปรเจคใน IntelliJ IDEA
2. **คลิกขวา** ที่โฟลเดอร์ `lib` ใน Project Explorer
3. เลือก **"Add as Library..."**
4. กด **OK** เพื่อเพิ่ม library เข้าโปรเจค
5. รัน `Main.java` ได้เลย!


## 👥 ทีมพัฒนา

**C++ TEAM**
- **วชิรวิทย์ วงค์แสง** (67011212055) - Project Manager
- **ชินดนัย ภูหัดสวน** (67011212026) - Lead Developer  
- **นางสาวเศรณี ภูนาโพธิ์** (67011212143) - UI/UX Designer






# Note🧠 

## FileData.java
**จัดการค่าจากไฟล์** 

**เมธอดทั้งหมด :**
- `public boolean readFile(String path)`  
  •: อ่านค่าจากไฟล์  
- `public double getBottom(int r, int c)`  
  •: ดึงค่า Base Horizon 
- `public double getTop(int r, int c)`  
  •: ดึงค่า  Top Horizon
- `public double getVolume(int r, int c)`  
  •: ดึงค่า ปริมาตรแก้ส
- `public double getPercent(int r, int c)`  
  •: ดึงค่า เปอเชนแก้ส
- `public int getLevel(int r, int c)`  
  •: ดึงค่า ระดับแก้ส
- `public double getTotalVolume(ไม่มี)`  
  •: ดึงค่า แก้สทั้งหมด 
- `public void setFluid(double level)`  
  •: เช็ตค่า Fluid
- `public double getFluid(ไม่มี)`  
  •: ดึงค่า Fluid 
- `public int getRows(ไม่มี)`  
  •: ดึงค่า แถว 
- `public int getCols(ไม่มี)`  
  •: ดึงค่า คอลัม 
- `public void clear(ไม่มี)`  
  •: เคลียร์ค่า
- `public boolean loadFromFile(String path)`  
  •: โหลด่าจากไฟล์
- `public boolean isValidNumber(String str)`  
  •: เช็คว่าตัวเลขไหม ป้้องกันบัค
- `public int countZeroCells(ไม่มี)`  
  •: เช็คจำนวน ช่องที่ไม่มีแก้สเลย


## FileUploader.java
**ทำหน้าอัพโหลดไฟล์** 
- เลย์เอาต์: BoxLayout

**เมธอดทั้งหมด**
- `private boolean isCurrentThemeDark(ไม่มี)`  
  •: เช็คว่าใช้ธีมอะไรอยู่เพื่อไปปรับสีข้อความหรือสีนั้นนี่ได้ให้มันตัดกัน
- `public void refresh(ไม่มี)`  
  •: รีเฟชค่า
- `private void updateTextColors(ไม่มี)`  
  •: อัพเดทสีข้อความนั้นนี่


## GridDisplay.java
**ตารางแสดงแก้ส**

**เมธอดทั้งหมด**
- `private boolean isCurrentThemeDark(ไม่มี)`  
  •: เช็คว่าใช้ธีมอะไรอยู่เพื่อไปปรับสีข้อความหรือสีนั้นนี่ได้ให้มันตัดกัน
- `private void makeBorder(ไม่มี)`  
  •: สร้างเส้นขอบ
- `private void makeGrid(ไม่มี)`  
  •: สร้าพาแนลไว้ใส่แก้สนั้นแหละ
- `private void calcCellSize(ไม่มี)`  
  •: คำนวณขนาดช่อง เพื่อป้องกันไม่ให้มันใหญ่ หากมีจำนวนเยอะ
- `private void makeCells(ไม่มี)`  
  •: สร้างช่องตารางแก้ส
- `private JPanel addNumbers(JPanel mainGrid, int rows, int cols)`  
  •: สร้างเลขแสดงตามแถวคอลัม แบบให้มันดูง่าย เลขกำกับ
- `private JPanel makeCell(int r, int c)`  
  •: สร้าวงช่องแก้สในแต่ละช่อง
- `public void handleMouseIn(int r, int c, JPanel cell)`  
  •: เช็คเมือเมาส์ hover ช่องแก้ส
- `public void handleMouseOut(int r, int c, JPanel cell)`  
  •: เช็คเมือเมาส์ออกจาก ช่องแก้ส
- `public void setInfoLabel(JLabel lbl)`  
  •: เช็ตค่าแสดงรายละเอียดแก้ส
- `private void clearHover(ไม่มี)`  
  •: เคลียร์ข้อความเมื่อเอาเมาส์ออก
- `private void showInfo(int r, int c)`  
  •: แสดงค่ารายละเอียดแก้ส ด้านล่าง
- `private Color getColor(int r, int c)`  
  •: ดึงค่า สี
- `private String makeInfo(int r, int c)`  
  •: สร้างส่วนรายละเอียดแก้ส
- `private boolean isColorDark(Color color)`  
  •: เช็คว่าอยู่ธีมมืดไหม เพื่อปรับสีข้อความให้ตัดสีกัน
- `public void refresh(ไม่มี)`  
  •: รีเฟชค่า

- เลย์เอาต์: BorderLayout, GridLayout


## Main.java
**ไว้รันโปรแกรมเฉยๆ**

## Settings.java
**ไว้เก็บตัวแปรต่างๆพวกตั้งค่านั้นนี่** 


## SummaryView.java
**สรุปข้อมูลหลังจากคำนวณแล้ว**


- `private void createSummaryWindow(ไม่มี)`  
  •: สร้างหน้าสรุป
- `private double calculateTotalVolume(ไม่มี)`  
  •: คำนวณค่าแก้สทั้งหมด
- `private int calculateTotalActiveCells(ไม่มี)`  
  •: คำนวณแก้ทั้งหมดที่มีในช่อง
- `private JPanel createSummaryCards(int totalActiveCells, double totalVolume)`  
  •: สร้างช่องแสดงแก้สทสรุป
- `private JPanel createDetailTable(ไม่มี)`  
  •: สร้างงรายละเอียดแก้ส
- `private JPanel createButtonPanel(ไม่มี)`  
  •: ทำปุ่ม

- `private JPanel createInfoCard(String labelText, String valueText)`  
  •: สร้างรายละเอียดของงแก้สในแต่ะช่อง


- `private void createTableDataRow(JPanel table, GridBagConstraints constraints, int rowNumber, Color gasColor, String gasTypeName, int cellCount, double volume)`  
  •: ไว้สร้างหลอดสำหรับแสดงข้อมูลแบบแถว
- `private JLabel createDataLabel(String text)`  
  •: รายละเอียดของข้อมูลตามแถว
- `private JPanel createColorIndicator(Color color)`  
  •: แก้ไขพวกสีข้อความให้ไม่ตัดกับสีธีม
- `private JProgressBar createPercentageBar(int percentage, Color color)`  
  •: หลอดโหลดแถบโหลดแสดงข้อมูลแก้ส JProgressBar



## Actions.java
**รวมการแอ้คชั่นปุ่มทุกอย่าง:** 
- **มี** `Actions`, `AboutAction`, `CalculateAction`, `ClearAction`, `ExitAction`, `LoadAction`, `SummaryAction`, `ThemeAction`, `CellMouseAction`, `ClickLoadAction`



## App.java
**คลาสหลักรวมโครงสร้างต่างๆ:** 

- `private void setup(ไม่มี)`  
  •: เช็ตอัพโครวสร้าง
- `private void theme(ไม่มี)`  
  •: เช็ตธีม โหลดค่าจากdb มาเช็คด้วย
- `private void setLaf(String name)`  
  •: ใช้lib เช็ตธีม
- `private void repaintAll(ไม่มี)`  
  •: สร้างโครงงสร้างคอมโพเนนใหม่ทั้งหมด ไว้ใช้ตอนอัพเดทธีมหรอือื่นๆ
- `private void window(ไม่มี)`  
  •: เช็ตค่าพวก frame หลัก
- `private void ui(ไม่มี)`  
  •: จัดการพวก ui หลักคอมมโพเนนต่างๆ
- `private void top(JPanel p)`  
  •: ส่วนข้างบนเช่นโลโก้ หรือเมนู  -พาแนล
- `private void middle(JPanel p)`  
  •: ส่วนกลาง -พาแนล
- `private void left(JPanel p)`  
  •: ส่วนข้างซ้าย  -พาแนล
- `private JPanel inputPanel(ไม่มี)`  
  •: ส่วนช่องใส่ค่า
- `private JPanel colorPanel(ไม่มี)`  
  •: ส่วนพวกแสดงระดับแก้ส พวกชองสี
- `private JPanel createColorItem(String txt, Color c)`  
  •: สร้างช่องสี
- `private JLabel getColorItemLabel(JPanel colorItem)`  
  •: สร้างแสดงข้อความสีกำกับสี
- `private JPanel resultPanel(ไม่มี)`  
  •: แสดงผลลัพพวกแจ้งเตือนนนั้

- `private void right(JPanel p)`  
  •: ส่วนข้างขวา  -พาแนล
- `public boolean hasData(ไม่มี)`  
  •: เช็คว่ามีข้อมูลจากไฟล์หรือยัง 
- `public void loadFile(ไม่มี)`  
  •: อัพโหลดไฟล์
- `public void calculate(ไม่มี)`  
  •: คำนวณค่าจากไฟล์
- `public void clearData(ไม่มี)`  
  •: เคลียร์ค่า
- `private void updateBtns(ไม่มี)`  
  •: อัพเดทปุ่ม เช่น ปุ่มโหลด หรือจะให้แสดงปุ่มเคลียร์ และอื่นๆ 
- `private void update(ไม่มี)`  
  •: จัดการอัพเดทต่างๆเมือ่มีการอัพเดทค่า หรือคำนวณใหม่
- `private void showStats(ไม่มี)`  
  •: โชว์แสดงข้อมูลแก้ส
- `public void exitApp(ไม่มี)`  
  •: ปิด-ออกโปรแกรม
- `private void icon(ไม่มี)`  
  •: ไอคอน ของงโปรแกรม
- `private JLabel getIcon(ไม่มี)`  
  •: ไอคอนแสดงบนซ้ายโปรแกรม
- `public void changeTheme(JButton btn)`  
  •: เปลี่ยนธีม

- `private void updateTextColorsForDarkTheme(ไม่มี)`  
  •: เช็ตอัพเดทสี ไม่ให้ทืบเมื่อใช้ธีมมืด
- `private void updateTextColorsForLightTheme(ไม่มี)`  
  •: เช็ตอัพเดทสี เมื่อใช้ธีมสว่าง
- `private void showLoadingScreen(ไม่มี)`  
  •: หน้าโหลดโปรแกรม
- `private void saveSettings(String theme)`  
  •: บันทึกค่าลง db
- `private String[] loadSettings(ไม่มี)`  
  •: โหลดค่าจาก db
- `private void saveDB(ไม่มี)`  
  •: บันทึกค่าลง db
- `public void showSummary(ไม่มี)`  
  •: เมื่อกดปุ่มสรุป

-: BorderLayout, FlowLayout, JButton, JDialog, JFileChooser, JFrame, JLabel, JOptionPane, JPanel, JScrollPane, JTextField
- เลย์เอาต์: BorderLayout, BoxLayout, FlowLayout


## Display.java
**แสดง about และแจ้งงเตือนต่างๆ**


- JDialog,JOptionPane, JPanel

---
