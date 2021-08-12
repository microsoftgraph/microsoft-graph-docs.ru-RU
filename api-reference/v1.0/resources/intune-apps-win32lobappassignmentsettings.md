---
title: тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения мобильного приложения Win32 LOB группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a21b5f49c66da3e4334941200c06275516ff4c45895f572608abb4a5d0c87b0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169636"
---
# <a name="win32lobappassignmentsettings-resource-type"></a>тип ресурса win32LobAppAssignmentSettings

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения мобильного приложения Win32 LOB группе.


Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|уведомления|[win32LobAppNotification](../resources/intune-apps-win32lobappnotification.md)|Состояние уведомления для этого назначения приложения. Возможные значения: `showAll`, `showReboot`, `hideAll`.|
|restartSettings|[win32LobAppRestartSettings](../resources/intune-apps-win32lobapprestartsettings.md)|Параметры перезагрузки, которые необходимо применить для этого назначения приложения.|
|installTimeSettings|[mobileAppInstallTimeSettings](../resources/intune-apps-mobileappinstalltimesettings.md)|Параметры времени установки, которые необходимо применить для этого назначения приложения.|
|deliveryOptimizationPriority|[win32LobAppDeliveryOptimizationPriority](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|Приоритет оптимизации доставки для этого назначения приложения. Этот параметр не поддерживается в национальных облачных средах. Возможные значения: `notConfigured`, `foreground`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String",
  "restartSettings": {
    "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
    "gracePeriodInMinutes": 1024,
    "countdownDisplayBeforeRestartInMinutes": 1024,
    "restartNotificationSnoozeDurationInMinutes": 1024
  },
  "installTimeSettings": {
    "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
    "useLocalTime": true,
    "startDateTime": "String (timestamp)",
    "deadlineDateTime": "String (timestamp)"
  },
  "deliveryOptimizationPriority": "String"
}
```




