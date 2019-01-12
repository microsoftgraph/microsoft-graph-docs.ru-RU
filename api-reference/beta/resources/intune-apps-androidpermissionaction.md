---
title: Тип ресурса androidPermissionAction
description: Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5ad7b438951b947cc515f1472dd1eae8caf472f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977124"
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





