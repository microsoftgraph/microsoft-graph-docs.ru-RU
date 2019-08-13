---
title: Тип ресурса Впнпроксисервер
description: VPN-прокси-сервер.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: faa9a1bd74a9535cccca8d387a5a8a23de6db3b4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367619"
---
# <a name="vpnproxyserver-resource-type"></a>Тип ресурса Впнпроксисервер

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

VPN-прокси-сервер.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|аутоматикконфигуратионскриптурл|String|URL-адрес скрипта автоматической настройки прокси-сервера.|
|address|String|Address.|
|порта|Int32|Порта. Допустимые значения — от 0 до 65535|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```



