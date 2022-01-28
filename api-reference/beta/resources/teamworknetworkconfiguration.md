---
title: тип ресурса teamworkNetworkConfiguration
description: Представляет сведения о конфигурации сети для устройства с Microsoft Teams с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5f08d5d3263917adfb9bc20ca5f964972281ecbb
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262498"
---
# <a name="teamworknetworkconfiguration-resource-type"></a>тип ресурса teamworkNetworkConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о конфигурации сети для устройства с Microsoft Teams [включенной поддержкой](../resources/teamworkdevice.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|defaultGateway|String|Шлюз по умолчанию — это путь, используемый для получения сведений, когда назначение неизвестно устройству.|
|domainName|String|Сетевой домен устройства, например, contoso.com.|
|hostName|String|Имя устройства в сети.|
|ipAddress|String|IP-адрес — это числовая метка, которая однозначно идентифицирует каждое устройство, подключенное к Интернету.|
|isDhcpEnabled|Логическое|`True` если включенА DHCP.|
|isPCPortEnabled|Логическое|`True` если порт ПК включен.|
|primaryDns|String|Основной DNS — это первая точка контакта для устройства, которое преобразует имя хост-адреса в IP-адрес.|
|secondaryDns|String|Вторичный DNS используется, когда основная DNS недоступна.|
|subnetMask|String|Маска подсети — это номер, который различает сетевой адрес и хост-адрес в IP-адресе.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkNetworkConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkNetworkConfiguration",
  "defaultGateway": "String",
  "domainName": "String",
  "hostName": "String",
  "ipAddress": "String",
  "isDhcpEnabled": "Boolean",
  "isPCPortEnabled": "Boolean",
  "primaryDns": "String",
  "secondaryDns": "String",
  "subnetMask": "String"
}
```

