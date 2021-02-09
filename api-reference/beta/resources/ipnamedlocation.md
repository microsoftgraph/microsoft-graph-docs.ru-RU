---
title: Тип ресурса ipNamedLocation
description: Представляет именуемую позицию Azure Active Directory, определяемую диапазонами IP-адресов. Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b63452ca6eefb9ad3a0d4b3f860fb1a8d41638fb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158403"
---
# <a name="ipnamedlocation-resource-type"></a>Тип ресурса ipNamedLocation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет именуемую позицию Azure Active Directory, определяемую диапазонами IP-адресов. Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.

Наследуется от [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список ipNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [Коллекция ipNamedLocation](ipNamedLocation.md) | Получить все **объекты ipNamedLocation** в организации. |
| [Создание ipNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [ipNamedLocation](ipNamedLocation.md) | Создание объекта **ipNamedLocation.** |
| [Get ipNamedLocation](../api/ipnamedlocation-get.md) | [ipNamedLocation](ipnamedlocation.md) | Чтение свойств и связей объекта **ipNamedLocation.** |
| [Обновление ipNamedLocation](../api/ipnamedlocation-update.md) | [ipNamedLocation](ipnamedlocation.md) | Обновление объекта **ipNamedLocation.** |
| [Удаление ipNamedLocation](../api/ipnamedlocation-delete.md) | Нет | Удаление объекта **ipNamedLocation.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет дату и время создания расположения в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Наследуется [от namedLocation.](../resources/namedLocation.md)|
|displayName|String|Понятное человеку имя расположения.|
|id|String|Идентификатор объекта namedLocation. Только для чтения. Наследуется [от namedLocation.](../resources/namedLocation.md)|
|ipRanges|Коллекция объектов [ipRange](iprange.md)|Список диапазонов IP-адресов в формате IPv4 CIDR (например, 1.2.3.4/32) или любой допустимый формат IPv6 из IETF RFC596.|
|isTrusted|Boolean|Имеет true, если это расположение является явным доверенным.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет дату и время последнего изменения расположения в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Наследуется [от namedLocation.](../resources/namedLocation.md)|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipNamedLocation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "ipRanges": [{"@odata.type": "microsoft.graph.ipRange"}],
  "isTrusted": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ipNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


