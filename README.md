# SeleniumAutomationScripts
package param;

import java.io.File;
import java.io.FileInputStream;
import java.io.FileNotFoundException;
import java.io.IOException;

import org.apache.poi.hssf.usermodel.HSSFWorkbook;
import org.apache.poi.ss.usermodel.Row;
import org.apache.poi.ss.usermodel.Sheet;

public class ClassParameter {

       public static void main(String[] args) {
              // TODO Auto-generated method stub
              //Connect to Excel Workbook
              File file =    new File("C:\\Users\\240963\\Desktop\\ExcelParam.xls");
              //Read the Content
              //Create an object of FileInputStream class to read excel file
           try {
                     FileInputStream inputStream = new FileInputStream(file);                 
                     HSSFWorkbook wkb1 = new HSSFWorkbook(inputStream);
                     //Read sheet inside the workbook by its name
                  Sheet sheet1 = wkb1.getSheet("Sheet1");
                 
                  int rowCount=0;
                  rowCount=sheet1.getLastRowNum()-sheet1.getFirstRowNum();
                  for (int i = 0; i < rowCount+1; i++) {

                      Row row = sheet1.getRow(i);
                    
                      //Create a loop to print cell values in a row

                      for (int j = 0; j < row.getLastCellNum(); j++) {

                          //Print Excel data in console

                          System.out.print(row.getCell(j).getStringCellValue()+"|| ");

                      }

                      System.out.println();
                  } 


              } catch (FileNotFoundException e) {
                     // TODO Auto-generated catch block
                     e.printStackTrace();
              }
           catch (IOException e) {
                     // TODO Auto-generated catch block
                     e.printStackTrace();
              }
       }

}
