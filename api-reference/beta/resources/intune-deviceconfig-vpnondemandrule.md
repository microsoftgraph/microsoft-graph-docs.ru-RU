---
title: Тип ресурса vpnOnDemandRule
description: Определение правила по запросу VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8164d1c12aeb172120bb9803d7f3dd98366ec948
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421461"
---
# <a name="vpnondemandrule-resource-type"></a>Тип ресурса vpnOnDemandRule

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила по запросу VPN.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|идентификаторов SSID|Коллекция String|Сетевая служба задайте идентификаторов SSID.|
|dnsSearchDomains|Коллекция String|Домены поиска DNS.|
|probeUrl|String|URL-адрес для поиска. Если этот URL-адрес был успешно извлечь (возврат 200 код состояния HTTP) без в режиме одобрения администратором, соответствует данное правило.|
|action|[vpnOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Действие. Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|domainAction|[vpnOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Действие домена (возможно, только когда действие оценка подключения). Возможные значения: `connectIfNeeded`, `neverConnect`.|
|домены|Коллекция String|Домены (возможно, только когда действие оценка подключения).|
|probeRequiredUrl|String|Поиск необходимых URL-адреса (возможно, только если действие оценка подключения и DomainAction — это подключение при необходимости).|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```




