---
title: Тип ресурса androidPermissionAction
description: Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.
ms.openlocfilehash: e65f9b28169e231e34b5a7a46316821f77639233
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076841"
---
# <a name="androidpermissionaction-resource-type"></a>Тип ресурса androidPermissionAction

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.
## <a name="properties"></a>Свойства
|Свойство|Тип|Description|
|:---|:---|:---|
|разрешение|String|Строка, Android разрешений, определенных в Официальная документация Android.  Пример «android.permission.READ_CONTACTS».|
|action|[androidPermissionActionType](../resources/intune-apps-androidpermissionactiontype.md)|Тип действия Android разрешений. Возможные значения: `prompt`, `autoGrant`, `autoDeny`.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```





