---
title: Тип ресурса deviceExchangeAccessStateSummary
description: Сводка по состоянию доступа к Exchange для устройств
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39f944b7559abf72d144f5c1608ec4efec014530
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549120"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a>Тип ресурса deviceExchangeAccessStateSummary

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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





