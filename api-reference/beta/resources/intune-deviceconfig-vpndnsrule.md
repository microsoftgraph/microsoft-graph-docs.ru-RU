---
title: тип ресурса vpnDnsRule
description: Определение правила VPN DNS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e034016fe3a6eff5d84db1421e5e6e80d1f70be3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081215"
---
# <a name="vpndnsrule-resource-type"></a>тип ресурса vpnDnsRule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила VPN DNS.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя.|
|серверы|Коллекция объектов string|Серверы.|
|proxyServerUri|String|Прокси-сервер Uri.|
|autoTrigger|Boolean|Автоматически подключайтесь к VPN при подключении устройства к этому домену: False по умолчанию.|
|стойкий|Логическое|Сохранение этого правила активным даже при не подключении VPN: False по умолчанию|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```



