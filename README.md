public class DayOfWeek{
public enum Day{
SUNDAY, MONDAY, TUESDAY, WEDNESDAY,
THURSDAY, FRIDAY, SATURDAY
}
Day day;
public DayOfWeek(Day day) {
this.day = day;
System.out.println(day);
}
public boolean isWorkday(){
if ((day == Day.MONDAY)||(Day.TUESDAY==day)||(day==Day.WEDNESDAY) ||
(day==Day.THURSDAY) || (day==Day.FRIDAY))
return true;
else
return false;
}
public static void main(String[] args) {
DayOfWeek firstDay = new DayOfWeek(Day.FRIDAY);
boolean a =firstDay.isWorkday();
System.out.println("returned value is "+ a);
DayOfWeek sixthDay = new DayOfWeek(Day.SUNDAY);
boolean b=sixthDay.isWorkday();
System.out.println("returned value is "+ b);
}
}
