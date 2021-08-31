---
title: тип ресурса androidPermissionAction
description: Сопоставление между разрешением приложения Android и действием, которое должен принимать Android при запросе этого разрешения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d99ec168ae3cdb46dbe7727e9b60fb63624202fe
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819733"
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



