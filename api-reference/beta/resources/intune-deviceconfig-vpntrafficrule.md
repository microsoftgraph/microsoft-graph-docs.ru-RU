---
title: Тип ресурса Впнтраффикруле
description: Определение правила трафика VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f1e87a3076c53d4d95b60f0ac884cc825da6a85
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43359382"
---
# <a name="vpntrafficrule-resource-type"></a>Тип ресурса Впнтраффикруле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила трафика VPN.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Расширением.|
|QP|Int32|Протоколы (0-255). Допустимые значения — от 0 до 255|
|локалпортранжес|Коллекция [нумберранже](../resources/intune-deviceconfig-numberrange.md)|Локальный диапазон портов можно задать только в том случае, если протокол имеет значение TCP или UDP (6 или 17). Эта коллекция может содержать не более 500 элементов.|
|ремотепортранжес|Коллекция [нумберранже](../resources/intune-deviceconfig-numberrange.md)|Диапазон удаленных портов можно задать только в том случае, если протокол имеет значение TCP или UDP (6 или 17). Эта коллекция может содержать не более 500 элементов.|
|локаладдрессранжес|Коллекция [iPv4Range](../resources/intune-shared-ipv4range.md)|Диапазон локальных адресов. Эта коллекция может содержать не более 500 элементов.|
|ремотеаддрессранжес|Коллекция [iPv4Range](../resources/intune-shared-ipv4range.md)|Диапазон удаленных адресов. Эта коллекция может содержать не более 500 элементов.|
|appId|String|Идентификатор приложения, если это правило трафика вызывается приложением.|
|Тип|[впнтраффикрулеапптипе](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|Тип приложения, если это правило трафика вызывается приложением. Возможные значения: `none`, `desktop`, `universal`.|
|раутингполицитипе|[впнтраффикрулераутингполицитипе](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|Когда приложение запускается, указывает, следует ли включить раздельное туннелирование по этому маршруту. Возможные значения: `none`, `splitTunnel`, `forceTunnel`.|
|страх|String|Утверждения, связанные с этим правилом трафика.|

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



