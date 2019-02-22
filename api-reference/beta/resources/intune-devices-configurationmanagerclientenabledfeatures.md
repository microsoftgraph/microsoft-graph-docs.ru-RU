---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed376bc616c26f1ad6e8a3ea06d3898c051e8d0b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148778"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>Тип ресурса configurationManagerClientEnabledFeatures

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|Ендпоинтпротектион|Логический|Управляет ли Intune Endpoint Protection|
|Оффицеаппс|Логический|Управляет ли Intune приложением Office|

## <a name="relationships"></a>Отношения
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




