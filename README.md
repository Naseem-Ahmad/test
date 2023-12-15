
<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">
<head runat="server">
    <title>Your Page Title</title>
    <!-- Include Bootstrap and jQuery libraries here -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"/>
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"></script>

    <!-- Bootstrap Datepicker CSS and JS -->
    <link rel="stylesheet" href="Scripts/bootstrap-datepicker.css"/>
    <script src="Scripts/bootstrap-datepicker.js"></script>
</head>
<body>
    <form id="form1" runat="server">
        <div>
            <!-- Your TextBox control with Bootstrap classes -->
            <asp:TextBox ID="textID" CssClass="form-control datepicker" runat="server"></asp:TextBox>
        </div>
    </form>

    <!-- Initialize the datepicker in your script -->
    <script>
        $(document).ready(function () {
            // Assuming your datepicker class is 'datepicker'
            $('.datepicker').datepicker({
                format: 'dd/mm/yyyy', // Customize the date format as needed
                autoclose: true
            });
        });
    </script>
</body>
</html>
