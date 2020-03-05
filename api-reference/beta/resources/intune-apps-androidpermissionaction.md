---
title: Тип ресурса Андроидпермиссионактион
description: Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52b105c831399b935196254d794bd5da513d19f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42494102"
---
# <a name="androidpermissionaction-resource-type"></a>Тип ресурса Андроидпермиссионактион

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|права|String|Строка разрешений Android, определенная в официальной документации по Android.  Пример: "Android. Permission. READ_CONTACTS".|
|action|[андроидпермиссионактионтипе](../resources/intune-apps-androidpermissionactiontype.md)|Тип действия разрешений Android. Возможные значения: `prompt`, `autoGrant`, `autoDeny`.|

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



