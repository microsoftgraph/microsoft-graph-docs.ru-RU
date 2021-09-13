---
title: тип ресурса customUpdateTimeWindow
description: Настраиваемое окно времени обновления
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4653237f56ef0f00d7c22e2e2c09bfb694cd8cca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146704"
---
# <a name="customupdatetimewindow-resource-type"></a>тип ресурса customUpdateTimeWindow

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настраиваемое окно времени обновления

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|startDay|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|Начало дня окне времени. Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|endDay|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|Конец дня окне времени. Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|startTime|TimeOfDay|Время начала окне времени|
|endTime|TimeOfDay|Время окончания окне времени|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customUpdateTimeWindow"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customUpdateTimeWindow",
  "startDay": "String",
  "endDay": "String",
  "startTime": "String (time of day)",
  "endTime": "String (time of day)"
}
```



