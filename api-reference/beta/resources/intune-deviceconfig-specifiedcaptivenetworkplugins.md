---
title: указанный тип ресурсаCaptiveNetworkPlugins
description: Указывает все плагины сети Captive, разрешенные во время VPN-подключения IKEv2 AlwaysOn
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e8ff13aed2200c309ee83f5514b5cd421998262
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023528"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a>указанный тип ресурсаCaptiveNetworkPlugins

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает все плагины сети Captive, разрешенные во время VPN-подключения IKEv2 AlwaysOn

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedBundleIdentifiers|Коллекция строк|Адрес сервера IKEv2. Должен быть FQDN, UserFQDN, сетевой адрес или ASN1DN|

## <a name="relationships"></a>Отношения
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



