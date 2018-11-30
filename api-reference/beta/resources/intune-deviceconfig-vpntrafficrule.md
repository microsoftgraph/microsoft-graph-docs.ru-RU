---
title: Тип ресурса vpnTrafficRule
description: Определение правила трафика через VPN.
ms.openlocfilehash: 564528cf0c0ae39785a2cc43dc800d8dbdf7d285
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076640"
---
# <a name="vpntrafficrule-resource-type"></a>Тип ресурса vpnTrafficRule

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определение правила трафика через VPN.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя.|
|протоколы|Int32|Протоколы (0-255). Допустимые значения от 0 до 255|
|localPortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md) коллекции|Диапазон портов для локального может устанавливаться только в том случае, если протокол TCP или UDP-ПОРТ (6 или 17). Эта коллекция может содержать не более 500 элементов.|
|remotePortRanges|[numberRange](../resources/intune-deviceconfig-numberrange.md) коллекции|Диапазон портов для удаленного может устанавливаться только в том случае, если протокол TCP или UDP-ПОРТ (6 или 17). Эта коллекция может содержать не более 500 элементов.|
|localAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) коллекции|Диапазон локальных адресов. Эта коллекция может содержать не более 500 элементов.|
|remoteAddressRanges|[iPv4Range](../resources/intune-shared-ipv4range.md) коллекции|Удаленный адрес диапазона. Эта коллекция может содержать не более 500 элементов.|
|appId|String|Идентификатор приложения, если правило трафика используется приложением.|
|Тип|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|Тип приложения, если правило трафика используется приложением. Возможные значения: `none`, `desktop`, `universal`.|
|routingPolicyType|[vpnTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|При запуске приложения указывает, следует ли включить разделенное туннелирование по этому маршруту. Возможные значения: `none`, `splitTunnel`, `forceTunnel`.|
|утверждения|String|Утверждений, связанный с этим правилом трафика.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnTrafficRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnTrafficRule",
  "name": "String",
  "protocols": 1024,
  "localPortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "remotePortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "localAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "remoteAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "appId": "String",
  "appType": "String",
  "routingPolicyType": "String",
  "claims": "String"
}
```





