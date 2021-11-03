---
title: Тип ресурса утверждения
description: Объект утверждения, связанный с accessPackageAssignmentRequest или userConsentRequest.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e9c459563fa776427dfebcc6c6063b9bda1da846
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730391"
---
# <a name="approval-resource-type"></a>Тип ресурса утверждения

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](entitlementmanagement-root.md)объект утверждения решений, связанных с `accessPackageAssignmentRequest` . Запрос на один шаг может иметь один шаг, связанный с ним, на который могут действовать одобрители. Кроме того, многоэтапный запрос может иметь несколько действий, связанных с ним, на которые могут действовать одобрители. Однако в многоэтапных утверждениях показаны как ожидающих, так и ранее завершенных действий.

В [userConsentRequests](../resources/userconsentrequest.md)объект утверждения решений, связанных с запросом.

В [управлении ролью](../resources/rolemanagement.md)принимаются решения об утверждении или отказе в назначении ролей.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Получить утверждение](../api/approval-get.md) | [утверждение](approval.md) | Извлечение свойств объекта **утверждения.** |


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта утверждения.  В управлении правами это тот же идентификатор, что и идентификатор запроса на назначение пакета [доступа.](accesspackageassignmentrequest.md)|
|действия|[коллекция approvalStep](../resources/approvalstep.md)|Используется для представления решения, связанного с одним шагом в процессе утверждения, настроенного в [approvalStage.](../resources/approvalstage.md)|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|stages|[коллекция approvalStage](../resources/approvalstage.md)|Используется для **свойства approvalStages** параметров утверждения в свойстве **requestApprovalSettings** политики назначения [пакета доступа.](accesspackageassignmentpolicy.md) Указывает основные, откаты и утверждения эскалации на каждом этапе.|


## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "baseType": "microsoft.graph.entity",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "steps": [{
        "@odata.type": "#microsoft.graph.approvalStep"
    }]
}
```
