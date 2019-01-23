---
title: Тип ресурса vpnTrafficRule
description: Определение правила трафика через VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b28d26356eea113f267c4eb0499f9600671f114
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415287"
---
# <a name="vpntrafficrule-resource-type"></a>Тип ресурса vpnTrafficRule

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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

## <a name="relationships"></a>Отношения
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




