* 方法は2通りある。
* 方法A. Eclipse のプラグインである m2e を使ってプロジェクトを作る方法。
    * http://javazuki.doorblog.jp/articles/apache/maven/maven-module.html
    * Eclipse; New; Maven Project で親プロジェクト(packaging pom)を作る。
    * Eclipse; New; Maven Module でモジュール(packaging jarなど)を作る。
* 方法B. Maven の Eclipse 対応プラグインである maven-eclipse-plugin を使って Eclipse にインポートする。
    * http://tnaka0128.blogspot.jp/2013/05/maven.html
    * pom.xml を eclipse 以外の方法でセッティングしたあと、 mvn eclipse:eclipse コマンドを実行すると eclipse 用の .project, .classpath ファイルが生成される。
    * この方法では親プロジェクトの .project は生成されない。よってインポートできない。
* Maven基礎
    * http://www.slideshare.net/taktos/maven-28516988
    * p.38 Eclipse maven-eclipse-plugin は Maven の Eclipse 対応プラグイン。 dependency の scope を解釈できないのでお勧めしない。
* Eclipse だけを使うのであれば、方法Aがよさそうだ。


