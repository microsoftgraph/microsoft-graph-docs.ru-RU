---
title: Тип ресурса Апплевпналвайсонконфигуратион
description: Конфигурация Always on VPN для MacOS и iOS IKEv2
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c48c22acf2344a0be569835902c20bca21ed0355
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636660"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a>Тип ресурса Апплевпналвайсонконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация Always on VPN для MacOS и iOS IKEv2

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|туннелконфигуратион|[впнтуннелконфигуратионтипе](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|Определяет, к каким подключениям применяется определенная конфигурация туннеля. Возможные значения: `wifiAndCellular`, `cellular`, `wifi`.|
|усертогглинаблед|Boolean|Разрешить пользователю переключать конфигурацию VPN с помощью пользовательского интерфейса|
|воицемаилексцептионактион|[впнсервицеексцептионактион](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Определите, будет ли служба голосовой почты исключена из постоянного подключения VPN. Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|аирпринтексцептионактион|[впнсервицеексцептионактион](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Определите, будет ли служба Аирпринт освобождена от постоянного подключения VPN. Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|целлуларексцептионактион|[впнсервицеексцептионактион](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Определите, будет ли служба сотовой связи освобождена от постоянного подключения VPN. Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|алловаллкаптивенетворкплугинс|Boolean|Указывает, следует ли разрешить трафик от всех сетевых подключаемых модулей для подключения извне VPN|
|алловедкаптивенетворкплугинс|[спеЦифиедкаптивенетворкплугинс](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|Определяет, разрешены ли все, некоторые или не являющиеся собственными сетевыми приложениями для работы с пререгистром|
|алловкаптивевебшит|Boolean|Определяет, разрешен ли трафик из приложения "Таблица" за прес помощью VPN-подключения|
|наткипаливеинтервалинсекондс|Int32|Указывает, как часто в секундах отправлять пакет KeepAlive для преобразования сетевых адресов через VPN|
|наткипаливеоффлоаденабле|Boolean|Включение аппаратной разгрузки сигналов проверки активности сетевых адресов, когда устройство находится в спящем режиме|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnAlwaysOnConfiguration",
  "tunnelConfiguration": "String",
  "userToggleEnabled": true,
  "voicemailExceptionAction": "String",
  "airPrintExceptionAction": "String",
  "cellularExceptionAction": "String",
  "allowAllCaptiveNetworkPlugins": true,
  "allowedCaptiveNetworkPlugins": {
    "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
    "allowedBundleIdentifiers": [
      "String"
    ]
  },
  "allowCaptiveWebSheet": true,
  "natKeepAliveIntervalInSeconds": 1024,
  "natKeepAliveOffloadEnable": true
}
```



