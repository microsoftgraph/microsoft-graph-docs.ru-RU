---
title: тип ресурса windows10VpnProxyServer
description: VPN Прокси-сервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b60102b1139bc1c869082016afb1436bcf061b94
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785740"
---
# <a name="windows10vpnproxyserver-resource-type"></a>тип ресурса windows10VpnProxyServer

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

VPN Прокси-сервер.


Наследуется [от vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|automaticConfigurationScriptUrl|Строка|URL-адрес сценария автоматической конфигурации прокси. Унаследованный от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|Адрес. Унаследованный от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|порт|Int32|Порт. Допустимые значения от 0 до 65535, унаследованные от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|bypassProxyServerForLocalAddress|Логический|Обход прокси-сервера для локального адреса.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```



