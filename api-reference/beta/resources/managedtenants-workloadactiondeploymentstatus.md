---
title: workloadActionDeploymentStatus resource type
description: Представляет состояние развертывания для действия рабочей нагрузки.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a8c14b821ceabf8c8196a25c141ad8730f7151d6
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402603"
---
# <a name="workloadactiondeploymentstatus-resource-type"></a>workloadActionDeploymentStatus resource type

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние развертывания для действия рабочей нагрузки.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionId|String|Уникальный идентификатор для действия рабочей нагрузки. Обязательный. Только для чтения.|
|deployedPolicyId|String|Идентификатор любой политики, созданной с помощью действия рабочей нагрузки. Необязательно. Только для чтения.|
|error|[microsoft.graph.genericError](../resources/genericerror.md)|Подробные сведения об исключениях, которые возникают при развертывании действия рабочей нагрузки. Необязательное. Обязательный.|
|lastDeploymentDateTime|DateTimeOffset|Дата и время последнего развертывания действия рабочей нагрузки. Необязательное.|
|status|workloadActionStatus|Состояние развертывания действия рабочей нагрузки. Возможные значения: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `unknownFutureValue`. Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadActionDeploymentStatus",
  "actionId": "String",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.genericError"
  },
  "deployedPolicyId": "String",
  "lastDeploymentDateTime": "String (timestamp)"
}
```
