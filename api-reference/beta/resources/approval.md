---
title: Тип ресурса утверждения
description: Объект утверждения, связанный с accessPackageAssignmentRequest или userConsentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6f6751807f0dcb042958104c4b3146a555b22189
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945729"
---
# <a name="approval-resource-type"></a>Тип ресурса утверждения

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](entitlementmanagement-root.md)объект утверждения решений, связанных с `accessPackageAssignmentRequest` . Запрос на один шаг может иметь один шаг, связанный с ним, на который могут действовать одобрители. Кроме того, многоэтапный запрос может иметь несколько действий, связанных с ним, на которые могут действовать одобрители. Однако в многоэтапных утверждениях показаны как ожидающих, так и ранее завершенных действий.

В [userConsentRequests](../resources/userconsentrequest.md)объект утверждения решений, связанных с запросом.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Получить утверждение](../api/approval-get.md) | [утверждение](approval.md) | Извлечение свойств объекта **утверждения.** |


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор объекта утверждения.|
|действия|[коллекция approvalStep](../resources/approvalstep.md)|Используется для представления решения, связанного с одним шагом в процессе утверждения, настроенного в [approvalStage.](../resources/approvalstage.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|stages|[коллекция approvalStage](../resources/approvalstage.md)|Используется для **свойства approvalStages** параметров утверждения в свойстве **requestApprovalSettings** политики назначения [пакета доступа.](accesspackageassignmentpolicy.md) Указывает основные, откаты и утверждения эскалации на каждом этапе.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
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
