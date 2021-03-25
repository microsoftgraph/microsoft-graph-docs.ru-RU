---
title: тип ресурса userExperienceAnalyticsAutopilotDevicesSummary
description: Сводка аналитики пользовательского опыта о том, что устройства не готовы к автопилоту Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 27faa3cf52ba5b0118137b1d64c63552d9e4f127
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159468"
---
# <a name="userexperienceanalyticsautopilotdevicessummary-resource-type"></a>тип ресурса userExperienceAnalyticsAutopilotDevicesSummary

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка аналитики пользовательского опыта о том, что устройства не готовы к автопилоту Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|devicesNotAutopilotRegistered|Int32|Количество устройств intune, которые не зарегистрированы автопилотом.|
|devicesWithoutAutopilotProfileAssigned|Int32|Количество устройств intune, не назначенное профилем автопилота.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
  "devicesNotAutopilotRegistered": 1024,
  "devicesWithoutAutopilotProfileAssigned": 1024
}
```




