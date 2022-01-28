---
title: тип ресурса teamworkDateTimeConfiguration
description: Представляет сведения о дате и времени конфигурации для Microsoft Teams устройства с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 489c76f123124aa0b6d6023d5a21dbc780e88a13
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262510"
---
# <a name="teamworkdatetimeconfiguration-resource-type"></a>тип ресурса teamworkDateTimeConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о дате и времени конфигурации Microsoft Teams устройства с [включенной поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|dateFormat|String|Формат даты для устройства.|
|officeHoursEndTime|TimeOfDay|Время отключения устройства.|
|officeHoursStartTime|TimeOfDay|Время дня, когда устройство включено.|
|timeFormat|String|Формат времени для устройства.|
|timeZone|String|Часовой пояс, в который применяются часы работы.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDateTimeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDateTimeConfiguration",
  "dateFormat": "String",
  "officeHoursEndTime": "String (time of day)",
  "officeHoursStartTime": "String (time of day)",
  "timeFormat": "String",
  "timeZone": "String"
}
```

