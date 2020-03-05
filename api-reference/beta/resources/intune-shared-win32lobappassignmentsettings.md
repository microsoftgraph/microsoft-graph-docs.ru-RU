---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c56d236c48918592394dc143bc6f2c45fb80401
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523501"
---
# <a name="win32lobappassignmentsettings-resource-type"></a>Тип ресурса win32LobAppAssignmentSettings

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.


Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|уведомления|[win32LobAppNotification](../resources/intune-shared-win32lobappnotification.md)|Состояние уведомления для этого назначения приложения. Возможные значения: `showAll`, `showReboot`, `hideAll`.|
|рестартсеттингс|[win32LobAppRestartSettings](../resources/intune-shared-win32lobapprestartsettings.md)|Параметры перезагрузки, которые необходимо применить к данному назначению приложения.|
|инсталлтимесеттингс|[mobileAppInstallTimeSettings](../resources/intune-shared-mobileappinstalltimesettings.md)|Параметры времени установки, применяемые к данному назначению приложения.|

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



