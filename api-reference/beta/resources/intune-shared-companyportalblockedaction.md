---
title: Тип ресурса Компанипорталблоккедактион
description: Заблокированные действия на корпоративном портале в соответствии с типами владения платформой и устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e456ba03de299a04a1434c7a19871aa908274b1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723773"
---
# <a name="companyportalblockedaction-resource-type"></a>Тип ресурса Компанипорталблоккедактион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Заблокированные действия на корпоративном портале в соответствии с типами владения платформой и устройствами

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|платформа|[девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|ОС устройства/платформа. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Тип владения устройством. Возможные значения: `unknown`, `company`, `personal`.|
|action|[companyPortalAction](../resources/intune-shared-companyportalaction.md)|Действие устройства. Возможные значения: `unknown`, `remove`, `reset`.|

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





