---
title: тип ресурса userExperienceAnalyticsAutopilotDevicesSummary
description: Сводка аналитики пользовательского опыта о том, что устройства не готовы к автопилоту Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 95d93e809d72df3e2e224c77d6691f5c801e376f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806112"
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
|totalWindows10DevicesWithoutTenantAttached|Int32|Количество устройств с Windows 10, которые являются Intune и Comanaged.|

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
  "devicesWithoutAutopilotProfileAssigned": 1024,
  "totalWindows10DevicesWithoutTenantAttached": 1024
}
```



