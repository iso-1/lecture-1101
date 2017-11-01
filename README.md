# テクノロジー（藤原） 11/1授業

```
iso1:~/workspace $ pry
[1] pry(main)> num = 2
=> 2
[2] pry(main)> num
=> 2
[3] pry(main)> if num % == 0
SyntaxError: unexpected ==
if num % == 0
           ^
[3] pry(main)> puts "偶数です"
偶数です
=> nil
[4] pry(main)> end
SyntaxError: unexpected keyword_end, expecting end-of-input
[4] pry(main)> num
=> 2
[5] pry(main)> puts "偶数です" if num %2 == 0
SyntaxError: (eval):2: unknown type of %string
puts "偶数です" if num %2 == 0
                              ^
[5] pry(main)> num = 1000
=> 1000
[6] pry(main)> if num >= 1500
[6] pry(main)*   puts "送料無料です。"  
[6] pry(main)* elsif 0 < num && num < 1500  
[6] pry(main)*   puts "送料300円です。"  
[6] pry(main)* else  
[6] pry(main)*   puts "入力が間違ってます。"  
[6] pry(main)* end  
送料300円です。
=> nil
[7] pry(main)> num = rand 3
=> 0
[8] pry(main)> case num
[8] pry(main)* when 0  
[8] pry(main)*   puts "吉です。"  
[8] pry(main)* when 1  
[8] pry(main)*   puts "凶です。"  
[8] pry(main)* else  
[8] pry(main)*   puts "大凶です。"  
[8] pry(main)* end  
吉です。
=> nil
[9] pry(main)> def triangle(b, h)
[9] pry(main)*   result = b * h / 2.0  
[9] pry(main)*   result  # 返り値は最後の1行  
[9] pry(main)* end  
=> :triangle
[10] pry(main)> 
[11] pry(main)> triangle(11, 9)  #=> 49.5
=> 49.5
[12] pry(main)> triangle 11, 9   # 括弧を省略した形
=> 49.5
[13] pry(main)> name = gets

=> "(適当な文字列を入力してEnter)\rname.chomp!\rname\n"
[14] pry(main)> a
NameError: undefined local variable or method `a' for main:Object
from (pry):29:in `__pry__'
[15] pry(main)> name = gets
isowa
=> "isowa\n"
[16] pry(main)> name.chomp!
=> "isowa"
[17] pry(main)> name
=> "isowa"
[18] pry(main)> 
[19] pry(main)> 10.times do |i|
[19] pry(main)*   print i, ", "  
[19] pry(main)* end  
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, => 10
[20] pry(main)> a = ["りんご", "みかん", "ぶどう"]
=> ["りんご", "みかん", "ぶどう"]
[21] pry(main)> a.each do |item|
[21] pry(main)*   puts "おいしい" + item + "だよ"  
[21] pry(main)* end  
おいしいりんごだよ
おいしいみかんだよ
おいしいぶどうだよ
=> ["りんご", "みかん", "ぶどう"]
[22] pry(main)> b= ["あさだ","いそわ","いちはら","いぬい"]
=> ["あさだ", "いそわ", "いちはら", "いぬい"]
[23] pry(main)> b.each do |item|; puts "私は" + item + "だよ"; end
私はあさだだよ
私はいそわだよ
私はいちはらだよ
私はいぬいだよ
=> ["あさだ", "いそわ", "いちはら", "いぬい"]
[24] pry(main)> ```