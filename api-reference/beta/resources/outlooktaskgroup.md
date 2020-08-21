---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), содержащая задачи Outlook (коллекция объектов outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 112ffab7699a2c8812311ba0c21c2b0e47efff70
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849795"
---
# <a name="outlooktaskgroup-resource-type"></a>Тип ресурса outlookTaskGroup

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


Группа папок[(outlookTaskFolder),](outlooktaskfolder.md)которая содержит задачи Outlook (коллекция [объектов outlookTask).](outlooktask.md) 

В Outlook есть группа задач по умолчанию, `My Tasks` которую невозможно переименовать или удалить. Однако можно создавать дополнительные группы задач. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get outlookTaskGroup](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |Получение свойств и связей указанной группы задач Outlook.|
|[Создание объекта outlookTaskFolder](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Создайте папку задач Outlook.|
|[Перечисление объектов taskFolder](../api/outlooktaskgroup-list-taskfolders.md) |[Коллекция outlookTaskFolder](outlooktaskfolder.md)| Получение коллекции папок задач Outlook.|
|[обновление](../api/outlooktaskgroup-update.md). | [outlookTaskGroup](outlooktaskgroup.md)  |Обновление записываемых свойств группы задач Outlook. |
|[удаление](../api/outlooktaskgroup-delete.md); | Нет |Удаление указанной группы задач Outlook. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|changeKey|String|Версия группы задач.|
|groupKey|Edm.Guid|Уникальный идентификатор GUID группы задач.|
|id|String|Уникальный строковый идентификатор группы задач. Только для чтения.|
|isDefaultGroup|Boolean|True, если группа задач является группой задач по умолчанию.|
|name|String|Имя группы задач.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|taskFolders|[Коллекция outlookTaskFolder](outlooktaskfolder.md)| Коллекция папок задач в группе задач. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
