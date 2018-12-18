---
title: Тип ресурса androidPermissionAction
description: Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.
author: tfitzmac
ms.openlocfilehash: 90117b30dae765151e79d8ad1c2ae1afaa5a42ff
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331138"
---
# <a name="androidpermissionaction-resource-type"></a>Тип ресурса androidPermissionAction

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|разрешение|String.|Строка, Android разрешений, определенных в Официальная документация Android.  Пример «android.permission.READ_CONTACTS».|
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





