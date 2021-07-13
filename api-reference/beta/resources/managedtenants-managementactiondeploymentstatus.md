---
title: тип ресурса managementActionDeploymentStatus
description: Представляет состояние развертывания для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: efd789a7b4b48098e8d679273da1152f6611a28c
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403044"
---
# <a name="managementactiondeploymentstatus-resource-type"></a>тип ресурса managementActionDeploymentStatus

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние развертывания для данного управляемого клиента.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|managementActionId|String|Идентификатор для действия управления. Обязательный. Только для чтения.|
|managementTemplateId|String|Идентификатор шаблона управления, который использовался для создания действия управления. Обязательный. Только для чтения.|
|status|managementActionStatus|Состояние действия управления. Возможные значения: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, `riskAccepted`, `unknownFutureValue`. Обязательный.|
|workloadActionDeploymentStatuses|[коллекция microsoft.graph.managedTenants.workloadActionDeploymentStatus](../resources/managedtenants-workloadactiondeploymentstatus.md)|Коллекция статуй развертывания действий рабочей нагрузки для данного действия управления. Необязательное.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionDeploymentStatus",
  "managementTemplateId": "String",
  "managementActionId": "String",
  "status": "String",
  "workloadActionDeploymentStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
    }
  ]
}
```
