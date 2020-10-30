# PythonDeobfuscate

import base64
import zlib

OBFUSCATED_SCRIPT = 'PASTE HERE THE RANDOM STRING'

with open('deobuscated-script.txt', 'w') as file:
    file.write("None + None\n" + zlib.decompress(base64.b64decode(OBFUSCATED_SCRIPT)).decode('UTF-8'))
