---
title: тип ресурса vpnOnDemandRule
description: Определение правила VPN по требованию.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 71bfbf09f9fcb8de63956855ec3c13fed60a2d604d1a3b1601c1b2f6007e8867
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54131180"
---
# <a name="vpnondemandrule-resource-type"></a>тип ресурса vpnOnDemandRule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила VPN по требованию.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ssids|Коллекция String|Идентификаторы набора сетевых служб (SSID).|
|dnsSearchDomains|Коллекция String|Домены поиска DNS.|
|probeUrl|Строка|URL-адрес для зонда. Если этот URL-адрес успешно извлечен (возврат кода состояния HTTP 200) без перенаправления, это правило совпадает.|
|action|[VPNOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Действие. Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|domainAction|[VPNOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Действие домена (применимо только при оценке подключения Action). Возможные значения: `connectIfNeeded`, `neverConnect`.|
|домены|Коллекция String|Домены (применимы только при оценке подключения Action).|
|probeRequiredUrl|String|Url-адрес Probe Required (применим только при оценке подключения Action и подключения DomainAction).|

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




