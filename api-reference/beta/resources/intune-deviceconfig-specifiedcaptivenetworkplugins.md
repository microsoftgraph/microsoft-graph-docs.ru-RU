---
title: указанный тип ресурсаCaptiveNetworkPlugins
description: Указывает все плагины сети Captive, разрешенные во время VPN-подключения IKEv2 AlwaysOn
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0843c5a6cc6bc71eb10c8a42f0b9ad0ac49cb328
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785145"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a>указанный тип ресурсаCaptiveNetworkPlugins

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает все плагины сети Captive, разрешенные во время VPN-подключения IKEv2 AlwaysOn

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedBundleIdentifiers|Коллекция String|Адрес сервера IKEv2. Должен быть FQDN, UserFQDN, сетевой адрес или ASN1DN|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.specifiedCaptiveNetworkPlugins",
  "allowedBundleIdentifiers": [
    "String"
  ]
}
```



