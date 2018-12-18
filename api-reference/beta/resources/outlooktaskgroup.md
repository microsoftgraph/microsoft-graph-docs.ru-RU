---
title: Тип ресурса outlookTaskGroup
description: 'Группа папок (outlookTaskFolder), которые содержат задачи Outlook (коллекцию объектов outlookTask). '
author: angelgolfer-ms
ms.openlocfilehash: 9fed69e1401f2b11ae3630a3c4cef66fd9446920
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359397"
---
# <a name="outlooktaskgroup-resource-type"></a>Тип ресурса outlookTaskGroup

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Группа папок ([outlookTaskFolder](outlooktaskfolder.md)), которые содержат задачи Outlook (коллекцию объектов [outlookTask](outlooktask.md) ). 

В программе Outlook является группу задач по умолчанию `My Tasks` которого невозможно переименование или удаление. Тем не менее, можно создать дополнительные группы задач. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение outlookTaskGroup](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |Получите свойства и связи в указанную группу задач Outlook.|
|[Создание outlookTaskFolder](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Создайте папку задач Outlook.|
|[Список taskFolders](../api/outlooktaskgroup-list-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md) коллекции| Получите коллекцию папок задач Outlook.|
|[обновление](../api/outlooktaskgroup-update.md). | [outlookTaskGroup](outlooktaskgroup.md)  |Обновление для записи свойств группы задач Outlook. |
|[Delete](../api/outlooktaskgroup-delete.md) | Нет |Удаление указанной группы задач Outlook. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|changeKey|Строка|Версия групповой задачи.|
|groupKey|Edm.Guid|Уникальный идентификатор GUID для группы задач.|
|id|Строка|Уникальная строка идентификатор группы задач. Только для чтения.|
|isDefaultGroup|Boolean.|Значение true, если группа задач является группу задач по умолчанию.|
|name|Строка|Имя группы задач.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|taskFolders|[outlookTaskFolder](outlooktaskfolder.md) коллекции| Коллекция папок задач в группе задач. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->