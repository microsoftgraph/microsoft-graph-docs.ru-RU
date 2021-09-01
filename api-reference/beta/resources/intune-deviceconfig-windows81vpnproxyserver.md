---
title: тип ресурса windows81VpnProxyServer
description: VPN Прокси-сервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b2c70ce97a73ccef8ccdba62ea1e63590f758a7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783472"
---
# <a name="windows81vpnproxyserver-resource-type"></a>тип ресурса windows81VpnProxyServer

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
|automaticallyDetectProxySettings|Boolean|Автоматически обнаруживать параметры прокси.|
|bypassProxyServerForLocalAddress|Логический|Обход прокси-сервера для локального адреса.|

## <a name="relationships"></a>Связи
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



