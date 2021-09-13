---
title: тип ресурса androidPermissionAction
description: Сопоставление между разрешением приложения Android и действием, которое должен принимать Android при запросе этого разрешения.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f1065497839de4ccc4a90d48deb6651e11422e84
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115606"
---
# <a name="androidpermissionaction-resource-type"></a>тип ресурса androidPermissionAction

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сопоставление между разрешением приложения Android и действием, которое должен принимать Android при запросе этого разрешения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|разрешение|String|Строка разрешений на Android, определяемая в официальной документации на Android.  Пример "android.permission.READ_CONTACTS".|
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



