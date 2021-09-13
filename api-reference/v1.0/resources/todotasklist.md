---
title: тип ресурса todoTaskList
description: Список в Microsoft To Do, содержащий один или несколько ресурсов todoTask.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 24d98f5fa351db7aed56a637eee2d606d42fb504
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134292"
---
# <a name="todotasklist-resource-type"></a>тип ресурса todoTaskList

Пространство имен: microsoft.graph

Список в Microsoft To Do, содержащий один или несколько [ресурсов todoTask.](./todotask.md) 

В To Do есть встроенные списки задач,  такие как помеченные  электронные почты и задачи, которые нельзя переименовать или удалить.  Однако можно создать дополнительные списки задач.

Этот ресурс поддерживает
* Добавление данных в настраиваемые свойства в качестве [открытых расширений](/graph/extensibility-overview)
* Использование [delta-запроса](/graph/delta-query-overview) для отслеживания дополнительных дополнений, удалений и обновлений.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление списков](../api/todo-list-lists.md) | Коллекция [todoTaskList](todotasklist.md) | Получите весь [todoTaskList](todotasklist.md) в почтовом ящике пользователя. |
|[Создание todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Создайте [todoTaskList](todotasklist.md) в почтовом ящике пользователя. |
|[Получить список задач](../api/todotasklist-get.md)|[todoTaskList](todotasklist.md)|Ознакомьтесь с свойствами и отношениями указанного [todoTaskList.](todotasklist.md)|
|[Обновление списка задач](../api/todotasklist-update.md)|[todoTaskList](todotasklist.md)| Обновим ритабельные свойства указанного [todoTaskList.](todotasklist.md)|
|[Удаление списка задач](../api/todotasklist-delete.md)|Нет| Удаление указанного [todoTaskList](todotasklist.md) .|
|[Перечисление задач](../api/todotasklist-list-tasks.md)|Коллекция [todoTask](todotask.md)|Получение всех ресурсов [todoTask](todotask.md) в указанном списке.|
|[Создание задачи](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Создание [todoTask](todotask.md) в указанном списке задач.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя списка задач.|
|id|String| Идентификатор списка задач, уникальный в почтовом ящике пользователя. Только для чтения. Унаследованный от [сущности](entity.md)|
|isOwner|Boolean| True, если пользователь является владельцем данного списка задач.|
|IsShared|Boolean| True, если список задач совместно с другими пользователями|
|wellknownListName|wellknownListName| Свойство, указывающее имя списка, если данный список хорошо известен. Возможные значения: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|

### <a name="wellknownlistname-values"></a>значения wellknownListName
|Member|Описание|
|:---|:---|
|Нет| Созданный пользователем список.|
|defaultList| Встроенный список **задач.**|
|flaggedEmails| Встроенный список **электронной почты с флагами.** Задачи из помеченных электронных почт присутствуют в этом списке.|
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|extensions|Коллекция [extension](extension.md)| Коллекция открытых расширений, определенных для списка задач. Допускается значение null.|
|tasks|Коллекция [todoTask](todotask.md)|Задачи в этом списке задач. Только для чтения. Допускается значение null.|

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



