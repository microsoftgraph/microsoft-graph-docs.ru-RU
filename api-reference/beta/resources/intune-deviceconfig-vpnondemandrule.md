---
title: тип ресурса vpnOnDemandRule
description: Определение правила VPN по требованию.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4bcf5b6331777600bb847dc2aad4a921c2745702
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58815101"
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
|probeRequiredUrl|Строка|Url-адрес Probe Required (применим только при оценке подключения Action и подключения DomainAction).|

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



