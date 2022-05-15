---
title: тип ресурса plannerPlanContainer
description: Представляет контейнер для plannerPlan. Контейнер — это ресурс, указывающий правила авторизации и время существования плана.
author: TarkanSevilmis
ms.localizationpriority: high
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: dbb95f1124461e12b36d6c4f69dac193aa349b15
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420788"
---
# <a name="plannerplancontainer-resource-type"></a>тип ресурса plannerPlanContainer

Пространство имен: microsoft.graph

Представляет контейнер для [plannerPlan](plannerplan.md). Контейнер — это ресурс, указывающий правила авторизации и время существования плана. Это означает, что только пользователи, которым разрешено работать с ресурсом, содержащим план, смогут работать с планом и задачами в нем. При удалении содержащего ресурса также удаляются содержащиеся планы. Свойства **plannerPlanContainer** нельзя изменить после создания плана.

Планировщик в настоящее время поддерживает типы контейнеров, перечисленные в следующей таблице. При создании плана необходимо указать свойство **containerUrl** с путем к ресурсу, указанному в следующей таблице.

|Тип|Описание|Путь к ресурсу|
|----|-----------|--------------------|
|group| План содержится в [группе](group.md).| https://graph.microsoft.com/v1.0/groups/{id}|
|состав| План содержится в **plannerRoster** | https://graph.microsoft.com/beta/planner/rosters/{id}. **plannerRosters** в настоящее время доступны только в бета-версии.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|containerId|String|Идентификатор ресурса, содержащего план.|
|type|plannerContainerType| Тип ресурса, содержащего план. Поддерживаемые типы см. в предыдущей таблице. Возможные значения: `group`, `unknownFutureValue`, `roster`. Обратите внимание, что требуется использоваться заголовок запроса `Prefer: include-unknown-enum-members`, чтобы получить следующее значение в этом [расширяемом перечислении](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `roster`.|
|url|String|Полный канонический URL-адрес контейнера.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerPlanContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlanContainer",
  "containerId": "String",
  "type": "String",
  "url": "String"
}
```

