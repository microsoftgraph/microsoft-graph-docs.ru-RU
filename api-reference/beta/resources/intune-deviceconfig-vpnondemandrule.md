---
title: тип ресурса vpnOnDemandRule
description: Определение правила VPN по требованию.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cd9999ee2fdae94c21848535e39dc93f88949839
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146102"
---
# <a name="vpnondemandrule-resource-type"></a>тип ресурса vpnOnDemandRule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила VPN по требованию.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ssids|Коллекция объектов string|Идентификаторы набора сетевых служб (SSID).|
|dnsSearchDomains|Коллекция объектов string|Домены поиска DNS.|
|probeUrl|String|URL-адрес для зонда. Если этот URL-адрес успешно извлечен (возврат кода состояния HTTP 200) без перенаправления, это правило совпадает.|
|action|[VPNOnDemandRuleConnectionAction](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Действие. Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|domainAction|[VPNOnDemandRuleConnectionDomainAction](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Действие домена (применимо только при оценке подключения Action). Возможные значения: `connectIfNeeded`, `neverConnect`.|
|домены|Коллекция объектов string|Домены (применимы только при оценке подключения Action).|
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



