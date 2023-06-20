# kodluyoruzilkrepo
Kodluyoruz Front-End Eğitim kapsamında açtığım ilk repo
Imports System.Windows.Forms

Public Class Form1
    Inherits Form

    Private WithEvents button As Button

    Public Sub New()
        button = New Button()
        button.Text = "Tıkla"
        button.Location = New Point(50, 50)
        button.Size = New Size(100, 30)

        Controls.Add(button)
    End Sub

    Private Sub Button_Click(sender As Object, e As EventArgs) Handles button.Click
        MessageBox.Show("Merhaba, Dünya!")
    End Sub

    Public Shared Sub Main()
        Application.Run(New Form1())
    End Sub
End Class
