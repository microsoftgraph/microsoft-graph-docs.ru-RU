---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25bc1fe1592b2aa1a1f0cde1b4bf45b6092a36d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407038"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a>Тип ресурса deviceExchangeAccessStateSummary

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по состоянию доступа к Exchange для устройств

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedDeviceCount|Int32|Общее количество устройств с состоянием доступа к Exchange "Разрешено".|
|blockedDeviceCount|Int32|Общее количество устройств с состоянием доступа к Exchange "Заблокировано".|
|quarantinedDeviceCount|Int32|Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".|
|unknownDeviceCount|Int32|Общее количество устройств с состоянием доступа к Exchange "Неизвестно".|
|unavailableDeviceCount|Int32|Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```







