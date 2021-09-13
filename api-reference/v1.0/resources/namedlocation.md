---
title: тип ресурса namedLocation
description: Это базовый класс, который представляет расположение Azure Active Directory имени. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 01825465c415ef3a769812896dbc80105c50ed68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084274"
---
# <a name="namedlocation-resource-type"></a>тип ресурса namedLocation

Пространство имен: microsoft.graph

Это базовый класс, который представляет расположение Azure Active Directory имени. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список namedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [коллекция namedLocation](namedLocation.md) | Получите все **объекты namedLocation** в организации. |
| [Get namedLocation](../api/namedlocation-get.md) | [namedLocation](namedlocation.md) | Ознакомьтесь с свойствами и отношениями объекта **с именемLocation.** |
| [Удаление namedLocation](../api/namedlocation-delete.md) | Нет | Удаление **объекта namedLocation.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|displayName|String|Понятное человеку имя расположения.|
|id|Строка|Идентификатор объекта namedLocation. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет последнюю измененную дату и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
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
  "description": "namedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

