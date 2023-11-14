# MySql mb_name 칼럼을 조회하여 해당 row를 출력.

## 과제 : 검색 기능 구현 중 기능이 정상 작동하지 않아 문제점을 찾고, 해결

```
기존 소스 (PHP)
$sql_search .= "and mb_name like '{$stxs}' ";

수정 소스
if ($stxs) { 
    if($sxt == '이름') {
        $sql_search .= "and mb_name like '%{$stxs}%' ";
    } else {
        $sql_search .= "and substring_index(".$mb_text.",',',1) = '".$stxs."'";
    }
}
```
<p> 이름만 입력받아 mb_name 칼럼에서 like(특정 문자가 포함되어있는지)를 사용하여 sql문을 실행</p>
<p> > 검색 시 이름으러 검색할지, 특정 조건으로 검색할지를 따져 이름(mb_name)일 경우 기존과 동일하게 like를 쓰나 %를 검색어(stxs)의 앞,뒤로 붙혀 시작하거나 끝나는단어로 전체 포함시킴 </p>
<p> > 특정조건일 경우 특정칼럼($mb_text)에 저장된 값을 ',' 로 구분하여 일치 값을 출력 </p>

### 1차 시도
```
$sql_search .= "and find_in_set($stxs,$mb_text)";
```
> 문제 점 : $mb_text를 , 로 구분하여 배열로 만들었을 때 0번째 배열의 값만 비교해야하나 전체를 비교하는 문제가 생김.
<p> 출처 [ https://www.w3schools.com/sql/func_mysql_find_in_set.asp ] </p>

### 2차 시도
```
$sql_search .= "and substring_index(".$mb_text.",',',1) = '".$stxs."'";
```
> 해결 : substring_index 를 사용하여 ,(특정문자)를 기준으로 배열을 만들어 첫번째 값과 비교하는 sql 문으로 변경
<p> 출처 [ https://www.w3schools.com/sql/func_mysql_substring_index.asp ]</p>


#### 금일은 작업 중 트러블 슈팅이 발생한 것에 대한 공부를 정리 하였다.
#### 당일 작업 하면서 몸이 안좋아져, 약먹고 쉬어 정리가 늦음.