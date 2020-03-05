---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2dfae041f1aab4c4ea74490d372350c5c0c2087b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528685"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>Тип ресурса configurationManagerClientEnabledFeatures

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Включенные клиентом функции диспетчера конфигураций

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|inventory|Логический|Управляет ли Intune данными инвентаризации|
|modernApps|Логический|Управляет ли Intune современным приложением|
|resourceAccess|Логический|Управляет ли Intune доступом к ресурсам|
|deviceConfiguration|Логический|Управляет ли Intune конфигурацией устройства|
|compliancePolicy|Логический|Управляется ли Intune политикой соответствия требованиям|
|windowsUpdateForBusiness|Boolean|Управляет ли Intune Центром обновления Windows для бизнеса|
|ендпоинтпротектион|Логический|Управляет ли Intune Endpoint Protection|
|оффицеаппс|Логический|Управляет ли Intune приложением Office|

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
  "windowsUpdateForBusiness": true,
  "endpointProtection": true,
  "officeApps": true
}
```



