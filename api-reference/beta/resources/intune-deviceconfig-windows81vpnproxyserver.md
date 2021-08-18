---
title: тип ресурса windows81VpnProxyServer
description: VPN Прокси-сервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3b818e68b76d74297dd820114e1e445050cd3481bf5d9cc5b86bb30c7df6e72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248489"
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
|automaticallyDetectProxySettings|Логический|Автоматически обнаруживать параметры прокси.|
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




