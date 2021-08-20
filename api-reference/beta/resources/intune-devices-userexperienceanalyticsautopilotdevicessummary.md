---
title: тип ресурса userExperienceAnalyticsAutopilotDevicesSummary
description: Сводка аналитики пользовательского опыта о том, что устройства не готовы к автопилоту Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6cf2eafac549b0627a9f6ea6557199a3aa0eb61f91e05e0720b2039b2df6814f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54133224"
---
# <a name="userexperienceanalyticsautopilotdevicessummary-resource-type"></a>тип ресурса userExperienceAnalyticsAutopilotDevicesSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка аналитики пользовательского опыта о том, что устройства не готовы к автопилоту Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|devicesNotAutopilotRegistered|Int32|Количество устройств intune, которые не зарегистрированы автопилотом.|
|devicesWithoutAutopilotProfileAssigned|Int32|Количество устройств intune, не назначенное профилем автопилота.|

## <a name="relationships"></a>Связи
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




