---
title: Тип ресурса Андроидпермиссионактион
description: Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4766bb91d5d1cde99a12f5a8e4903451a3ac5aca
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950489"
---
# <a name="androidpermissionaction-resource-type"></a>Тип ресурса Андроидпермиссионактион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|права|Строка|Строка разрешений Android, определенная в официальной документации по Android.  Пример: "Android. Permission. РЕАД_КОНТАКТС".|
|action|[Андроидпермиссионактионтипе](../resources/intune-apps-androidpermissionactiontype.md)|Тип действия разрешений Android. Возможные значения: `prompt`, `autoGrant`, `autoDeny`.|

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




