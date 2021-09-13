---
title: тип ресурса userExperienceAnalyticsCloudIdentityDevicesSummary
description: Аналитика пользовательских интерфейсов работает из любого сводки облачных устройств удостоверений.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4042ae6b67e5e5ba1ea8e493b71aeb013121227
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59141145"
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



