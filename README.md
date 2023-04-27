# AttendanceMonitoring
import java.util.*;

public class AttendanceMonitoringSystem {
   public static void main(String[] args) {
      // Create a list of students
      List<String> students = new ArrayList<>();
      students.add("John");
      students.add("Jane");
      students.add("Peter");
      students.add("Mary");
      
      // Create a map to store attendance status for each student
      Map<String, Boolean> attendance = new HashMap<>();
      
      // Initialize all attendance statuses to false
      for (String student : students) {
         attendance.put(student, false);
      }
      
      // Simulate attendance marking
      attendance.put("John", true);
      attendance.put("Mary", true);
      
      // Print attendance report
      System.out.println("Attendance Report:");
      for (String student : students) {
         String status = attendance.get(student) ? "Present" : "Absent";
         System.out.println(student + ": " + status);
      }
   }
}
