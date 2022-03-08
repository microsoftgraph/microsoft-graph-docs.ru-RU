---
title: тип ресурсов аббревиатуры
description: Аббревиатура — это административный ответ в результатах поиска Майкрософт для определения общих аббревиатур в организации.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0201a3b76201825b13e069b52924eacca9077d9f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339593"
---
# <a name="acronym-resource-type"></a>тип ресурсов аббревиатуры

Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Аббревиатура — это административный ответ в результатах поиска Майкрософт для определения общих аббревиатур в организации.

Наследуется [из searchAnswer](../resources/search-searchAnswer.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Акронимы списка](../api/search-searchentity-list-acronyms.md)|[коллекция microsoft.graph.search.acronym](../resources/search-acronym.md)|Получите список объектов [аббревиатуры](../resources/search-acronym.md) и их свойств.|
|[Создание аббревиатуры](../api/search-searchentity-post-acronyms.md)|[microsoft.graph.search.acronym](../resources/search-acronym.md)|Создайте новый [объект аббревиатуры](../resources/search-acronym.md) .|
|[Получить аббревиатура](../api/search-acronym-get.md)|[microsoft.graph.search.acronym](../resources/search-acronym.md)|Ознакомьтесь с свойствами и отношениями объекта [аббревиатуры](../resources/search-acronym.md) .|
|[Аббревиатура Update](../api/search-acronym-update.md)|[microsoft.graph.search.acronym](../resources/search-acronym.md)|Обновление свойств объекта [аббревиатуры](../resources/search-acronym.md) .|
|[Удаление аббревиатуры](../api/search-acronym-delete.md)|Нет|Удаляет объект [аббревиатуры](../resources/search-acronym.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Краткое описание аббревиатуры, которая предоставляет пользователям дополнительные сведения о аббревиатуре и о том, что она означает. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|displayName|String|Фактическая короткая форма или аббревиатура. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|id|Строка|Уникальный идентификатор (GUID) для аббревиатуры. Наследуется [от сущности](../resources/entity.md).|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|Сведения о пользователе, который создал или в последний раз изменил аббревиатура. Наследуется [от searchAnswer](../resources/search-searchAnswer.md). Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Время создания или редактирования аббревиатуры. Наследуется [от searchAnswer](../resources/search-searchAnswer.md). Только для чтения.|
|standsFor|Коллекция String|Что такое аббревиатура.|
|state|microsoft.graph.search.answerState|Состояние аббревиатуры. Возможные значения: `published`, , `draft`, или `excluded``unknownFutureValue`.|
|webUrl|String|URL-адрес страницы или веб-сайта, на котором пользователи могут получить дополнительные сведения о аббревиатуре. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.acronym",
  "baseType": "microsoft.graph.search.searchAnswer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.acronym",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "standsFor": [
    "String"
  ],
  "state": "String"
}
```

