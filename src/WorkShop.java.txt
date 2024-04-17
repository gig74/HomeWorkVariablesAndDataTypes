import java.util.Arrays;

public class WorkShop {
    public static void main(String[] args) {
        Friend[] myFriends = {
                new Friend("Вася", Integer.parseInt("26"),false,2.4f),
                new Friend("Лиза", Integer.parseInt("23"),true,2.7f),
                new Friend("Петя", Integer.parseInt("24"),true,4.3f),
                new Friend("Оля", Integer.parseInt("24"),true,0.1f),
                new Friend("Саша", Integer.parseInt("27"),false,20.6f)
        };
        System.out.println(Arrays.toString(myFriends));
    }
}
class Friend {
    String name;
    int age;
    boolean isFriendFromSchool;
    float hoursSpentTogetherLastWeek;
    public Friend(String name, int age, boolean isFriendFromSchool, float hoursSpentTogetherLastWeek) {
        this.name = name;
        this.age = age;
        this.isFriendFromSchool = isFriendFromSchool;
        this.hoursSpentTogetherLastWeek = hoursSpentTogetherLastWeek;
    }

    @Override
    public String toString() {
        return "\n Friend{" +
                "name='" + name + '\'' +
                ", age=" + age +
                ", isFriendFromSchool=" + isFriendFromSchool +
                ", hoursSpentTogetherLastWeek=" + hoursSpentTogetherLastWeek +
                '}';
    }
}