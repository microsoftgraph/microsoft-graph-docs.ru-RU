---
title: тип ресурса windows10VpnProxyServer
description: VPN Прокси-сервер.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9ab8f6ab7a662487d7cf8e144cd25bb8bd53a0f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147908"
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
|automaticConfigurationScriptUrl|String|URL-адрес сценария автоматической конфигурации прокси. Унаследованный от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|Адрес. Унаследованный от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|порт|Int32|Порт. Допустимые значения от 0 до 65535, унаследованные от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|
|bypassProxyServerForLocalAddress|Логическое|Обход прокси-сервера для локального адреса.|

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



