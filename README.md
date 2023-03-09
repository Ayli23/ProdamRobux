# ProdamRobux

<html>
<head><title>Калькулятор</title>

<script language="JavaScript">
<!--
//Поучение пользовательских данных и вычисление результата
function GetResult(oper)
{ 
  var n1 = 0;
  var n2 = 0;
    	
  n1 = eval(calcform.num_01.value);   //Число 1
  n2 = eval(calcform.num_02.value);   //Число 2
  
  switch (oper)                       //Проверяем, какая кнопка
  {                                   //была нажата
    case 3:   //Кнопка *
    {
      calcform.res.value = n1 * n2;
      break;
    }
  }
}
// -->
</script>

</head>
<body>
    

    <form name="calcform">

        <table border="20" cellpadding=40 width=350 bgcolor="lightyellow" >

            <tr>
                <td>руб:</td>
                <td>
                    <center>
                        <input name="num_01" type="text" size="30" maxlength=25 value="1">
                    </center>
                </td>
            </tr>

            <tr>
                <td>Робуксов:</td>
                <td>
                    <center>
                        <input name="num_02" type="text" size="24" maxlength=16 value="3" readonly="true" color="green" ;>
                    </center>
            </tr>
            <tr>
                <td>Ответ:</td>
                <td>
                    <center>
                        <input name="res" type="text" maxlength=0 readonly="true" size="20">
                    </center>
                </td>
            </tr>

        </table>

        <table border="20" cellpadding=10 width=15 style="padding: 10px 180px;">


            <tr bgcolor="lightgreen">
                </td>
                <td>
                    <center>
                        <input name="btnmul" type="button" value="  Отправить  " onClick="GetResult(3)">
                    </center>
                </td>
            </tr>

        </table>

    </form>
</body>
</html>
