---
title: Тип ресурса Девицеманажементпартнерассигнмент
description: Целевая группа пользователей для партнера по управлению устройствами
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 306acfae948a81ca5c8933f455a21347bf27ee9e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42778724"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a>Тип ресурса Девицеманажементпартнерассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Целевая группа пользователей для партнера по управлению устройствами

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Группы пользователей, предназначенные для регистрации устройств с помощью партнера.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



