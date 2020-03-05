---
title: Тип ресурса Апплевпналвайсонконфигуратион
description: Конфигурация Always on VPN для MacOS и iOS IKEv2
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3b963556254766cff951faeed707e5c6aceed05f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527145"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a>Тип ресурса Апплевпналвайсонконфигуратион

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация Always on VPN для MacOS и iOS IKEv2

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|туннелконфигуратион|[vpnTunnelConfigurationType](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|Определяет, к каким подключениям применяется определенная конфигурация туннеля. Возможные значения: `wifiAndCellular`, `cellular`, `wifi`.|
|усертогглинаблед|Логический|Разрешить пользователю переключать конфигурацию VPN с помощью пользовательского интерфейса|
|воицемаилексцептионактион|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Определите, будет ли служба голосовой почты исключена из постоянного подключения VPN. Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|аирпринтексцептионактион|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Определите, будет ли служба Аирпринт освобождена от постоянного подключения VPN. Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|целлуларексцептионактион|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Определите, будет ли служба сотовой связи освобождена от постоянного подключения VPN. Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|алловаллкаптивенетворкплугинс|Логический|Указывает, следует ли разрешить трафик от всех сетевых подключаемых модулей для подключения извне VPN|
|алловедкаптивенетворкплугинс|[specifiedCaptiveNetworkPlugins](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|Определяет, разрешены ли все, некоторые или не являющиеся собственными сетевыми приложениями для работы с пререгистром|
|алловкаптивевебшит|Логический|Определяет, разрешен ли трафик из приложения "Таблица" за прес помощью VPN-подключения|
|наткипаливеинтервалинсекондс|Int32|Указывает, как часто в секундах отправлять пакет KeepAlive для преобразования сетевых адресов через VPN|
|наткипаливеоффлоаденабле|Логический|Включение аппаратной разгрузки сигналов проверки активности сетевых адресов, когда устройство находится в спящем режиме|

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



