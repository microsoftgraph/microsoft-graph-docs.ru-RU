---
title: тип ресурса comanagementEligibleDevicesSummary
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90f4cb5f33b0ea1c260d6b6acaffac46d3e08434
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111042"
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



