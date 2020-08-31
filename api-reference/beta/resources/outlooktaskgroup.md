---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), которая содержит задачи Outlook (Коллекция объектов outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: afd5da7663a9328a87b5df2616b0093a4208caeb
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312122"
---
# <a name="outlooktaskgroup-resource-type-deprecated"></a>Тип ресурса outlookTaskGroup (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


Группа папок ([outlookTaskFolder](outlooktaskfolder.md)), которая содержит задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ). 

В Outlook существует группа задач по умолчанию, `My Tasks` которую нельзя переименовать или удалить. Тем не менее, вы можете создать дополнительные группы задач. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение outlookTaskGroup](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |Получение свойств и связей указанной группы задач Outlook.|
|[Создание outlookTaskFolder](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Создайте папку задач Outlook.|
|[Список Таскфолдерс](../api/outlooktaskgroup-list-taskfolders.md) |Коллекция [outlookTaskFolder](outlooktaskfolder.md)| Получение коллекции папок задач Outlook.|
|[обновление](../api/outlooktaskgroup-update.md). | [outlookTaskGroup](outlooktaskgroup.md)  |Обновление свойств, доступных для записи, для группы задач Outlook. |
|[Удаление](../api/outlooktaskgroup-delete.md) | Нет |Удаление указанной группы задач Outlook. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|changeKey|String|Версия группы задач.|
|граупкэй|Edm.Guid|Уникальный идентификатор GUID для группы задач.|
|id|String|Уникальный строковый идентификатор группы задач. Только для чтения.|
|исдефаултграуп|Логический|Значение true, если группа задач является группой задач по умолчанию.|
|name|String|Имя группы задач.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|таскфолдерс|Коллекция [outlookTaskFolder](outlooktaskfolder.md)| Коллекция папок задач в группе задач. Только для чтения. Допускается значение null.|

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
