# uipath-linq


### Group By

LinQ Test 기록/활용 목적 Repository

(From Data in DataTable.AsEnumerable() Group Data By New with { Key.이름 = Data.Item("이름") } Into grp = Group Where grp.count = 1 Select {Cstr(Data.이름)}).ToList

- List(Of Array(Of String))



### Group By 예시 (UiPath)

(FROM row IN dt_Test.AsEnumerable() Group By X = New With { Key.광고계정 = row.Item("광고계정") } INTO grp = GROUP SELECT {X.광고계정, grp.count(), grp.Sum(function(row) CInt(row.item("키워드 개수")))}).ToList



### Let Usage

(From i in ExtractDataTable.AsEnumerable Let n = CInt(i.item(0)) Where n > 0 Select i)
