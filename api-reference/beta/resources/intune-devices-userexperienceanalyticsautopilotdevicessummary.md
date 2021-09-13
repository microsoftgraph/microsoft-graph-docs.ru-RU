---
title: тип ресурса userExperienceAnalyticsAutopilotDevicesSummary
description: Сводка аналитики пользовательского опыта о том, что устройства не готовы к автопилоту Windows.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3ec2b055c67a03f65acdd306f0f1f49b30f27663
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040052"
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



