---
title: тип ресурса userExperienceAnalyticsCloudIdentityDevicesSummary
description: Аналитика пользовательских интерфейсов работает из любого сводки облачных устройств удостоверений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89f8f4fde6b0fc075c0f8dffe07406468cca4bfb
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259324"
---
# <a name="userexperienceanalyticscloudidentitydevicessummary-resource-type"></a>тип ресурса userExperienceAnalyticsCloudIdentityDevicesSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Аналитика пользовательских интерфейсов работает из любого сводки облачных устройств удостоверений.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceWithoutCloudIdentityCount|Int32|Количество устройств, не относяющихся к облачной идентификации.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudIdentityDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCloudIdentityDevicesSummary",
  "deviceWithoutCloudIdentityCount": 1024
}
```




