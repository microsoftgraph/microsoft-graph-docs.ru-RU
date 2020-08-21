---
title: Тип ресурса todoTaskList
description: Список в Microsoft To Do, содержащий один или несколько ресурсов todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d34f90329fc6ca4d5e12ff2f2b191819b88f895b
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850045"
---
# <a name="todotasklist-resource-type"></a>Тип ресурса todoTaskList

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список в Microsoft To Do, содержащий один или несколько [ресурсов todoTask.](./todotask.md) 

В задачах есть встроенные списки задач, такие как отмеченные **сообщения электронной** почты и **задачи,** которые нельзя переименовать или удалить.  Однако можно создавать дополнительные списки задач.

Этот ресурс поддерживает
* Добавление данных к настраиваемым свойствам в качестве [открытых расширений](/graph/extensibility-overview)
* Использование [разностного запроса](/graph/delta-query-overview) для отслеживания добавлений, удалений и обновлений.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Списки](../api/todo-list-lists.md) | [Коллекция todoTaskList](todotasklist.md) | Получение [всех объектов todoTaskList](todotasklist.md) в почтовом ящике пользователя. |
|[Создание объекта todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Создание [списка todoTaskList](todotasklist.md) в почтовом ящике пользователя. |
|[Вывод списка задач](../api/todotasklist-get.md)|[todoTaskList](todotasklist.md)|Чтение свойств и связей указанного [объекта todoTaskList.](todotasklist.md)|
|[Обновление списка задач](../api/todotasklist-update.md)|[todoTaskList](todotasklist.md)| Обновление записываемых свойств [указанного объекта todoTaskList.](todotasklist.md)|
|[Удаление списка задач](../api/todotasklist-delete.md)|Нет| Удаление указанного [объекта todoTaskList.](todotasklist.md)|
|[Перечисление задач](../api/todotasklist-list-tasks.md)|[Коллекция todoTask](todotask.md)|Получение всех [ресурсов todoTask](todotask.md) в указанном списке.|
|[Создание задачи](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Создание объекта [todoTask](todotask.md) в указанном списке задач.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя списка задач.|
|id|String| Идентификатор списка задач, уникальный в почтовом ящике пользователя. Только для чтения. Наследуется от [сущности](entity.md)|
|isOwner|Boolean| Имеет значение true, если пользователь является владельцем заданного списка задач.|
|IsShared|Boolean| Имеет значение True, если доступ к списку задач предоставлен другим пользователям|
|wellknownListName|wellknownListName| Свойство, указывающее имя известного списка, если данный список является известным. Возможные значения: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|extensions|Коллекция объектов [extension](extension.md)| Коллекция открытых расширений, определенных для списка задач. Допускается значение null.|
|tasks|[Коллекция todoTask](todotask.md)|Задачи, перечисленные в этом списке задач. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTaskList",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "String (identifier)",
  "displayName": "String",
  "isOwner": "Boolean",
  "isShared": "Boolean",
  "wellknownListName": "String"
}
```

