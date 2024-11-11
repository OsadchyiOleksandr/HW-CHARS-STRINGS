В проекті має бути реалізовано функціонал виправлення (корегування) слів, де це потрібно. Виведення має бути таким:

1) orange
2) plum
3) tomato
4) onion
5) grape

(1) Cтворіть проект Word-Corrector на локальній машині через IntelliJ IDEA (IDE).

(2) Структура проекту має бути такою:

(3) Функціонал класу DataProvider

package app;

public class DataProvider {

    public String[] getData() {
        return new String[]{"brange", "plum", "tomato", "onibn", "grape"};
    }
}


(4) Доопрацюйте функціонал класу Main

package app;

public class Main {

    public static void main(String[] args) {
        getOutput(Corrector().handleData(
                new DataProvider())
        );
    }

    private static void getOutput(String output) {
        System.out.println(output);
    }
}

5) Доопрацюйте функціонал класу Corrector

package app;

public class Corrector {

    public String handleData(String[] strs) {
        stringBuilder = new StringBuilder();
        int count = 0;
        for (String str : strs) {
            if (str.("b")) {
                str = str.replac("b", "o");
            }
            count;
            stringBuilder.append(count).append(") ").append(str).append("\\n");
        }
        return stringBuilder.toString();
    }
}

6) Залийте виконаний проект на свій GitHub репозиторій, посилання на який зазначте в LMS.