---
title: тип ресурса comanagementEligibleDevicesSummary
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14585d673c1f101c7204bffe4f1d2f3ede632c88d8c6c88a3218b3be4bb67e6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54179034"
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




