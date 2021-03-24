---
title: тип ресурса userExperienceAnalyticsCloudManagementDevicesSummary
description: Пользовательский интерфейс работает в любом месте сводки устройств облачного управления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0fb4e7d9a8ac5b2ab9c134d45c2e625a935b491
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146833"
---
# <a name="userexperienceanalyticscloudmanagementdevicessummary-resource-type"></a>тип ресурса userExperienceAnalyticsCloudManagementDevicesSummary

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пользовательский интерфейс работает в любом месте сводки устройств облачного управления.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|coManagedDeviceCount|Int32|Общее количество совместно управляемых устройств.|
|intuneDeviceCount|Int32|Количество устройств intune, которые не зарегистрированы автопилотом.|
|tenantAttachDeviceCount|Int32|Общее количество устройств присоединений клиента.|

## <a name="relationships"></a>Отношения
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




