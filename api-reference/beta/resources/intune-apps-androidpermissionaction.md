---
title: тип ресурса androidPermissionAction
description: Сопоставление между разрешением приложения Android и действием, которое должен принимать Android при запросе этого разрешения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1d686d85cb4bbe7979a6e3bcdac453c0f9ebfedd017ed61829dbbf24d5e61f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54242124"
---
# <a name="androidpermissionaction-resource-type"></a>тип ресурса androidPermissionAction

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сопоставление между разрешением приложения Android и действием, которое должен принимать Android при запросе этого разрешения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|разрешение|Строка|Строка разрешений на Android, определяемая в официальной документации на Android.  Пример "android.permission.READ_CONTACTS".|
|action|[AndroidPermissionActionType](../resources/intune-apps-androidpermissionactiontype.md)|Тип действия разрешения Android. Возможные значения: `prompt`, `autoGrant`, `autoDeny`.|

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




