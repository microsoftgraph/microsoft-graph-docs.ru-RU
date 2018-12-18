---
title: Тип ресурса mobileAppTroubleshootingAppTargetHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
ms.openlocfilehash: cdb901d4c532b57025837a2fb0cc0975ceba3f8c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312735"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a>Тип ресурса mobileAppTroubleshootingAppTargetHistory

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.

Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|Время возникновения элемент журнала. Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|
|securityGroupId|String.|К которому нацелено AAD идентификатор группы безопасности.|
|runState|[runState](../resources/intune-shared-runstate.md)|Состояние элемента. Возможные значения: `unknown`, `success`, `fail`.|
|errorCode|String|Код ошибки сбоя, пустой, если нет сбоев.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```





