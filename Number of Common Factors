class Solution {
    public int commonFactors(int a, int b) {
        int common_max = gcd(a, b), count = 0;

        for (int i = 1; i <= Math.sqrt(common_max); i++) {
            if (common_max % i == 0) {
                count++;
                if (i != common_max / i) {
                    count++;
                }
            }
        }

        return count;
    }

    private int gcd(int a, int b) {
        while (b != 0) {
            int temp = b;
            b = a % b;
            a = temp;
        }

        return a;
    }
}
