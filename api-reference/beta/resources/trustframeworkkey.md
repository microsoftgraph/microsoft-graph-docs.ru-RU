---
title: Тип ресурса trustFrameworkKey
description: Представляет JWK (веб-ключ JSON). TrustFrameworkKey — это структура данных JSON, которая представляет криптографический ключ. Структура этого ресурса следует формату, определенному в разделе 4 RFC 7517.
localization_priority: Normal
author: valnav
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3de9ce67298f31b3c40682040da69f5c2f6ba007
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135858"
---
# <a name="trustframeworkkey-resource-type"></a>Тип ресурса trustFrameworkKey

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет JWK (веб-ключ JSON). TrustFrameworkKey — это структура данных JSON, которая представляет криптографический ключ. Структура этого ресурса следует формату, определенному в разделе [4 RFC 7517.](https://tools.ietf.org/html/rfc7517#section-4)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| 1 | string | Уникальный идентификатор ключа.   |
| kty | string | Параметр "kty" (тип ключа) определяет семейство криптографических алгоритмов, используемого с ключом. Допустимые значения: rsa, oct. |
| use | string | Параметр "use" (использование открытого ключа) определяет предназначенное использование открытого ключа.  Параметр "use" используется для того, чтобы указать, используется ли открытый ключ для шифрования данных или проверки подписи данных. Возможные значения: 1. "sig" (подпись) 2.  "enc" (шифрование)   |
| x5c | Коллекция строк | Параметр "x5c" (цепочка сертификатов X.509) содержит цепочку из одного или более сертификатов [PKIX RFC 5280.](https://tools.ietf.org/html/rfc5280) |
| x5t | string | Параметр "x5t" (отпечаток сертификата SHA-1 X.509) — это отпечаток SHA-1 в коде base64url (т. е. отпечаток SHA-1). дайджест) кодив der сертификата X.509 [RFC 5280.](https://tools.ietf.org/html/rfc5280) |
| e | string | Ключ RSA — открытый экспонент |
| d| string | Ключ RSA — частный экспонент. Поле не может быть прочитано обратно. |
| n | string | Ключ RSA — модулю |
| p | string | Ключ RSA — первый простор. Поле не может быть прочитано обратно. |
| q | string | Клавиша RSA — second prime. Поле не может быть прочитано обратно. |
| dp | string | Ключ RSA — первый показатель. Поле не может быть прочитано обратно. |
| dq | string | Ключ RSA — второй показатель. Поле не может быть прочитано обратно. |
| фа | string | Ключ RSA — коэффициент. Поле не может быть прочитано обратно. |
| k | string | Симметричный ключ для типа клавиши oct. Поле не может быть прочитано обратно.   |
| nbf | int | Это значение является числовом значении, определенном в RFC 7519 (число JSON, представляющее количество секунд от 1970-01-01T00:00:00Z UTC до указанной даты и времени UTC, игнорируя високосные секунды.) |
| exp | int | Это значение является числовом значении, определенном в RFC 7519 (число JSON, представляющее количество секунд от 1970-01-01T00:00:00Z UTC до указанной даты и времени UTC, игнорируя високосные секунды.) |



## <a name="json-representation"></a>Представление в формате JSON

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


