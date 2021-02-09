---
title: Тип ресурса trustFrameworkKeySet
description: Представляет набор ключей и ключи политики для структуры доверия.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4223681a11ff11b8ea75b165247b5269d1a6cf84
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159859"
---
# <a name="trustframeworkkeyset-resource-type"></a>Тип ресурса trustFrameworkKeySet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор ключей и ключи политики для структуры доверия. В базе identity Experience framework хранится секрет, который можно использовать в политиках. Секреты могут быть паролями, сертификатами или другими файлами. На портале эти сущности показаны как `Policy keys` . В структуре identity Experience используется стандарт JSON Web Key (JWK) для ключей. Эта сущность следует формату, указанному в разделе [5 RFC 7517.](https://tools.ietf.org/html/rfc7517#section-5)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/trustframework-list-keysets.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) Коллекция | Список trustFrameworkKeySets. |
| [Создание](../api/trustframework-post-keysets.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Создание trustFrameworkKeySet. |
| [Получение](../api/trustframeworkkeyset-get.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Чтение свойств и связей объекта trustFrameworkKeySet. |
| [Обновление](../api/trustframeworkkeyset-update.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Обновление объекта trustFrameworkKeySet. |
| [удаление](../api/trustframeworkkeyset-delete.md); | Нет | Удаление объекта trustFrameworkKeySet. |
|[Создание ключа](../api/trustframeworkkeyset-generatekey.md)|[trustFrameworkKey](trustframeworkkey.md)| Создание ключа в наборе ключей. |
|[Получить активный ключ](../api/trustframeworkkeyset-getactivekey.md)|[trustFrameworkKey](trustframeworkkey.md)| Получите текущий активный ключ в наборе ключей. |
|[Отправка сертификата](../api/trustframeworkkeyset-uploadcertificate.md)|[trustFrameworkKey](trustframeworkkey.md)| Отправка сертификата X.509. |
|[Отправка PKCS12](../api/trustframeworkkeyset-uploadpkcs12.md)|[trustFrameworkKey](trustframeworkkey.md)| Отправка сертификата формата PKCS12. |
|[Секрет отправки](../api/trustframeworkkeyset-uploadsecret.md)|[trustFrameworkKey](trustframeworkkey.md)| Отправка секрета на основе строки. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор наборов ключей инфраструктуры доверия |
|keys|[Коллекция trustFrameworkKey](trustframeworkkey.md)| Коллекция ключей. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "keys": [{"@odata.type": "microsoft.graph.trustFrameworkKey"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


