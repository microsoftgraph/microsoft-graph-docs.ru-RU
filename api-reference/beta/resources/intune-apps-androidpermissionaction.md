---
title: Тип ресурса Андроидпермиссионактион
description: Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c0e1b793a447d29d1ed554e1b6466895ccc9e57f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459144"
---
# <a name="androidpermissionaction-resource-type"></a>Тип ресурса Андроидпермиссионактион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|права|String|Строка разрешений Android, определенная в официальной документации по Android.  Пример: "Android. Permission. READ_CONTACTS".|
|action|[андроидпермиссионактионтипе](../resources/intune-apps-androidpermissionactiontype.md)|Тип действия разрешений Android. Возможные значения: `prompt`, `autoGrant`, `autoDeny`.|

## <a name="relationships"></a>Отношения
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



