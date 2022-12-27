public class TriangleN1 {
    public double a;
    public double b;
    public double c;
    public double p;
    public double halfPerimeter(double a, double b, double c){
        return (a + b + c) / 2;
    }
    public double sqrtPart(double a, double b, double c){
        p = halfPerimeter(a, b,c);
        return Math.sqrt(p * (p - a) * (p - b) * (p - c));
    }
    public double heightA(){
        return (2 / a) * sqrtPart(a, b, c);
    }
    public double heightB(){
        return (2 / b) * sqrtPart(a, b, c);
    }
    public double heightC(){
        return (2 / c) * sqrtPart(a, b, c);
    }
}
