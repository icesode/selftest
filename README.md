//# selftest
package JavaClass.problem;

public class ExangeArray {
    public static void main(String[] args){
        int[] a={8,3,0,4,5,9,2,};//初始化数组
        int max=a[0];
        int min=a[0];
        int q=0;//用于记录最大值的数组元素下标
        int b=0;//用于记录最小值的数组元素下标
        for(int i=0;i<a.length;i++){
            if(a[i]>max){
                max=a[i];
                q=i;
            }
        }
        for(int i=0;i<a.length;i++){
            if(a[i]<min){
                min=a[i];
                b=i;
            }
        }
        a[q]=min;
        a[b]=max;
        for(int i=0;i<a.length;i++){
            System.out.print(a[i]);
        }
    }
}
