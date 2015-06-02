unit Unit1;

{$mode objfpc}{$H+}

interface

uses
  Classes, SysUtils, db, FileUtil, Forms, Controls, Graphics, Dialogs, StdCtrls,
  ValEdit, DBGrids, ExtCtrls, ZConnection, ZDataset;

type

  { TForm1 }

  TForm1 = class(TForm)
    DataSource1: TDataSource;
    DBGrid1: TDBGrid;
    Panel1: TPanel;
    Tambahkan: TButton;
    Ubah: TButton;
    Hapus: TButton;
    keluar: TButton;
    Edit1: TEdit;
    Edit2: TEdit;
    Edit3: TEdit;
    Edit4: TEdit;
    NIS: TLabel;
    Nama: TLabel;
    Kelas: TLabel;
    Email: TLabel;
    ZConnection1: TZConnection;
    ZQuery1: TZQuery;
    ZQuery2: TZQuery;
    procedure Edit1Change(Sender: TObject);
    procedure FormCreate(Sender: TObject);
    procedure TambahkanClick(Sender: TObject);
  private
    { private declarations }
  public
    { public declarations }
  end;

var
  Form1: TForm1;

implementation

{$R *.lfm}

{ TForm1 }

procedure TForm1.FormCreate(Sender: TObject);
begin

end;

procedure TForm1.TambahkanClick(Sender: TObject);
begin
 Zquery2.SQL.Clear;
 try
   ZQuery2.SQL.add('insert into siswa values("'+Edit1.text+'","'+Edit2.text+'","'+Edit3.Text+'","'+Edit4.Text+'")');
   ZQuery2.ExecSQL;
   Showmessage('Berhasil.');
 except
   showmessage('aduh, gagal. coba lagi. :)');

 end;
 ZQuery1.refresh; //Ayo Jalan
end;

procedure TForm1.Edit1Change(Sender: TObject);
begin

end;

end.

