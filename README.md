Simple base45 (charset of Qr codes, alphanumeric mode) encoder/decoder.

Typical use:

```
	var input = "A string..."
	var buffer = System.Text.Encoding.ASCII.GetBytes(input);
	string encoded = Base45Encoding.Encode(buffer);

	string input = "01234"
	byte[] decoded = Base45Encoding.Decode(input);
	var stringResult = System.Text.Encoding.ASCII.GetString(decoded);

```

