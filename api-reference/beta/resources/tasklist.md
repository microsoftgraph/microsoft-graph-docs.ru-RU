---
title: тип ресурса taskList
description: Представляет список, созданный пользователем в Microsoft To Do, содержащий один или несколько ресурсов Task.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 070a427de0531e5ce715e31c91b2ffddd6be4576
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61425196"
---
# <a name="tasklist-resource-type"></a>тип ресурса taskList

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет список, созданный пользователем в Microsoft To Do, содержащий один или несколько [ресурсов Task.](./task.md) 

Этот ресурс поддерживает
* Добавление данных в настраиваемые свойства в качестве [открытых расширений](/graph/extensibility-overview)
* Использование [delta-запроса](/graph/delta-query-overview) для отслеживания дополнительных дополнений, удалений и обновлений.

Наследует [из baseTaskList](../resources/basetasklist.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список списков задач](../api/tasks-list-lists.md)|[коллекция taskList](../resources/tasklist.md)|Получите список объектов [taskList](../resources/tasklist.md) и их свойств.|
|[Get taskList](../api/basetasklist-get.md)|[taskList](../resources/tasklist.md)|Ознакомьтесь с свойствами и отношениями объекта [taskList.](../resources/tasklist.md)|
|[Обновление списка задач](../api/tasklist-update.md)|[taskList](../resources/tasklist.md)|Обновление свойств объекта [taskList.](../resources/tasklist.md)|
|[Удаление списка задач](../api/tasklist-delete.md)|Нет|Удаляет объект [taskList.](../resources/tasklist.md)|
|[Перечисление задач](../api/basetasklist-list-tasks.md)|[коллекция baseTask](../resources/basetask.md)|Получите ресурсы baseTask из свойства навигации задач.|
|[Создание baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Создайте новый объект baseTask.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя списка задач. Унаследованный от [baseTaskList](../resources/basetasklist.md).|
|id|Строка|Идентификатор списка задач, уникальный в почтовом ящике пользователя. Только для чтения. Унаследованный от [baseTaskList](../resources/basetasklist.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|extensions|Коллекция [extension](../resources/extension.md)|Коллекция открытых расширений, определенных для списка задач. Допускается значение null. Унаследованный от [baseTaskList](../resources/basetasklist.md)|
|tasks|[коллекция baseTask](../resources/basetask.md)|Задачи в этом списке задач. Только для чтения. Допускается значение null. Унаследованный от [baseTaskList](../resources/basetasklist.md)|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.taskList",
  "baseType": "microsoft.graph.baseTaskList",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taskList",
  "displayName": "String",
  "id": "String (identifier)"
}
```

