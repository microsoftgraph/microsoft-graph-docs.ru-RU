---
title: тип ресурса userExperienceAnalyticsCloudIdentityDevicesSummary
description: Аналитика пользовательских интерфейсов работает из любого сводки облачных устройств удостоверений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d138f6a64cce1992b1416369660899ac02ec9a3f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58810276"
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



