# Call in order
Suppose we have the following code:
public class Foo{
  public Foo(){ ... }
  public void first() { ... }
  public void second() { ... }
  public void third() { ... }
}
The same instance of Foo will be passed to three different threads. ThreadA will call first, threadB will call second, and threadC vill call third. Design a mechanism to ensure that first is called before second and second is called before third.

## sources
  - CTCI 15.5 pg. 180
