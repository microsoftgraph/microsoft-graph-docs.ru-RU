---
title: Тип ресурса androidPermissionAction
description: Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: daf72bbc5f8d1e32480adeda72c3f759255f54db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860538"
---
# <a name="androidpermissionaction-resource-type"></a>Тип ресурса androidPermissionAction

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|разрешение|Строка|Строка, Android разрешений, определенных в Официальная документация Android.  Пример «android.permission.READ_CONTACTS».|
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





