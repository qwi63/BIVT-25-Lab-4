namespace Lab4
{
    public class White
    {
        public double Task1(int[] vector)
        {
            double length = 0;


            // code here
            if (vector == null || vector.Length == 0)
                return 0;

            double sumOfSquares = 0;

            for (int i = 0; i < vector.Length; i++)
            {
                sumOfSquares += vector[i] * vector[i];
            }

            length = Math.Sqrt(sumOfSquares);
            // end

            return length;
        }
        public int Task2(int[] array, int P, int Q)
        {
            int count = 0;

            // code here

            for (int i = 0; i < array.Length; i++)
            {

                if (P < array[i] && array[i] < Q)
                {
                    count++;
                }

            }
            // end

            return count;
        }
        public void Task3(int[] array)
        {

            // code here
            if (array == null || array.Length < 2)
                return;


            int maxIndex = 0;
            for (int i = 1; i < array.Length; i++)
            {
                if (array[i] > array[maxIndex])
                {
                    maxIndex = i;
                }
            }


            if (maxIndex >= array.Length - 1)
                return;


            int minAfterMaxIndex = maxIndex + 1;
            for (int i = maxIndex + 2; i < array.Length; i++)
            {
                if (array[i] < array[minAfterMaxIndex])
                {
                    minAfterMaxIndex = i;
                }
            }


            if (array[minAfterMaxIndex] < array[maxIndex])
            {

                int temp = array[maxIndex];
                array[maxIndex] = array[minAfterMaxIndex];
                array[minAfterMaxIndex] = temp;
            }
            // end

        }
        public void Task4(int[] array)
        {

            // code here
            int n = array.Length;
            int maxi = 0;
            for (int i = 0; i < n; i += 2)
            {
                if (array[i] > array[maxi])
                {
                    maxi = i;

                }
            }
            array[maxi] = maxi;

            // end

        }
        public int Task5(int[] array, int P)
        {
            int index = 0;

            // code here
            int n = array.Length;
            for (int i = 0; i < n; i++)
            {
                if (array[i] == P)
                {
                    index = i;
                    return index;
                }
            }
            return -1;
            // end

            return index;
        }
        public void Task6(int[] array)
        {

            // code here

            if (array == null || array.Length < 2)
                return;


            int maxIndex = 0;
            for (int i = 1; i < array.Length; i++)
            {
                if (array[i] > array[maxIndex])
                {
                    maxIndex = i;
                }
            }


            if (maxIndex <= 1)
                return;


            for (int i = 0; i < maxIndex - 1; i += 2)
            {

                int temp = array[i];
                array[i] = array[i + 1];
                array[i + 1] = temp;
            }
        }
        // end


        public int[] Task7(int[] array)
        {
            int[] answer = null;

            // code here
            if (array == null || array.Length == 0)
            {
                return array;
            }

            int count = 0;
            for (int i = 0; i < array.Length; i++)
            {
                if (array[i] >= 0)
                {
                    count++;
                }
            }

            if (count == array.Length)
            {
                answer = new int[array.Length];
                for (int i = 0; i < array.Length; i++)
                {
                    answer[i] = array[i];
                }
                return answer;
            }

            if (count == 0)
            {
                return new int[0];
            }

            answer = new int[count];
            int index = 0;
            for (int i = 0; i < array.Length; i++)
            {
                if (array[i] >= 0)
                {
                    answer[index] = array[i];
                    index++;
                }
            }

           
        
            
            return answer;
        }
        // end



        public int[] Task8(int[] array)
        {

            // code here
            if (array == null || array.Length < 2)
                return array;

            int n = array.Length;
            for (int i = 0; i < n - 1; i++)
            {
                for (int j = 0; j < n - i - 1; j++)
                {
                    if (array[j] < array[j + 1])
                    {

                        int temp = array[j];
                        array[j] = array[j + 1];
                        array[j + 1] = temp;
                    }
                }
            }


            return array;
            // end

        }
        public int[] Task9(int[] array)
        {

            // code here
            int temp, n = array.Length;
            for (int i = 0; i < n / 2; i++)
            {
                temp = array[i];
                array[i] = array[n - 1 - i];
                array[n - 1 - i] = temp;
            }
            return array;

            // end

        }
        public int[] Task10(int[] A, int[] B)
        {
            int[] C = null;

            // code here
            if (A == null && B == null)
            {
                C = new int[0];
                return C;
            }

            if (A == null || A.Length == 0)
            {
                C = B != null ? (int[])B.Clone() : new int[0];
                return C;
            }

            if (B == null || B.Length == 0)
            {
                C = (int[])A.Clone();
                return C;
            }

            int totalLength = A.Length + B.Length;
            C = new int[totalLength];

            int indexA = 0;
            int indexB = 0;
            int indexC = 0;

            while (indexA < A.Length && indexB < B.Length)
            {
                C[indexC++] = A[indexA++];
                C[indexC++] = B[indexB++];
            }

            while (indexA < A.Length)
            {
                C[indexC++] = A[indexA++];
            }

            while (indexB < B.Length)
            {
                C[indexC++] = B[indexB++];
            }
            // end

            return C;
        }
        public double[] Task11(double a, double b, int n)
        {
            double[] array = null;

            // code here
            if (n <= 0)
                return null;

            if (n == 1)
            {
                if (a == b)
                {
                    array = new double[] { a };
                    return array;
                }
                return null;
            }

            array = new double[n];

            if (a < b)
            {
                double step = (b - a) / (n - 1);
                for (int i = 0; i < n; i++)
                {
                    array[i] = a + i * step;
                }
            }
            else if (a > b)
            {
                double step = (a - b) / (n - 1);
                for (int i = 0; i < n; i++)
                {
                    array[i] = a - i * step;
                }
            }
            else
            {
                return null;
            }
            // end

            return array;
        }

        public double[] Task12(double[] raw)
        {
            double[] restored = null;

            // code here
            if (raw.Length < 3)
            {
                return null;
            }

            else
            {
                bool allMinusOne = true;
                for (int i = 0; i < raw.Length; i++)
                {
                    if (raw[i] != -1)
                    {
                        allMinusOne = false;
                        break;
                    }
                }

                if (allMinusOne)
                {
                    restored = new double[raw.Length];
                    for (int i = 0; i < raw.Length; i++)
                    {
                        restored[i] = -1;
                    }
                    return restored;
                }

                restored = new double[raw.Length];
                for (int i = 0; i < raw.Length; i++)
                {
                    restored[i] = raw[i];
                }

                for (int i = 0; i < raw.Length; i++)
                {
                    if (raw[i] == -1)
                    {
                        double leftNeighbor;
                        if (i == 0)
                        {
                            leftNeighbor = raw[raw.Length - 1];
                        }
                        else
                        {
                            leftNeighbor = raw[i - 1];
                        }

                        double rightNeighbor;
                        if (i == raw.Length - 1)
                        {
                            rightNeighbor = raw[0];
                        }
                        else
                        {
                            rightNeighbor = raw[i + 1];
                        }

                        if (leftNeighbor != -1 && rightNeighbor != -1)
                        {
                            restored[i] = (leftNeighbor + rightNeighbor) / 2;
                        }

                    }
                }
            }

            // end

            return restored;
        }
    }

}
