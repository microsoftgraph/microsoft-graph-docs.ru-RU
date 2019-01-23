---
title: Тип ресурса windows81VpnProxyServer
description: VPN-сервер прокси-сервера.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a400ed128a80e6fae11f090f7cdd445fe8c174b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398893"
---
# <a name="windows81vpnproxyserver-resource-type"></a>Тип ресурса windows81VpnProxyServer

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

VPN-сервер прокси-сервера.


Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|automaticConfigurationScriptUrl|String|Прокси-Автоматическая настройка сценария URL-адрес. Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|Адрес. Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|port|Int32|Порт. Допустимыми значениями от 0 до 65535 унаследованные от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|automaticallyDetectProxySettings|Логический|Автоматическое определение параметров прокси-сервера.|
|bypassProxyServerForLocalAddress|Логический|Использовать прокси-сервер для локальных адресов.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```




