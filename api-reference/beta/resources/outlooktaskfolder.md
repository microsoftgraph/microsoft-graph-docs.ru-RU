---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (коллекцию объектов outlookTask). '
author: angelgolfer-ms
ms.openlocfilehash: 505b6bf0fe172d701d85230b907727663595d9d3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306211"
---
# <a name="outlooktaskfolder-resource-type"></a>Тип ресурса outlookTaskFolder

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Папка, содержащая задачи Outlook (коллекцию объектов [outlookTask](outlooktask.md) ). 

В программе Outlook, группа задач по умолчанию, `My Tasks`, содержащая папки задач по умолчанию, `Tasks`, для почтового ящика пользователя. Невозможно переименовать или удалить эти группы по умолчанию задач и папки, но можно создать дополнительные группы задач и папок задач.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение outlookTaskFolder](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |Получите свойства и связи указанной папки задач Outlook.|
|[Создание outlookTask](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| Создание задачи Outlook в папке указанной задачи.|
|[Перечисление задач](../api/outlooktaskfolder-list-tasks.md) |[outlookTask](outlooktask.md) коллекции| Получите все задачи Outlook в указанной папке.|
|[обновление](../api/outlooktaskfolder-update.md). | [outlookTaskFolder](outlooktaskfolder.md)   |Обновление для записи свойств папки задач Outlook. |
|[Delete](../api/outlooktaskfolder-delete.md) | Нет |Удаление указанной папки задач Outlook.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |Создайте один или несколько расширенных свойств одно значение в новую или существующую папку задач Outlook.   |
|[Получение папки задач с одним значением расширенные свойства](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Получение папки задач Outlook, которые содержат одно значение расширенные свойства с помощью `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | Создайте один или несколько расширенных свойств Многозначный в новую или существующую папку задач Outlook.  |
|[Получение папки задач с несколькими значениями расширенные свойства](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Получение папки задач Outlook, которая содержит свойство расширенного Многозначный с помощью `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|changeKey|Строка|Версия папки задач.|
|id|Строка|Идентификатор папки задач, уникальные в почтовом ящике пользователя. Только для чтения.|
|isDefaultFolder|Boolean.|Значение true, если папка является папки задач по умолчанию.|
|name|Строка|Имя папки задач.|
|parentGroupKey|Guid|Уникальный идентификатор GUID для родительской папки задач группы.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)|Коллекция Многозначный расширенные свойства для папки задач. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)|Коллекция расширенные свойства одно значение, определенное для папки задач. Только для чтения. Допускается значение null.|
|tasks|[outlookTask](outlooktask.md) коллекции|Задачи в этой папке задач. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->