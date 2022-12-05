# Инструмент анализа статистики продаж
## Простая версия сервиса, который поможет рассчитать выручку в определенный период.
### С помощью метода max можно определить максимальную выручку за указанный период.
### public class SalesManager {
    protected int[] sales;

    public SalesManager(int[] sales) {
        this.sales = sales;
    }

    public int max() {
        int max = -1;
        for (int sale : sales) {
            if (sale > max) {
                max = sale;
            }
        }
        return max;
    }
}
