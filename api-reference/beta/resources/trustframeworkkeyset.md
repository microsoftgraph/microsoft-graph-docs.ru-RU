---
title: Тип ресурса Трустфрамеворккэйсет
description: Представляет ключи набора ключей и политики для инфраструктуры доверия.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 17e9e0d73ce25fab0462d6ee8eb50e3e232f8340
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083892"
---
# <a name="trustframeworkkeyset-resource-type"></a>Тип ресурса Трустфрамеворккэйсет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ключи набора ключей и политики для инфраструктуры доверия. В платформе удостоверений хранятся секреты, которые можно использовать в политиках. Секреты могут представлять собой пароли, сертификаты и другие файлы. В портале эти сущности отображаются как `Policy keys` . Платформа удостоверений использует стандарт JSON Web Key (ЖВК) для кэйсетс. Эта сущность соответствует формату, указанному в [RFC 7517 в разделе 5](https://tools.ietf.org/html/rfc7517#section-5).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление](../api/trustframework-list-keysets.md) | [трустфрамеворккэйсет](trustframeworkkeyset.md) Семейства | Список Трустфрамеворккэйсетс. |
| [Создание](../api/trustframework-post-keysets.md) | [трустфрамеворккэйсет](trustframeworkkeyset.md) | Создайте Трустфрамеворккэйсет. |
| [Получение](../api/trustframeworkkeyset-get.md) | [трустфрамеворккэйсет](trustframeworkkeyset.md) | Чтение свойств и связей объекта Трустфрамеворккэйсет. |
| [Обновление](../api/trustframeworkkeyset-update.md) | [трустфрамеворккэйсет](trustframeworkkeyset.md) | Обновление объекта Трустфрамеворккэйсет. |
| [удаление](../api/trustframeworkkeyset-delete.md); | Нет | Удаление объекта Трустфрамеворккэйсет. |
|[Создание ключа](../api/trustframeworkkeyset-generatekey.md)|[трустфрамеворккэй](trustframeworkkey.md)| Создание ключа в наборе ключей. |
|[Получение активного ключа](../api/trustframeworkkeyset-getactivekey.md)|[трустфрамеворккэй](trustframeworkkey.md)| Получить активный в данный момент ключ в наборе ключей. |
|[Отправка сертификата](../api/trustframeworkkeyset-uploadcertificate.md)|[трустфрамеворккэй](trustframeworkkey.md)| Отправьте сертификат X. 509. |
|[Отправка PKCS12](../api/trustframeworkkeyset-uploadpkcs12.md)|[трустфрамеворккэй](trustframeworkkey.md)| Отправьте сертификат формата PKCS12. |
|[Отправка секрета](../api/trustframeworkkeyset-uploadsecret.md)|[трустфрамеворккэй](trustframeworkkey.md)| Отправка секрета на основе строки. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Уникальный идентификатор набора ключей трустфрамеворк |
|переключен|Коллекция [трустфрамеворккэй](trustframeworkkey.md)| Коллекция ключей. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "baseType": "",
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


