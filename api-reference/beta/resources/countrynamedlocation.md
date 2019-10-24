---
title: Тип ресурса Каунтринамедлокатион
description: Представляет имя расположения Azure Active Directory, определенное странами и регионами. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cb413aab72abe401152b67b985f023350f80f30
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653673"
---
# <a name="countrynamedlocation-resource-type"></a>Тип ресурса Каунтринамедлокатион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет имя расположения Azure Active Directory, определенное странами и регионами. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.

Наследуется от [намедлокатион](../resources/namedLocation.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Каунтринамедлокатионс](../api/conditionalaccessroot-list-namedlocations.md) | Коллекция [каунтринамедлокатион](countryNamedLocation.md) | Получение всех объектов **каунтринамедлокатион** в Организации. |
| [Создание Каунтринамедлокатион](../api/conditionalaccessroot-post-namedlocations.md) | [каунтринамедлокатион](countryNamedLocation.md) | Создание нового объекта **каунтринамедлокатион** . |
| [Получение Каунтринамедлокатион](../api/countrynamedlocation-get.md) | [каунтринамедлокатион](countrynamedlocation.md) | Чтение свойств и связей объекта **каунтринамедлокатион** . |
| [Обновление Каунтринамедлокатион](../api/countrynamedlocation-update.md) | [каунтринамедлокатион](countrynamedlocation.md) | Обновление объекта **каунтринамедлокатион** . |
| [Удаление Каунтринамедлокатион](../api/countrynamedlocation-delete.md) | Нет | Удаление объекта **каунтринамедлокатион** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|каунтриесандрегионс|Коллекция строк|Список стран и/или регионов в формате из двух букв, заданных в стандарте ISO 3166-2.|
|createdDateTime|DateTimeOffset|Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Наследуется от [намедлокатион](../resources/namedLocation.md).|
|displayName|Строка|Удобное для человека имя расположения. Наследуется от [намедлокатион](../resources/namedLocation.md).|
|id|String|Идентификатор объекта Намедлокатион. Только для чтения. Наследуется от [намедлокатион](../resources/namedLocation.md).|
|инклудеункновнкаунтриесандрегионс|Логический|Значение true, если IP-адреса, которые не сопоставляются со страной или регионом, должны быть включены в именованное расположение.|
|modifiedDateTime|DateTimeOffset|Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Наследуется от [намедлокатион](../resources/namedLocation.md).|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation",
  "baseType": ""
}-->

```json
{
  "countriesAndRegions": ["String"],
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "includeUnknownCountriesAndRegions": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "countryNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
