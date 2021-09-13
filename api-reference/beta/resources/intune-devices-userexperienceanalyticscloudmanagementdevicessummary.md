---
title: тип ресурса userExperienceAnalyticsCloudManagementDevicesSummary
description: Пользовательский интерфейс работает в любом месте сводки устройств облачного управления.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 567a3743110111e5f013c6197bef1729de6a27d0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59141138"
---
# <a name="userexperienceanalyticscloudmanagementdevicessummary-resource-type"></a>тип ресурса userExperienceAnalyticsCloudManagementDevicesSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пользовательский интерфейс работает в любом месте сводки устройств облачного управления.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|coManagedDeviceCount|Int32|Общее количество совместно управляемых устройств.|
|intuneDeviceCount|Int32|Количество устройств intune, которые не зарегистрированы автопилотом.|
|tenantAttachDeviceCount|Int32|Общее количество устройств присоединений клиента.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
  "coManagedDeviceCount": 1024,
  "intuneDeviceCount": 1024,
  "tenantAttachDeviceCount": 1024
}
```



