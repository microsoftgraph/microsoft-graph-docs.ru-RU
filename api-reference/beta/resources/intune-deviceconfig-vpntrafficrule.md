---
title: тип ресурса vpnTrafficRule
description: Определение правила трафика VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d62c0d2357b3d46cce5654d460853ad063a351ad
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800055"
---
# <a name="vpntrafficrule-resource-type"></a>тип ресурса vpnTrafficRule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила трафика VPN.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя.|
|протоколы|Int32|Протоколы (0-255). Допустимые значения от 0 до 255|
|localPortRanges|[коллекция numberRange](../resources/intune-deviceconfig-numberrange.md)|Диапазон локальных портов можно установить только в том случае, если протокол TCP или UDP (6 или 17). Эта коллекция может содержать не более 500 элементов.|
|remotePortRanges|[коллекция numberRange](../resources/intune-deviceconfig-numberrange.md)|Диапазон удаленных портов можно установить только в том случае, если протокол TCP или UDP (6 или 17). Эта коллекция может содержать не более 500 элементов.|
|localAddressRanges|[коллекция iPv4Range](../resources/intune-shared-ipv4range.md)|Локальный диапазон адресов. Эта коллекция может содержать не более 500 элементов.|
|remoteAddressRanges|[коллекция iPv4Range](../resources/intune-shared-ipv4range.md)|Диапазон удаленных адресов. Эта коллекция может содержать не более 500 элементов.|
|appId|String|Идентификатор приложения, если это правило трафика запускается приложением.|
|appType|[vpnTrafficRuleAppType](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|Тип приложения, если это правило трафика запускается приложением. Возможные значения: `none`, `desktop`, `universal`.|
|routingPolicyType|[VPNTrafficRuleRoutingPolicyType](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|При запуске приложения указывает, следует ли включить раздельный туннель по этому маршруту. Возможные значения: `none`, `splitTunnel`, `forceTunnel`.|
|утверждения|Строка|Утверждения, связанные с этим правилом трафика.|

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



