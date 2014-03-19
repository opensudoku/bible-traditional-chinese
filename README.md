bible-traditional-chinese
=========================

Application developer can use this API to get any verse from Traditional Chinese Bible, source from http://a2z.fhl.net/CBOL.html  API self contains entire Bible, no need to link remotely or access any database.

Sample:
<pre>
import com.opensuodku.bible.tw.Bible;
public class Demo1 {

    public static void main(String[] args) {
        Bible bible = new Bible();

        for (int style = 0; style <=3; style++) {
            System.out.println("\n ---------- style=" + style);

            System.out.println(bible.getVerse(1, 1, 1, style));
            System.out.println(bible.getVerse(1, 1, 2, style));
            System.out.println(bible.getVerse(1, 1, 3, style));
            System.out.println(bible.getVerse(66, 22, 1, style));
            System.out.println(bible.getVerse(66, 22, 2, style));
            System.out.println(bible.getVerse(66, 22, 3, style));
        }
    }
}
</pre>

Result:
<pre>
1:1 起初，　神創造天地。
1:2 地是空虛混沌，淵面黑暗；　神的靈運行在水面上。
1:3 　神說：「要有光」，就有了光。
22:1 天使又指示我在城內街道當中一道生命水的河，明亮如水晶，從　神和羔羊的寶座流出來。
22:2 在河這邊與那邊有生命樹，結十二樣（或譯：回）果子，每月都結果子；樹上的葉子乃為醫治萬民。
22:3 以後再沒有咒詛；在城裡有　神和羔羊的寶座；他的僕人都要事奉他，

 ---------- style=2
創 1:1 起初，　神創造天地。
創 1:2 地是空虛混沌，淵面黑暗；　神的靈運行在水面上。
創 1:3 　神說：「要有光」，就有了光。
啟 22:1 天使又指示我在城內街道當中一道生命水的河，明亮如水晶，從　神和羔羊的寶座流出來。
啟 22:2 在河這邊與那邊有生命樹，結十二樣（或譯：回）果子，每月都結果子；樹上的葉子乃為醫治萬民。
啟 22:3 以後再沒有咒詛；在城裡有　神和羔羊的寶座；他的僕人都要事奉他，

 ---------- style=3
(1)創 1:1 起初，　神創造天地。
(1)創 1:2 地是空虛混沌，淵面黑暗；　神的靈運行在水面上。
(1)創 1:3 　神說：「要有光」，就有了光。
(66)啟 22:1 天使又指示我在城內街道當中一道生命水的河，明亮如水晶，從　神和羔羊的寶座流出來。
(66)啟 22:2 在河這邊與那邊有生命樹，結十二樣（或譯：回）果子，每月都結果子；樹上的葉子乃為醫治萬民。
(66)啟 22:3 以後再沒有咒詛；在城裡有　神和羔羊的寶座；他的僕人都要事奉他，
</pre>
