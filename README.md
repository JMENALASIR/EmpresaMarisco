# EmpresaMarisco
INSERT INTO [EmpresaMarisco].[dbo].[EMPLEADOS](DNIEmpleado, NombreEmpleado, ApellidosEmpleado, TelefonoEmpleado, DomicilioEmpleado, idEmpleadoEncargadoFK1) 
VALUES ('12345698A','Juan','Lopez Onz','628568946','Calle Portugal nº6 2º izq','1'),('98745612B','Iris','Gonzalez Pardo','612694389','Avenida Rioja nº1 1º A','2');
SELECT * FROM EMPLEADOS

INSERT INTO [EmpresaMarisco].[dbo].[GESTORES](TitulacionGestoria, IdEmpleadoFK2) 
VALUES ('Gestoria Superior','1'),('Gestoria basica','2');
SELECT * FROM GESTORES

INSERT INTO [EmpresaMarisco].[dbo].[ADMINISTRATIVOS](TitulosAdministrativos, Contabilidad, idEmpleadoFK3) 
VALUES ('Administracion de Empresa','Si','1'),('Administracion empresarial','Si','2');
SELECT * FROM ADMINISTRATIVOS

INSERT INTO [EmpresaMarisco].[dbo].[ORDENCOMPRAS](FechaOrdenCompra, PesoOrdenCompra, SubTotalOrdenCompra, IVAOrdenCompra, TotalOrdenCompra, idEmpleadoFK4) 
VALUES ('2021/03/10','25.50','300.97','21.00','346.56','1'),('2021/03/11','50.00','421.29','21.00','487.46','2');
SELECT * FROM ORDENCOMPRAS

INSERT INTO [EmpresaMarisco].[dbo].[PRODUCTOS](FechaPescaProducto, NombreProducto, StockProducto, idOrdenCompraFK5) 
VALUES ('2021/03/09','Gambones','500','1'),('2021/03/11','Cangrejo Real','20','2');
SELECT * FROM PRODUCTOS

INSERT INTO [EmpresaMarisco].[dbo].[ENCARGOS](FechaEncargo, PesoEncargo, idOrdenCompraFK6, idProductoFK7) 
VALUES ('2021/03/10','25.50','1','1'),('2021/03/11','50.00','2','2');
SELECT * FROM ENCARGOS
