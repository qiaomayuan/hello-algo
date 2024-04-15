<!--
    File: two_sum.md
    Created Time: 2024-01-05
    Author: krahets (krahets@163.com)
--->

<!-- [file]{two_sum}-[class]{}-[func]{two_sum_brute_force} -->
https://pythontutor.com/render.html#code=def%20two_sum_brute_force%28nums%3A%20list%5Bint%5D%2C%20target%3A%20int%29%20-%3E%20list%5Bint%5D%3A%0A%20%20%20%20%22%22%22%E6%96%B9%E6%B3%95%E4%B8%80%EF%BC%9A%E6%9A%B4%E5%8A%9B%E5%88%97%E8%88%89%22%22%22%0A%20%20%20%20%23%20%E5%85%A9%E5%B1%A4%E8%BF%B4%E5%9C%88%EF%BC%8C%E6%99%82%E9%96%93%E8%A4%87%E9%9B%9C%E5%BA%A6%E7%82%BA%20O%28n%5E2%29%0A%20%20%20%20for%20i%20in%20range%28len%28nums%29%20-%201%29%3A%0A%20%20%20%20%20%20%20%20for%20j%20in%20range%28i%20%2B%201%2C%20len%28nums%29%29%3A%0A%20%20%20%20%20%20%20%20%20%20%20%20if%20nums%5Bi%5D%20%2B%20nums%5Bj%5D%20%3D%3D%20target%3A%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20return%20%5Bi%2C%20j%5D%0A%20%20%20%20return%20%5B%5D%0A%0A%22%22%22Driver%20Code%22%22%22%0Aif%20__name__%20%3D%3D%20%22__main__%22%3A%0A%20%20%20%20nums%20%3D%20%5B2%2C%207%2C%2011%2C%2015%5D%0A%20%20%20%20target%20%3D%2013%0A%20%20%20%20res%20%3D%20two_sum_brute_force%28nums%2C%20target%29&cumulative=false&curInstr=5&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=311&rawInputLstJSON=%5B%5D&textReferences=false

<!-- [file]{two_sum}-[class]{}-[func]{two_sum_hash_table} -->
https://pythontutor.com/render.html#code=def%20two_sum_hash_table%28nums%3A%20list%5Bint%5D%2C%20target%3A%20int%29%20-%3E%20list%5Bint%5D%3A%0A%20%20%20%20%22%22%22%E6%96%B9%E6%B3%95%E4%BA%8C%EF%BC%9A%E8%BC%94%E5%8A%A9%E9%9B%9C%E6%B9%8A%E8%A1%A8%22%22%22%0A%20%20%20%20%23%20%E8%BC%94%E5%8A%A9%E9%9B%9C%E6%B9%8A%E8%A1%A8%EF%BC%8C%E7%A9%BA%E9%96%93%E8%A4%87%E9%9B%9C%E5%BA%A6%E7%82%BA%20O%28n%29%0A%20%20%20%20dic%20%3D%20%7B%7D%0A%20%20%20%20%23%20%E5%96%AE%E5%B1%A4%E8%BF%B4%E5%9C%88%EF%BC%8C%E6%99%82%E9%96%93%E8%A4%87%E9%9B%9C%E5%BA%A6%E7%82%BA%20O%28n%29%0A%20%20%20%20for%20i%20in%20range%28len%28nums%29%29%3A%0A%20%20%20%20%20%20%20%20if%20target%20-%20nums%5Bi%5D%20in%20dic%3A%0A%20%20%20%20%20%20%20%20%20%20%20%20return%20%5Bdic%5Btarget%20-%20nums%5Bi%5D%5D%2C%20i%5D%0A%20%20%20%20%20%20%20%20dic%5Bnums%5Bi%5D%5D%20%3D%20i%0A%20%20%20%20return%20%5B%5D%0A%0A%22%22%22Driver%20Code%22%22%22%0Aif%20__name__%20%3D%3D%20%22__main__%22%3A%0A%20%20%20%20nums%20%3D%20%5B2%2C%207%2C%2011%2C%2015%5D%0A%20%20%20%20target%20%3D%2013%0A%20%20%20%20res%20%3D%20two_sum_hash_table%28nums%2C%20target%29&cumulative=false&curInstr=5&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=311&rawInputLstJSON=%5B%5D&textReferences=false