---
title: Тип ресурса Каунтринамедлокатион
description: Представляет имя расположения Azure Active Directory, определенное странами и регионами. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8c4807abc04cb980ec452590b9643f2b07d0ce67
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016711"
---
# <a name="countrynamedlocation-resource-type"></a>Тип ресурса Каунтринамедлокатион

Пространство имен: microsoft.graph

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
|каунтриесандрегионс|Коллекция String|Список стран и/или регионов в формате из двух букв, заданных в стандарте ISO 3166-2.|
|createdDateTime|DateTimeOffset|Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Наследуется от [намедлокатион](../resources/namedLocation.md).|
|displayName|String|Удобное для человека имя расположения. Наследуется от [намедлокатион](../resources/namedLocation.md).|
|id|String|Идентификатор объекта Намедлокатион. Только для чтения. Наследуется от [намедлокатион](../resources/namedLocation.md).|
|инклудеункновнкаунтриесандрегионс|Boolean|Значение true, если IP-адреса, которые не сопоставляются со страной или регионом, должны быть включены в именованное расположение.|
|modifiedDateTime|DateTimeOffset|Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Наследуется от [намедлокатион](../resources/namedLocation.md).|

## <a name="relationships"></a>Отношения

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


