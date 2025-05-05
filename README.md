Pruebas de Flujo Completo
Crear Cliente: POST /clientes
Crear Cuenta: POST /cuentas
Realizar Movimientos:
  POST /movimientos (Depósito)
  POST /movimientos (Retiro)
Generar Reporte: GET /reportes

# Crear cliente
http://localhost:8080/clientes
{
    "nombre": "Juan Osorio",
    "genero": "MASCULINO",
    "edad": 40,
    "identificacion": "098874587",
    "direccion": "13 junio y Equinoccial",
    "telefono": "098874587",
    "contrasena": "1245",
    "estado": true
}

# Crear cuenta
{
    "numeroCuenta": "495878",
    "tipo": "AHORRO",
    "saldoInicial": 0,
    "estado": true,
    "clienteId": 3
}

# Realizar movimiento
{
    "valor": 150.00,
    "numeroCuenta": "495878"
}
