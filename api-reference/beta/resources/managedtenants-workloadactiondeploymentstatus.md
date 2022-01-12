---
title: workloadActionDeploymentStatus resource type
description: Представляет состояние развертывания для действия рабочей нагрузки.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 763ad6e70969565f15f9db159a423d6ec1bbb4a2
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792045"
---
# <a name="workloadactiondeploymentstatus-resource-type"></a>workloadActionDeploymentStatus resource type

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние развертывания для действия рабочей нагрузки.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionId|String|Уникальный идентификатор для действия рабочей нагрузки. Обязательное. Только для чтения.|
|deployedPolicyId|String|Идентификатор любой политики, созданной с помощью действия рабочей нагрузки. Необязательно. Только для чтения.|
|error|[microsoft.graph.genericError](../resources/genericerror.md)|Подробные сведения об исключениях, которые возникают при развертывании действия рабочей нагрузки. Необязательно. Обязательное.|
|lastDeploymentDateTime|DateTimeOffset|Дата и время последнего развертывания действия рабочей нагрузки. Необязательное свойство.|
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
