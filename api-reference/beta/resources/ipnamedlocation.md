---
title: тип ресурса ipNamedLocation
description: Представляет расположение Azure Active Directory, определенное диапазонами IP. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 44fc4c076f5c99ca0f14e0fc2771ad930f20b144
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161741"
---
# <a name="ipnamedlocation-resource-type"></a>тип ресурса ipNamedLocation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расположение Azure Active Directory, определенное диапазонами IP. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.

Наследует от [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список ipNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [коллекция ipNamedLocation](ipNamedLocation.md) | Получите все **объекты ipNamedLocation** в организации. |
| [Создание ipNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [ipNamedLocation](ipNamedLocation.md) | Создание нового **объекта ipNamedLocation.** |
| [Get ipNamedLocation](../api/ipnamedlocation-get.md) | [ipNamedLocation](ipnamedlocation.md) | Ознакомьтесь с свойствами и отношениями **объекта ipNamedLocation.** |
| [Обновление ipNamedLocation](../api/ipnamedlocation-update.md) | [ipNamedLocation](ipnamedlocation.md) | Обновление **объекта ipNamedLocation.** |
| [Удаление ipNamedLocation](../api/ipnamedlocation-delete.md) | Нет | Удаление **объекта ipNamedLocation.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. Наследуется [от namedLocation](../resources/namedLocation.md).|
|displayName|Строка|Понятное человеку имя расположения. Обязательный.|
|id|Строка|Идентификатор объекта namedLocation. Только для чтения. Наследуется [от namedLocation](../resources/namedLocation.md).|
|ipRanges|Коллекция объектов [ipRange](iprange.md)|Список диапазонов IP-адресов в формате CIDR IPv4 (например, 1.2.3.4/32) или любого допустимого формата IPv6 от IETF RFC596. Обязательный.|
|isTrusted|Логическое|`true` если это расположение явно доверяется. Необязательно. Значение по умолчанию — `false`.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет последнюю измененную дату и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. Наследуется [от namedLocation](../resources/namedLocation.md).|

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

## <a name="see-also"></a>См. также

+ [Что такое условный доступ?](/azure/active-directory/conditional-access/overview)
+ [Использование условия расположения в политике условного доступа](/azure/active-directory/conditional-access/location-condition)


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ipNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


