---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e84a740a45cb57417c81b5c99a892642097413b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020396"
---
# <a name="win32lobappassignmentsettings-resource-type"></a>Тип ресурса win32LobAppAssignmentSettings

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.


Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|уведомления|[win32LobAppNotification](../resources/intune-apps-win32lobappnotification.md)|Состояние уведомления для этого назначения приложения. Возможные значения: `showAll`, `showReboot`, `hideAll`.|
|рестартсеттингс|[win32LobAppRestartSettings](../resources/intune-apps-win32lobapprestartsettings.md)|Параметры перезагрузки, которые необходимо применить к данному назначению приложения.|
|инсталлтимесеттингс|[mobileAppInstallTimeSettings](../resources/intune-apps-mobileappinstalltimesettings.md)|Параметры времени установки, применяемые к данному назначению приложения.|

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
  }
}
```





