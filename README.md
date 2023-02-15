# Quadratic-equation-code-using-VB
'
' Created by SharpDevelop.
' User: BRIAN WEREH
' Date: 2/15/2023
' Time: 11:25 AM
' 
' To change this template use Tools | Options | Coding | Edit Standard Headers.
'
Public Partial Class MainForm
	Public Sub New()
		' The Me.InitializeComponent call is required for Windows Forms designer support.
		Me.InitializeComponent()
		
		'
		' TODO : Add constructor code after InitializeComponents
		'
	End Sub
	
	Sub Button2Click(sender As Object, e As EventArgs)
     Me.Close()    		
	End Sub
	
	Sub BtnComputeClick(sender As Object, e As EventArgs)
		Dim a As Integer
		Dim b As Integer
		Dim c As Integer
		Dim x1 As Double
		Dim x2 As Double
		a=Val(txta.Text)
		b=Val(txtb.Text)
		c=Val(txtc.Text)
		x1=(-b+((b*b) +(4*c*a)^1/2))/(2*a)
		x2=(-b-((b*b) +(4*c*a)^1/2))/(2*a)
		lblx1.Text=x1.ToString
		lblx2.Text=x2.ToString
	End Sub
	
	Sub Button3Click(sender As Object, e As EventArgs)
		lblx1.Text="0"
		lblx2.Text="0"
		txta.Clear()
		txtb.Clear()
		txtc.Clear()
	End Sub
End Class
