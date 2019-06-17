---
title: Тип ресурса Макосфиреваллаппликатион
description: Представляет приложение в списке приложений брандмауэра macOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a22914ba0af21418b593015995b6d7665ae3bc3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992201"
---
# <a name="macosfirewallapplication-resource-type"></a>Тип ресурса Макосфиреваллаппликатион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет приложение в списке приложений брандмауэра macOS

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bundleId|String|Свойства bundleid приложения.|
|Алловсинкомингконнектионс|Boolean|Разрешены ли входящие подключения.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```





