# polymorphism-1
sample
//polymorphism sample program 2
//its a dynamic binding from overriding
class overriding
{
	public void noise()
	{
	System.out.println("bike produce some noise");
	}
}
class moterbike extends overriding
{
	public void noise()
	{
		System.out.println("bike produce some noise, it distrub others");
	}
}
class test
{
	public static void main(String []args)
{
	overriding o=new overriding();
	o.noise();
	overriding o1=new moterbike(); //it shows how a parent class refers child class object
	o1.noise();
	moterbike m=new moterbike();// it gives oly child class object
	m.noise();
}
}
