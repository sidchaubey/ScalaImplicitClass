# ScalaImplicitClass

Quick Reference on how we create and use Implicit class in Scala. Using Implicit Class we can directly utilise function similar to in-build function without the need to download the whole code base and do the correspomding changes in that downloaded code.

Eg: 
object ImplicitDemo{
  implicit class getSubstring(str: String){
    def getThreeChar(): String = {
      return str.substring(0,3)
     }
   }
  
  def main(args: Array[String]): Unit{
    var text = "Hello Man How are you !!"
    println(text.getThreeChar())
  }
}
