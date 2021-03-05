---
title: тип ресурса ipNamedLocation
description: Представляет расположение Azure Active Directory с именем, определенное диапазонами IP. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9e5a8f75be26e46bd24da0ff1f5aa1618cd8c8b4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448822"
---
# <a name="ipnamedlocation-resource-type"></a>тип ресурса ipNamedLocation

Пространство имен: microsoft.graph

Представляет расположение Azure Active Directory с именем, определенное диапазонами IP. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.

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
|createdDateTime|DateTimeOffset|Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Наследуется [от namedLocation](../resources/namedLocation.md).|
|displayName|String|Понятное человеку имя расположения.|
|id|String|Идентификатор объекта namedLocation. Только для чтения. Наследуется [от namedLocation](../resources/namedLocation.md).|
|ipRanges|Коллекция объектов [ipRange](iprange.md)|Список диапазонов IP-адресов в формате CIDR IPv4 (например, 1.2.3.4/32) или любого допустимого формата IPv6 от IETF RFC596.|
|isTrusted|Логический|True, если это расположение явно доверяется.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет последнюю измененную дату и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Наследуется [от namedLocation](../resources/namedLocation.md).|

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

