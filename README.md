# JAVA042
public class Parent {
		private void method1(){
			System.out.println ("Parent's method1()");
			}
		public void method2() {
			System.out.println ("Parent's method2()");
			method1();
		}
static class Child extends Parent {  //if we make it static ?/
	public void method1() {
		System.out.println ("Child's method1()");
}
	public static void  main(String args[]) {
		Parent p = new Child();
		p.method2();
	}
}
}

***output***
Parent's method2()
Parent's method1()
