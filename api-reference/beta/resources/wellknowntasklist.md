---
title: тип ресурса wellKnownTaskList
description: Встроенный список задач, который нельзя переименовать или удалить.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0594ac7082680096ce17b3780780cc105e30606c
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61425162"
---
# <a name="wellknowntasklist-resource-type"></a>тип ресурса wellKnownTaskList

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Встроенный список задач, который нельзя переименовать или удалить. Для выполнения имеется два встроенных списка, **помеченные электронной** почтой и **списком** задач.

Этот ресурс поддерживает добавление данных в настраиваемые свойства в [качестве открытых расширений](/graph/extensibility-overview)

Наследует [из baseTaskList](../resources/basetasklist.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список wellKnownTaskLists](../api/tasks-list-lists.md)|[коллекция wellKnownTaskList](../resources/wellknowntasklist.md)|Получите список объектов [wellKnownTaskList](../resources/wellknowntasklist.md) и их свойств.|
|[Get wellKnownTaskList](../api/basetasklist-get.md)|[wellKnownTaskList](../resources/wellknowntasklist.md)|Ознакомьтесь с свойствами и отношениями объекта [wellKnownTaskList.](../resources/wellknowntasklist.md)|
|[Перечисление задач](../api/basetasklist-list-tasks.md)|[коллекция baseTask](../resources/basetask.md)|Получите ресурсы baseTask из свойства навигации задач.|
|[Создание baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Создайте новый объект baseTask.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя списка задач. Унаследованный от [baseTaskList](../resources/basetasklist.md).|
|id|Строка|Идентификатор списка задач, уникальный в почтовом ящике пользователя. Только для чтения. Унаследованный от [baseTaskList](../resources/basetasklist.md).|
|wellKnownListName|wellKnownListName_v2|Свойство, указывающее имя списка, если данный список хорошо известен. Допустимые значения: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|

### <a name="wellknownlistname-values"></a>значения wellknownListName
|Member|Описание|
|:---|:---|
|Нет| Созданный пользователем список.|
|defaultList| Встроенный **список задач.**|
|flaggedEmails| Встроенный **помеченный список электронной почты.** Задачи из помеченных электронных почт присутствуют в этом списке.|
|unknownFutureValue| Эволюционирующее значение sentinel. Не следует использовать.|

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

