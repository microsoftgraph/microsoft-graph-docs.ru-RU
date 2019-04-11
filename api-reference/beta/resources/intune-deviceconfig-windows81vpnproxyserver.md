---
title: Тип ресурса windows81VpnProxyServer
description: VPN-прокси-сервер.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a337dc2d18ed5f10ecb9f8f654a7d19175fc476
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800912"
---
# <a name="windows81vpnproxyserver-resource-type"></a>Тип ресурса windows81VpnProxyServer

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

VPN-прокси-сервер.


НаСледуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Аутоматикконфигуратионскриптурл|String|URL-адрес скрипта автоматической настройки прокси-сервера. НаСледуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|Address. НаСледуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
|порта|Int32|Порта. Допустимые значения — от 0 до 65535, наСледуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
|Аутоматикаллидетектпроксисеттингс|Boolean|Автоматически определять параметры прокси-сервера.|
|Бипасспроксисерверфорлокаладдресс|Boolean|Обход прокси-сервера для локального адреса.|

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





