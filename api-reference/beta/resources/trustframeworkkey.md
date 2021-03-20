---
title: тип ресурса trustFrameworkKey
description: Представляет JWK (веб-ключ JSON). TrustFrameworkKey — это структура данных JSON, представляюная криптографический ключ. Структура этого ресурса следует формату, определенному в разделе RFC 7517 4.
localization_priority: Normal
author: valnav
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b50e82748db6c0c26252ce6b79290781fa88819b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945636"
---
# <a name="trustframeworkkey-resource-type"></a>тип ресурса trustFrameworkKey

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет JWK (веб-ключ JSON). TrustFrameworkKey — это структура данных JSON, представляюная криптографический ключ. Структура этого ресурса следует формату, определенному в [разделе RFC 7517 4](https://tools.ietf.org/html/rfc7517#section-4).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| малыш | string | Уникальный идентификатор для ключа.   |
| kty | Строка | Параметр **kty** (тип ключа) определяет семейство криптографических алгоритмов, используемых с ключом, Допустимые значения `rsa` , `oct` . |
| использование | Строка | Параметр **use** (public key use) определяет предназначенное использование общедоступных ключей.  Параметр **use** используется для того, чтобы указать, используется ли общедоступный ключ для шифрования данных или проверки подписи на данных. Возможные значения: `sig` (подпись), `enc` (шифрование)  |
| x5c | Коллекция строк | Параметр **x5c** (цепочка сертификатов X.509) содержит цепочку из одного или более сертификатов [PKIX RFC 5280.](https://tools.ietf.org/html/rfc5280) |
| x5t | string | Параметр **x5t** (X.509 сертификата SHA-1) является отпечатком пальца sha-1 с кодированной базой 64url (sha-1). дайджест) кодилизовки DER сертификата X.509 [RFC 5280.](https://tools.ietf.org/html/rfc5280) |
| e | string | Клавиша RSA — публичный показатель |
| d| string | Ключ RSA — частный экспонент. Поле не может быть прочитано обратно. |
| n | string | Клавиша RSA — modulus |
| p | string | Клавиша RSA — первый прайм. Поле не может быть прочитано обратно. |
| q | string | Клавиша RSA — второй прайм. Поле не может быть прочитано обратно. |
| dp | string | Клавиша RSA — первый экспонент. Поле не может быть прочитано обратно. |
| dq | string | Клавиша RSA — второй показатель. Поле не может быть прочитано обратно. |
| qi | string | Ключ RSA — коэффициент. Поле не может быть прочитано обратно. |
| k | string | Симметричный ключ для типа ключа oct. Поле не может быть прочитано обратно.   |
| nbf | int | Это значение — numericDate, как определено в RFC 7519 (численное значение JSON, представляющее число секунд с 1970-01-01T00:00:00:00Z UTC до указанной даты UTC/времени, игнорируя високосные секунды.) |
| exp | int | Это значение — numericDate, как определено в RFC 7519 (численное значение JSON, представляющее число секунд с 1970-01-01T00:00:00:00Z UTC до указанной даты UTC/времени, игнорируя високосные секунды.) |



## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKey",
  "baseType": null
}-->

```json
{
  "d": "String",
  "dp": "String",
  "dq": "String",
  "e": "String",
  "exp": 1024,
  "k": "String",
  "kid": "String",
  "kty": "String",
  "n": "String",
  "nbf": 1024,
  "p": "String",
  "q": "String",
  "qi": "String",
  "use": "String",
  "x5c": ["String"],
  "x5t": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKey resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


