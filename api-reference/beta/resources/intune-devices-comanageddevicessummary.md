---
title: тип ресурса comanagedDevicesSummary
description: Сводные данные для совместно управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 71c62ae41064199e55be9ed22b941017e2a2d6b3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784473"
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



