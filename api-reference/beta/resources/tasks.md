---
title: тип ресурса задач
description: Представляет службу задач To Do, доступную пользователю
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a354c71449b5934ae0479eb1833258e394d6987e
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61425180"
---
# <a name="tasks-resource-type"></a>тип ресурса задач

Пространство имен: microsoft.graph

Представляет службы выполнения задач, доступные пользователю.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление списков](../api/tasks-list-lists.md)|[коллекция baseTaskList](../resources/basetasklist.md)|Получите ресурсы baseTaskList из свойства навигации списков.|
|[Создание списка задач](../api/tasks-post-lists.md)|[taskList](../resources/basetasklist.md)|Создайте новый объект baseTaskList.|

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|alltasks|[коллекция baseTask](../resources/basetask.md)|Все задачи в почтовом ящике пользователей.|
|lists|[коллекция baseTaskList](../resources/basetasklist.md)|Списки задач в почтовом ящике пользователей.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tasks",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tasks",
  "id": "String (identifier)"
}
```

