---
title: тип ресурса appleVpnAlwaysOnConfiguration
description: Всегда на конфигурации VPN для MacOS и iOS IKEv2
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38b574bd07e4797a14de2e6061cf45e638ca2b98
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787008"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a>тип ресурса appleVpnAlwaysOnConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Всегда на конфигурации VPN для MacOS и iOS IKEv2

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|tunnelConfiguration|[vpnTunnelConfigurationType](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|Определяет, к каким подключениям применяется определенная конфигурация туннеля. Возможные значения: `wifiAndCellular`, `cellular`, `wifi`.|
|userToggleEnabled|Логический|Разрешить пользователю для настройки VPN с помощью пользовательского интерфейса|
|voicemailExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Определите, будет ли служба голосовой почты освобождена от подключения к VPN всегда. Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|airPrintExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Определите, будет ли служба AirPrint освобождена от подключения к VPN всегда. Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|cellularExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Определите, будет ли служба сотовой связи освобождена от подключения к VPN всегда. Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|allowAllCaptiveNetworkPlugins|Логический|Указывает, следует ли разрешать трафик из всех подключенных сетевых плагинов за пределами VPN|
|allowedCaptiveNetworkPlugins|[specifiedCaptiveNetworkPlugins](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|Определяет, разрешены ли все, некоторые или никакие несвойные сетевые приложения|
|allowCaptiveWebSheet|Логический|Определяет, разрешен ли трафик из приложения Websheet за пределами VPN|
|natKeepAliveIntervalInSeconds|Int32|Указывает, как часто в секундах отправлять пакет для сохраняемого перевода сетевых адресов через VPN|
|natKeepAliveOffloadEnable|Логический|Включить аппаратную разгрузку сигналов nat keepalive, когда устройство спит|

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



