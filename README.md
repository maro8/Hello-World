# Hello-World
Test
Just trying


Private Sub WorkSheet_Change(ByVal Target As Range)
    If Intersect(Target, Range("B2:C3")) Is Nothing Then
        Exit Sub
    Else
        Sample
    End If
End Sub

Sub Sample()
'ThisSheet.AutoFilter = False
    Range("B4:C5").Select
    Selection.AutoFilter Field:=1, Criteria1:=Range("B2").Value, Operator:=xlOr, Criteria2:=Range("C2").Value
    
End Sub

Sub Sample2()
Cells.AutoFilter
End Sub
