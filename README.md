# UiPath-LinQ


LinQ Test

(From Data as DataTable.AsEnumerable() Group Data By New with { Key.이름 = Data.Item("이름") } Into grp = Group Where grp.count = 1 Select {Cstr(Data.이름)}).ToList

>> List(Of Array(Of String))