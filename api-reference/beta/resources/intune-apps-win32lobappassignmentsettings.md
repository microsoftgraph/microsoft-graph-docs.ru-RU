---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8b6588c270c9b7977ddd7b3c7eb239f3b0432cb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993237"
---
# <a name="win32lobappassignmentsettings-resource-type"></a>Тип ресурса win32LobAppAssignmentSettings

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.


Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|уведомления|[win32LobAppNotification](../resources/intune-apps-win32lobappnotification.md)|Состояние уведомления о назначении этого приложения. Возможные значения: `showAll`, `showReboot`, `hideAll`.|

## <a name="relationships"></a>Отношения
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
  "notifications": "String"
}
```





