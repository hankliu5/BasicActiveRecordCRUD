# Active Record Relationships

這次的作業主要是利用上一次的作業(在master branch中)，來練習relationships。

1. 首先要先了解到所有表格的關係

     |------| 1      1 |----------|
     | User |----------| Profile  |
     |------|          |----------|
          |
          |  1   * |----------| 1      * |----------|
          |--------| TodoList |----------| TodoItem |
                   |----------|          |----------|

2. 接著在app/models下的檔案建立各個表格的關係，然後在db/migrate中的檔案。
（詳情請看檔案中的註解）

3. 建立seeds.rb

4. 在TodoList跟TodoItem中設定default_scope，讓排序是ascending的順序

5. 在User跟Profile中建立validation

6. 在各model中建立dependency

7. 在User model class下加入一個method -- get_completed_count

8. 加入一個class method -- self.get_all_profiles，其中會使用到SQL語法(optional)，
設定搜尋範圍時要避免SQL injection，最後依照ascending的順序回傳birth_year。

That's it!
