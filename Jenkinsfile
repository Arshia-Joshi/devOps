pipeline {
agent any
tools {
jdk &#39;JDK17&#39;
}
stages {
stage(&#39;Checkout Code&#39;) {
steps {
git branch: &#39;main&#39;,
url: &#39;https://github.com/&lt;your-username&gt;/&lt;your-repo-
name&gt;.git&#39;
}
}
stage(&#39;Compile Java&#39;) {
steps {

sh &#39;&#39;&#39;
javac src/HelloWorld.java
&#39;&#39;&#39;
}
}
stage(&#39;Run Program&#39;) {
steps {
sh &#39;&#39;&#39;
java -cp src HelloWorld
&#39;&#39;&#39;
}
}
}
}