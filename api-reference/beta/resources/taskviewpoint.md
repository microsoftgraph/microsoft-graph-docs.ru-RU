---
title: тип ресурса taskViewpoint
description: Содержит личные свойства задачи"
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 36590611168f34335795f6200bfe06e09436c1c0
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451551"
---
# <a name="taskviewpoint-resource-type"></a>тип ресурса taskViewpoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит личные свойства [задачи](task.md). При совместном использовании или назначении **задачи** другие пользователи не будут видеть эти свойства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата и время оповещения о **возникаемой** задаче.|
|categories|Коллекция String|Категории, связанные с задачей. Каждая категория соответствует свойству **displayName** объекта [outlookCategory](../resources/outlookcategory.md), определенному пользователем.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.taskViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taskViewpoint",
  "reminderDatetime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "categories": ["string"]
}
```

