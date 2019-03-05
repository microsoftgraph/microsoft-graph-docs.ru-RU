---
title: Тип ресурса Впнтраффикруле
description: Определение правила трафика VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd004341928260187518966e2356f59faff57898
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139944"
---
# <a name="vpntrafficrule-resource-type"></a>Тип ресурса Впнтраффикруле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила трафика VPN.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Расширением.|
|QP|Int32|Протоколы (0-255). Допустимые значения — от 0 до 255|
|Локалпортранжес|Коллекция [нумберранже](../resources/intune-deviceconfig-numberrange.md)|Локальный диапазон портов можно задать только в том случае, если протокол имеет значение TCP или UDP (6 или 17). Эта коллекция может содержать не более 500 элементов.|
|Ремотепортранжес|Коллекция [нумберранже](../resources/intune-deviceconfig-numberrange.md)|Диапазон удаленных портов можно задать только в том случае, если протокол имеет значение TCP или UDP (6 или 17). Эта коллекция может содержать не более 500 элементов.|
|Локаладдрессранжес|Коллекция [iPv4Range](../resources/intune-shared-ipv4range.md)|Диапазон локальных адресов. Эта коллекция может содержать не более 500 элементов.|
|Ремотеаддрессранжес|Коллекция [iPv4Range](../resources/intune-shared-ipv4range.md)|Диапазон удаленных адресов. Эта коллекция может содержать не более 500 элементов.|
|appId|String|Идентификатор приложения, если это правило трафика вызывается приложением.|
|Тип|[Впнтраффикрулеапптипе](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|Тип приложения, если это правило трафика вызывается приложением. Возможные значения: `none`, `desktop`, `universal`.|
|Раутингполицитипе|[Впнтраффикрулераутингполицитипе](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|Когда приложение запускается, указывает, следует ли включить раздельное туннелирование по этому маршруту. Возможные значения: `none`, `splitTunnel`, `forceTunnel`.|
|утверждения|String|Утверждения, связанные с этим правилом трафика.|

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




