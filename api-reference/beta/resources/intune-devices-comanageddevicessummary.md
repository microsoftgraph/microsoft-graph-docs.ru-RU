---
title: тип ресурса comanagedDevicesSummary
description: Сводные данные для совместно управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62c0f9dbf3600b32df3a1acbc2b7c58ec86b2727d6f6c5d22317772d6e3fde4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54219865"
---
# <a name="comanageddevicessummary-resource-type"></a>тип ресурса comanagedDevicesSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводные данные для совместно управляемых устройств

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|inventoryCount|Int32|Количество устройств с качнулся инвентаризации. Это свойство доступно только для чтения.|
|compliancePolicyCount|Int32|Количество устройств с помощью CompliancePolicy перемахнуло. Это свойство доступно только для чтения.|
|resourceAccessCount|Int32|Количество устройств с помощью ResourceAccess перемахнуло. Это свойство доступно только для чтения.|
|configurationSettingsCount|Int32|Количество устройств с конфигурациейSettings качнулся над. Это свойство доступно только для чтения.|
|windowsUpdateForBusinessCount|Int32|Количество устройств с WindowsUpdateForBusiness перемахнулось. Это свойство доступно только для чтения.|
|endpointProtectionCount|Int32|Количество устройств с endpointProtection, качнулся над. Это свойство доступно только для чтения.|
|modernAppsCount|Int32|Количество устройств с modernApps перемахнулись. Это свойство доступно только для чтения.|
|officeAppsCount|Int32|Количество устройств с качнулся Над OfficeApps. Это свойство доступно только для чтения.|
|totalComanagedCount|Int32|Количество Co-Managed устройств. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagedDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagedDevicesSummary",
  "inventoryCount": 1024,
  "compliancePolicyCount": 1024,
  "resourceAccessCount": 1024,
  "configurationSettingsCount": 1024,
  "windowsUpdateForBusinessCount": 1024,
  "endpointProtectionCount": 1024,
  "modernAppsCount": 1024,
  "officeAppsCount": 1024,
  "totalComanagedCount": 1024
}
```




