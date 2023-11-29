<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Özge'nin Hediyesi</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 50px;
            background-color: #301409; /* Red: 48, Green: 20, Blue: 9 */
            color: #D2B155; /* Red: 210, Green: 177, Blue: 85 */
        }
        input {
            padding: 10px;
            margin: 10px;
        }
        button {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        h1 {
            font-size: 36px; /* Increase the font size to make it larger */
            color: #D2B155; /* Red: 210, Green: 177, Blue: 85 */
        }
    </style>
</head>
<body>
    <h1>Tebrikler, QR'ı okutan koca yürekli!</h1>
    <p>Özge'nin sana hediyesi var. Kazanmak için aşağıdaki metni doldur.</p>
    <input type="text" id="firstName" placeholder="Ad">
    <br>
    <input type="text" id="lastName" placeholder="Soyad">
    <br>
    <input type="tel" id="phoneNumber" placeholder="Telefon Numarası">
    <br>
    <input type="email" id="emailAddress" placeholder="Mail Adresi">
    <br>
    <button onclick="submitForm()">Gönder</button>

    <script>
        function submitForm() {
            var firstName = document.getElementById('firstName').value;
            var lastName = document.getElementById('lastName').value;
            var phoneNumber = document.getElementById('phoneNumber').value;
            var emailAddress = document.getElementById('emailAddress').value;

            if (firstName && lastName && phoneNumber && emailAddress) {
                alert('Bilgileriniz gönderildi:\n' +
                      'Ad: ' + firstName + '\n' +
                      'Soyad: ' + lastName + '\n' +
                      'Telefon: ' + phoneNumber + '\n' +
                      'Mail: ' + emailAddress);
                // Bu veriyi bir sunucuya gönderebilir veya başka işlemler yapabilirsiniz.
            } else {
                alert('Lütfen tüm bilgileri eksiksiz girin.');
            }
        }
    </script>
</body>
</html>

