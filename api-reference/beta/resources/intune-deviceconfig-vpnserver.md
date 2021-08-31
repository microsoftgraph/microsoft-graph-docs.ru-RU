---
title: тип ресурса vpnServer
description: Определение VPN Server.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d81928758fc87b37954c2be38ee2c60e64a0d840
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783955"
---
# <a name="vpnserver-resource-type"></a>тип ресурса vpnServer

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение VPN Server.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание.|
|address|String|Адрес (IP-адрес, FQDN или URL-адрес)|
|isDefaultServer|Логический|Сервер по умолчанию.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```



