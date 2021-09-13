---
title: тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения мобильного приложения Win32 LOB группе.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: feefe30e7e9645471172ec38aaf147f675fc5149
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039051"
---
# <a name="win32lobappassignmentsettings-resource-type"></a>тип ресурса win32LobAppAssignmentSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения мобильного приложения Win32 LOB группе.


Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|уведомления|[win32LobAppNotification](../resources/intune-shared-win32lobappnotification.md)|Состояние уведомления для этого назначения приложения. Возможные значения: `showAll`, `showReboot`, `hideAll`.|
|restartSettings|[win32LobAppRestartSettings](../resources/intune-shared-win32lobapprestartsettings.md)|Параметры перезагрузки, которые необходимо применить для этого назначения приложения.|
|installTimeSettings|[mobileAppInstallTimeSettings](../resources/intune-shared-mobileappinstalltimesettings.md)|Параметры времени установки, которые необходимо применить для этого назначения приложения.|
|deliveryOptimizationPriority|[win32LobAppDeliveryOptimizationPriority](../resources/intune-shared-win32lobappdeliveryoptimizationpriority.md)|Приоритет оптимизации доставки для этого назначения приложения. Этот параметр не поддерживается в национальных облачных средах. Возможные значения: `notConfigured`, `foreground`.|

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



