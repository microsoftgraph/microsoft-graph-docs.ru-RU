---
title: Тип ресурса mobileAppTroubleshootingDeviceCheckinHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6b9d900e712e3c3b126dd36671049e8935f09a83
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844949"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a>Тип ресурса mobileAppTroubleshootingDeviceCheckinHistory

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.

Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|Время возникновения элемент журнала. Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```





