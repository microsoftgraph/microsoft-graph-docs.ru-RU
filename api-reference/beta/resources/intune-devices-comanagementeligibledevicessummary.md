---
title: Тип ресурса Команажементелигибледевицессуммари
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 55df0591dfcbabd997dfda1bb07dbd116c14dcbe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793453"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a>Тип ресурса Команажементелигибледевицессуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|команажедкаунт|Int32|Количество устройств, для которых уже осуществляется совместное управление|
|елигиблекаунт|Int32|Количество устройств, полностью доступных для совместного управления|
|елигиблебутнотазуреаджоинедкаунт|Int32|Количество устройств, подходящих для совместного управления, но еще не включенных в Azure Active Directory|
|нидсосупдатекаунт|Int32|Количество устройств, которые будут доступны для совместного управления после обновления ОС|
|инелигиблекаунт|Int32|Количество устройств, подходящих для совместного управления|

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



