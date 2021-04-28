---
title: тип ресурса approvalStep
description: Объект approvalStep, связанный с accessPackageAssignmentRequest или userConsentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 413af698c72be945e648a3fe21ce772f2b4e6102
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061877"
---
# <a name="approvalstep-resource-type"></a>тип ресурса approvalStep

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](entitlementmanagement-root.md)объект approvalStep для решений, связанных с `accessPackageAssignmentRequest` . Он используется для различия решений для различных действий рабочего процесса утверждения, на которые могут действовать одобрители.

В [userConsentRequests](../resources/userconsentrequest.md)решения об утверждении, связанные с запросом.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Утверждение спискаSteps](../api/approval-list-steps.md) | [коллекция approvalStep](approvalstep.md) | Список объектов **approvalStep,** связанных с объектом **утверждения.** |
|[Получить утверждениеStep](../api/approvalstep-get.md) | [approvalStep](approvalstep.md) | Извлечение свойств объекта **approvalStep.** |
|[Обновление approvalStep](../api/approvalstep-update.md) | Нет | Применить утверждение или отказ в принятии решения по **объекту approvalStep.** |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignedToMe|Логический|Указывает, назначен ли шаг пользователю вызова для проверки. Только для чтения.|
|displayName|String|Метка, предоставленная создателем политики для определения шага утверждения. Только для чтения.|
|id|String|Идентификатор шага, связанного с объектом утверждения. Только для чтения.|
|обоснование|String|Обоснование, связанное с решением о шаге утверждения.|
|reviewResult|String|Результат этой записи утверждения. Возможные значения: `NotReviewed` , `Approved` , `Denied` .|
|reviewedBy|[коллекция userIdentity](useridentity.md) | Идентификатор рецензента. Только для чтения.|
|reviewedDateTime|DateTimeOffset|Дата и время записи решения. Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|status|String|Состояние шага. Возможные значения: `InProgress` `Initializing` , , `Completed` `Expired` . Только для чтения.|


## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|утверждение|[коллекция утверждений](../resources/approval.md)|Объект утверждения решений, связанных с `accessPackageAssignmentRequest` .|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStep",
}
-->
``` json
{
   "@odata.type":"#microsoft.graph.approvalStep",
   "id":"String (identifier)",
   "displayName":"String",
   "status":"String",
   "assignedToMe":true,
   "reviewedBy": [{"@odata.type": "microsoft.graph.userIdentity"}],
   "reviewedDateTime":"String (timestamp)",
   "reviewResult":"String",
   "justification":"String"
}
```
