---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c69e0ae9528a31ec7512348931e9a6eb0b1dd7b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838943"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>Тип ресурса configurationManagerClientEnabledFeatures

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Включенные клиентом функции диспетчера конфигураций
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|inventory|Boolean|Управляет ли Intune данными инвентаризации|
|modernApps|Boolean|Управляет ли Intune современным приложением|
|resourceAccess|Boolean|Управляет ли Intune доступом к ресурсам|
|deviceConfiguration|Boolean|Управляет ли Intune конфигурацией устройства|
|compliancePolicy|Boolean|Управляется ли Intune политикой соответствия требованиям|
|windowsUpdateForBusiness|Boolean|Управляет ли Intune Центром обновления Windows для бизнеса|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```



