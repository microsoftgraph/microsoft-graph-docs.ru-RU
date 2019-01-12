---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dc1b994615c89b1a6e73785a5ebcdc85f0638953
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987595"
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



