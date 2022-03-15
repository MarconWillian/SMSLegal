![SMSLegal][smslegal-logo]
# ✉️ SMSLegal

## Install

You can install with [npm][smslegal-npm]:
```bash
  npm install smslegal
```

You can install with [yarn][smslegal-yarn]:
```bash
  yarn add smslegal
```


## Features

  * Enviar SMS
  * Verificar Status de SMS
  * Verificar Quantidade de SMS

## Config Start

First you need import the package for your project:

```TypeScript
const smslegal = require('smslegal');
```

  You need config with yours access:

```TypeScript
smslegal.config({user: "YOUR_USER", pass: "YOUR_PASS"});
```

## Examples

Verify balance of account.
```TypeScript
smslegal.balance()
```

  You can send a async sms, the number has to count the code 55 from brazil, after the ddd without the 0, plus 9 mobile number:

```TypeScript
smslegal.send({numberSMS: 5566999999999, message: "Message SMS"})
```

You can verify status of your sms of you send.
```TypeScript
smslegal.verifyStatus({messageId: 123112})
```


****
This project is under the MIT license. See the [LICENSE][license-link] file for more details.


<!-- Markdown link & img's -->
[license-link]: /LICENSE
[smslegal-logo]: https://i.imgur.com/9eCs2eb.png
[smslegal-npm]: https://www.npmjs.com/package/smslegal
[smslegal-yarn]: https://yarnpkg.com/package/smslegal
