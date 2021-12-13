---
title: тип ресурса personalTaskProperties
description: Содержит личные свойства задачи"
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 56007de468b5fd06998b94f5b5256cfb170ba127
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61425183"
---
# <a name="personaltaskproperties-resource-type"></a>тип ресурса personalTaskProperties

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит личные свойства [задачи.](task.md) При совместном использовании или назначении **задачи** эти свойства не будут рассматриваться другими пользователями.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|reminderDatetime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата и время оповещения о **возникаемой** задаче.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.personalTaskProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personalTaskProperties",
  "reminderDatetime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  }
}
```

