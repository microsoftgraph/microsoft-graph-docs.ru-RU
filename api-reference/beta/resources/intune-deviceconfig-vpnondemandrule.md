---
title: Тип ресурса vpnOnDemandRule
description: Определение правила по запросу VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43908a55ff43c533d02ace629a80b96dc09c10ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955417"
---
# <a name="vpnondemandrule-resource-type"></a>Тип ресурса vpnOnDemandRule

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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

## <a name="relationships"></a>Связи
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





