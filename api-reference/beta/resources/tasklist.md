---
title: Тип ресурса taskList
description: Представляет список, созданный пользователем в Список дел Microsoft, который содержит один или несколько ресурсов задачи.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bee831640d6ba392f359a1ad1dbd70b088733141
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819361"
---
# <a name="tasklist-resource-type-deprecated"></a>Тип ресурса taskList (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

Представляет список, созданный пользователем в Список дел Microsoft, который содержит один или [несколько ресурсов](./task.md) задачи. 

Этот ресурс поддерживает следующее:
* Добавление данных в пользовательские свойства в виде [открытых расширений](/graph/extensibility-overview)
* Использование [разностного](/graph/delta-query-overview) запроса для отслеживания добавочных дополнений, удалений и обновлений.

Ресурс **taskList** наследуется от [baseTaskList](../resources/basetasklist.md).
Его содержимое типа ресурса **задачи наследуется** от [baseTask](../resources/basetask.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление списков задач](../api/tasks-list-lists.md)|[Коллекция taskList](../resources/tasklist.md)|Получение списка объектов [taskList](../resources/tasklist.md) и их свойств.|
|[Получение списка задач](../api/basetasklist-get.md)|[Tasklist](../resources/tasklist.md)|Чтение свойств и связей объекта [taskList](../resources/tasklist.md) .|
|[Обновление списка задач](../api/tasklist-update.md)|[Tasklist](../resources/tasklist.md)|Обновление свойств объекта [taskList](../resources/tasklist.md) .|
|[Удаление списка задач](../api/tasklist-delete.md)|Нет|Удаляет объект [taskList](../resources/tasklist.md) .|
|[Перечисление задач](../api/basetasklist-list-tasks.md)|[Коллекция baseTask](../resources/basetask.md)|Получите ресурсы baseTask из свойства навигации задач.|
|[Создание baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Создайте объект baseTask.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя списка задач. Наследуется [от baseTaskList](../resources/basetasklist.md).|
|id|Строка|Идентификатор списка задач, уникальный в почтовом ящике пользователя. Только для чтения. Наследуется [от baseTaskList](../resources/basetasklist.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|extensions|Коллекция объектов [extension](../resources/extension.md)|Коллекция открытых расширений, определенных для списка задач. Допускается значение null. Наследуется от [baseTaskList](../resources/basetasklist.md)|
|tasks|[Коллекция baseTask](../resources/basetask.md)|Задачи в этом списке задач. Только для чтения. Допускается значение null. Наследуется от [baseTaskList](../resources/basetasklist.md)|

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

