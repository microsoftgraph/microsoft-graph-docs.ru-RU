---
title: тип ресурса cloudPcUserSettingAssignment
description: Представляет определенный набор назначений параметров пользователя.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 704142ce266a826606b6c32b209d69d052d1a3c9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993739"
---
# <a name="cloudpcusersettingassignment--resource-type"></a>тип ресурса cloudPcUserSettingAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный набор назначений параметров пользователя.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для назначения настройки пользователя. Только для чтения. Если `target` это группа пользователей, у ID есть эта структура: {policyID}_{groupID}.|
|target|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|Цель назначения для параметра пользователя. В настоящее время единственной целевой целью, поддерживаемой для параметров пользователя, является группа пользователей.|
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
