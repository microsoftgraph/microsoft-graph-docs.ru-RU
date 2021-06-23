---
title: тип ресурса cloudPcUserSettingAssignment
description: Представляет определенный набор назначений параметров пользователя.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: db97ff52ff8eb7ca1ef52563d577d5076273d859
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082190"
---
# <a name="cloudpcusersettingassignment--resource-type"></a>тип ресурса cloudPcUserSettingAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный набор назначений параметров пользователя.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для назначения настройки пользователя. Только для чтения. Если `target` это группа пользователей, iD имеет эту структуру: {policyID} \_ {groupID}.|
|target|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|Цель назначения для параметра пользователя. В настоящее время единственной целевой целью, поддерживаемой для этого параметра пользователя, является группа пользователей. Подробные сведения см. [в материале cloudPcManagementGroupAssignmentTarget.](cloudpcmanagementgroupassignmenttarget.md)|
|createdDateTime|DateTimeOffset|Дата и время создания этого назначения. Тип Timestamp представляет сведения о дате и времени с помощью формата ISO 8601 и всегда находится во времени UTC. Например, полночь UTC 1 января 2014 г. выглядит так: '2014-01-01T00:00:00Z'.  |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSettingAssignment",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementAssignmentTarget"
  }
}
```
