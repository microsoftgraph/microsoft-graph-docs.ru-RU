---
title: Тип ресурса Тодотасклист
description: Список в Майкрософт для этого содержит один или несколько ресурсов Тодотаск.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0523404e836223f8a59e191d1e7040a279433795
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073385"
---
# <a name="todotasklist-resource-type"></a>Тип ресурса Тодотасклист

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список в Майкрософт для этого содержит один или несколько ресурсов [тодотаск](./todotask.md) . 

В этом случае есть встроенные списки задач, такие как **помеченные сообщения электронной почты** и **задачи** , которые не могут быть переименованы или удалены.  Тем не менее, вы можете создавать дополнительные списки задач.

Этот ресурс поддерживает
* Добавление данных к настраиваемым свойствам в виде [открытых расширений](/graph/extensibility-overview)
* Использование [запроса изменений](/graph/delta-query-overview) для отслеживания добавочных дополнений, удалений и обновлений.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление списков](../api/todo-list-lists.md) | Коллекция [todoTaskList](todotasklist.md) | Получение всех [тодотасклист](todotasklist.md) в почтовом ящике пользователя. |
|[Создание Тодотасклист](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Создайте [тодотасклист](todotasklist.md) в почтовом ящике пользователя. |
|[Получение списка задач](../api/todotasklist-get.md)|[todoTaskList](todotasklist.md)|Чтение свойств и связей указанного [тодотасклист](todotasklist.md).|
|[Обновление списка задач](../api/todotasklist-update.md)|[todoTaskList](todotasklist.md)| Обновление свойств, доступных для записи, для указанного [тодотасклист](todotasklist.md).|
|[Удаление списка задач](../api/todotasklist-delete.md)|Нет| Удаление указанного [тодотасклист](todotasklist.md) .|
|[Перечисление задач](../api/todotasklist-list-tasks.md)|Коллекция [тодотаск](todotask.md)|Получение всех ресурсов [тодотаск](todotask.md) в указанном списке.|
|[Создание задачи](../api/todotasklist-post-tasks.md)|[тодотаск](todotask.md)| Создание [тодотаск](todotask.md) в указанном списке задач.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя списка задач.|
|id|String| Идентификатор списка задач, уникальный в почтовом ящике пользователя. Только для чтения. Наследуется от [объекта](entity.md)|
|Владелец|Boolean| Значение true, если пользователь является владельцем данного списка задач.|
|IsShared|Boolean| True, если список задач открыт для совместного использования с другими пользователями|
|веллкновнлистнаме|веллкновнлистнаме| Свойство, указывающее известное имя списка, если заданный список представляет собой известный список. Возможные значения: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|extensions|Коллекция [extension](extension.md)| Коллекция открытых расширений, определенных для списка задач. Допускается значение null.|
|tasks|Коллекция [тодотаск](todotask.md)|Задачи в этом списке задач. Только для чтения. Допускается значение null.|

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



