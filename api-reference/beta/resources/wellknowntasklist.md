---
title: Тип ресурса wellKnownTaskList
description: Встроенный список задач, который нельзя переименовать или удалить.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0391983a88f91255779b994221fed195ad890c7e
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821199"
---
# <a name="wellknowntasklist-resource-type-deprecated"></a>Тип ресурса wellKnownTaskList (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

Встроенный список задач, который нельзя переименовать или удалить. Список дел есть два встроенных списка: **помеченные сообщения** электронной почты и **задачи**.

Этот ресурс поддерживает добавление данных в пользовательские свойства в виде [открытых расширений.](/graph/extensibility-overview)

Наследуется [от baseTaskList](../resources/basetasklist.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов wellKnownTaskList](../api/tasks-list-lists.md)|[Коллекция wellKnownTaskList](../resources/wellknowntasklist.md)|Получение списка объектов [wellKnownTaskList](../resources/wellknowntasklist.md) и их свойств.|
|[Получение wellKnownTaskList](../api/basetasklist-get.md)|[wellKnownTaskList](../resources/wellknowntasklist.md)|Чтение свойств и связей объекта [wellKnownTaskList](../resources/wellknowntasklist.md) .|
|[Перечисление задач](../api/basetasklist-list-tasks.md)|[Коллекция baseTask](../resources/basetask.md)|Получите ресурсы baseTask из свойства навигации задач.|
|[Создание baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Создайте объект baseTask.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя списка задач. Наследуется [от baseTaskList](../resources/basetasklist.md).|
|id|Строка|Идентификатор списка задач, уникальный в почтовом ящике пользователя. Только для чтения. Наследуется [от baseTaskList](../resources/basetasklist.md).|
|wellKnownListName|wellKnownListName_v2|Свойство, указывающее имя списка, если данный список является известным списком. Допустимые значения: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|

### <a name="wellknownlistname-values"></a>Значения wellknownListName
|Member|Описание|
|:---|:---|
|Нет| Созданный пользователем список.|
|defaultList| Список **встроенных задач** .|
|flaggedEmails| Встроенный **помеченный список электронной почты** . Задачи из помеченных сообщений электронной почты присутствуют в этом списке.|
|unknownFutureValue| Значение sentinel для развиваемого перечисления. Не следует использовать.|

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
  "@odata.type": "microsoft.graph.wellKnownTaskList",
  "baseType": "microsoft.graph.baseTaskList",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.wellKnownTaskList",
  "displayName": "String",
  "id": "String (identifier)",
  "wellKnownListName": "String"
}
```

