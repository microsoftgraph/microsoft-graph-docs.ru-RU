---
title: Тип ресурса Трустфрамеворккэйсет
description: Представляет ключи набора ключей и политики для инфраструктуры доверия.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2620a7aca90e8a8ae27880343914dfcbbabe27d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519647"
---
# <a name="trustframeworkkeyset-resource-type"></a>Тип ресурса Трустфрамеворккэйсет

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ключи набора ключей и политики для инфраструктуры доверия. В платформе удостоверений хранятся секреты, которые можно использовать в политиках. Секреты могут представлять собой пароли, сертификаты и другие файлы. В портале эти сущности отображаются как `Policy keys`. Платформа удостоверений использует стандарт JSON Web Key (ЖВК) для кэйсетс. Эта сущность соответствует формату, указанному в [RFC 7517 в разделе 5](https://tools.ietf.org/html/rfc7517#section-5).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List](../api/trustframework-list-keysets.md) | [трустфрамеворккэйсет](trustframeworkkeyset.md) Семейства | Список Трустфрамеворккэйсетс. |
| [создание](../api/trustframework-post-keysets.md); | [трустфрамеворккэйсет](trustframeworkkeyset.md) | Создайте Трустфрамеворккэйсет. |
| [получение](../api/trustframeworkkeyset-get.md); | [трустфрамеворккэйсет](trustframeworkkeyset.md) | Чтение свойств и связей объекта Трустфрамеворккэйсет. |
| [обновление](../api/trustframeworkkeyset-update.md). | [трустфрамеворккэйсет](trustframeworkkeyset.md) | Обновление объекта Трустфрамеворккэйсет. |
| [удаление](../api/trustframeworkkeyset-delete.md); | Нет | Удаление объекта Трустфрамеворккэйсет. |
|[Создание ключа](../api/trustframeworkkeyset-generatekey.md)|[трустфрамеворккэй](trustframeworkkey.md)| Создание ключа в наборе ключей. |
|[Получение активного ключа](../api/trustframeworkkeyset-getactivekey.md)|[трустфрамеворккэй](trustframeworkkey.md)| Получить активный в данный момент ключ в наборе ключей. |
|[Отправка сертификата](../api/trustframeworkkeyset-uploadcertificate.md)|[трустфрамеворккэй](trustframeworkkey.md)| Отправьте сертификат X. 509. |
|[Отправка PKCS12](../api/trustframeworkkeyset-uploadpkcs12.md)|[трустфрамеворккэй](trustframeworkkey.md)| Отправьте сертификат формата PKCS12. |
|[Отправка секрета](../api/trustframeworkkeyset-uploadsecret.md)|[трустфрамеворккэй](trustframeworkkey.md)| Отправка секрета на основе строки. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор набора ключей трустфрамеворк |
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
