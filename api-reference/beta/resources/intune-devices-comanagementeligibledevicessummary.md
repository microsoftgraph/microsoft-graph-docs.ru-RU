---
title: Тип ресурса Команажементелигибледевицессуммари
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4c7244bd594e38a8f129aa81389b159caff6b928
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214640"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a>Тип ресурса Команажементелигибледевицессуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|команажедкаунт|Int32|Количество устройств, уже Co-Managed|
|елигиблекаунт|Int32|Количество устройств, полностью доступных для Co-Management|
|елигиблебутнотазуреаджоинедкаунт|Int32|Количество устройств, подходящих для Co-Management, но еще не присоединенных к Azure Active Directory|
|нидсосупдатекаунт|Int32|Количество устройств, которые будут доступны Co-Management после обновления ОС|
|инелигиблекаунт|Int32|Количество устройств, доступных для Co-Management|

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




