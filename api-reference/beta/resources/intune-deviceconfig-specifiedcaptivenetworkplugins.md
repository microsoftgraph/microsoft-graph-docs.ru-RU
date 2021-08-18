---
title: указанный тип ресурсаCaptiveNetworkPlugins
description: Указывает все плагины сети Captive, разрешенные во время VPN-подключения IKEv2 AlwaysOn
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b162b0aa3da966cb7a55b23163d2a3bf51dc9e466b4a95fcdfe324b32a1bc94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236943"
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




