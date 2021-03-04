---
title: тип ресурса trustFrameworkKeySet
description: Представляет набор ключей и ключей политики для фреймворка доверия.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4bd20bd3b9df4656a3bbc73a52511d64ad463bf5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442770"
---
# <a name="trustframeworkkeyset-resource-type"></a>тип ресурса trustFrameworkKeySet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор ключей и ключей политики для фреймворка доверия. В фреймворках Identity Experience хранится секрет, который можно использовать в политиках. Секретами могут быть пароли, сертификаты или другие файлы. На портале эти сущности показаны как `Policy keys` . В рамках "Опыт удостоверений" используется стандарт веб-ключа JSON (JWK) для клавиш. Эта сущность следует формату, указанному в [разделе 5 RFC 7517.](https://tools.ietf.org/html/rfc7517#section-5)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/trustframework-list-keysets.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) Коллекция | Список trustFrameworkKeySets. |
| [Создание](../api/trustframework-post-keysets.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Создание trustFrameworkKeySet. |
| [получение](../api/trustframeworkkeyset-get.md); | [trustFrameworkKeySet](trustframeworkkeyset.md) | Чтение свойств и связей объекта trustFrameworkKeySet. |
| [Обновление](../api/trustframeworkkeyset-update.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | Обновление объекта trustFrameworkKeySet. |
| [удаление](../api/trustframeworkkeyset-delete.md); | Нет | Удаление объекта trustFrameworkKeySet. |
|[Создание ключа](../api/trustframeworkkeyset-generatekey.md)|[trustFrameworkKey](trustframeworkkey.md)| Создание ключа в наборе ключей. |
|[Получить активный ключ](../api/trustframeworkkeyset-getactivekey.md)|[trustFrameworkKey](trustframeworkkey.md)| Получите активный ключ в наборе ключей. |
|[Сертификат загрузки](../api/trustframeworkkeyset-uploadcertificate.md)|[trustFrameworkKey](trustframeworkkey.md)| Загрузите сертификат X.509. |
|[Загрузка PKCS12](../api/trustframeworkkeyset-uploadpkcs12.md)|[trustFrameworkKey](trustframeworkkey.md)| Загрузите сертификат формата PKCS12. |
|[Отправка секрета](../api/trustframeworkkeyset-uploadsecret.md)|[trustFrameworkKey](trustframeworkkey.md)| Загрузите секрет на основе строки. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор наборов ключей trustframework |
|клавиши|[коллекция trustFrameworkKey](trustframeworkkey.md)| Коллекция ключей. |

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


