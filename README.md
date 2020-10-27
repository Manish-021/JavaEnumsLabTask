# JavaEnumsLabTask
Sample Solution for the Java Enums Lab Task
import java.time.LocalDate;
import java.time.Month;

public class DaysLeft {
    public static void main(String[]args){
        LocalDate currentDate = LocalDate.now();
        int currentDay = currentDate.getDayOfMonth();
        Month currentMonth = currentDate.getMonth();
        Months month = Months.valueOf(currentMonth.name());
        switch (month) {
            case JANUARY:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case FEBRUARY:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case MARCH:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case APRIL:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case MAY:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case JUNE:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case JULY:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case AUGUST:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case SEPTEMBER:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case OCTOBER:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case NOVEMBER:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            case DECEMBER:
                System.out.println(month.getNumberOfDays() + " - " + currentDay + " = " +
                        (month.getNumberOfDays() - currentDay) + " Days left in " + month + "!");
                break;
            }
        }
    }

    enum Months{
        JANUARY(31),
        FEBRUARY(28),
        MARCH(31),
        APRIL(30),
        MAY(31),
        JUNE(30),
        JULY(31),
        AUGUST(31),
        SEPTEMBER(30),
        OCTOBER(31),
        NOVEMBER(30),
        DECEMBER(31);

        private final int numberOfDays;

        Months(int numberOfDays) {
            this.numberOfDays = numberOfDays;
        }

        public int getNumberOfDays() {
            return numberOfDays;
        }
    }
