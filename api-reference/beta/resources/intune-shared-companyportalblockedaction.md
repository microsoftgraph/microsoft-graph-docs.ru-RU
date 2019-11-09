---
title: Тип ресурса Компанипорталблоккедактион
description: Заблокированные действия на корпоративном портале в соответствии с типами владения платформой и устройствами
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8ed24dc039742ef7c0412fcd8a67f1a460062c7f
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088282"
---
# <a name="companyportalblockedaction-resource-type"></a>Тип ресурса Компанипорталблоккедактион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Заблокированные действия на корпоративном портале в соответствии с типами владения платформой и устройствами

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|platform|[девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|ОС устройства/платформа. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Тип владения устройством. Возможные значения: `unknown`, `company`, `personal`.|
|action|[компанипорталактион](../resources/intune-shared-companyportalaction.md)|Действие устройства. Возможные значения: `unknown`, `remove`, `reset`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyPortalBlockedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyPortalBlockedAction",
  "platform": "String",
  "ownerType": "String",
  "action": "String"
}
```



