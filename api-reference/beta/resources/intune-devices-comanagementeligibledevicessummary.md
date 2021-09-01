---
title: тип ресурса comanagementEligibleDevicesSummary
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c4950dd620adb21c9ebdbb45b7c1acbd3380dc70
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806630"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a>тип ресурса comanagementEligibleDevicesSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|comanagedCount|Int32|Количество устройств, уже Co-Managed|
|eligibleCount|Int32|Количество устройств, полностью подходящих для Co-Management|
|eligibleButNotAzureAdJoinedCount|Int32|Количество устройств, имеющих право на Co-Management, но еще не присоединились к Azure Active Directory|
|needsOsUpdateCount|Int32|Количество устройств, которые будут иметь право на Co-Management после обновления ОС|
|ineligibleCount|Int32|Количество устройств, не допустимых для Co-Management|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagementEligibleDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevicesSummary",
  "comanagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAzureAdJoinedCount": 1024,
  "needsOsUpdateCount": 1024,
  "ineligibleCount": 1024
}
```



