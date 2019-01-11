---
title: Тип ресурса macOSFirewallApplication
description: Представляет приложение в списке приложений macOS брандмауэра
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 536f2f596286f6b5457557f575ba018c65001bfe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835223"
---
# <a name="macosfirewallapplication-resource-type"></a>Тип ресурса macOSFirewallApplication

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет приложение в списке приложений macOS брандмауэра
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bundleId|String|BundleId приложения.|
|allowsIncomingConnections|Логический|Указывает, разрешены ли входящих подключений.|

## <a name="relationships"></a>Связи
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





