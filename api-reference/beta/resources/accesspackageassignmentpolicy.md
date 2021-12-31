---
title: тип ресурса accessPackageAssignmentPolicy
description: Политика назначения пакета доступа указывает политику, по которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9045cc88e5e68fd49e85b8333c035cabba2bc5b9
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651262"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>тип ресурса accessPackageAssignmentPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](entitlementmanagement-overview.md)политика назначения пакетов доступа указывает политику, в которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа. Пакет доступа может иметь нулевую или несколько политик. При получении запроса субъекта субъекту соответствует каждая политика, чтобы найти политику (если таково) с requestorSettings, которые включают этот субъект. Затем политика определяет, требуется ли для запроса утверждение, продолжительность назначения пакета доступа и требуется ли регулярное рассмотрение назначения.

Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/entitlementmanagement-post-accesspackageassignmentrequests.md) который ссылается на политику назначения пакета доступа и пакета доступа.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackageAssignmentPolicies](../api/entitlementmanagement-list-accesspackageassignmentpolicies.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection | Извлечение списка объектов accessPackageAssignmentPolicy. |
| [Создание accessPackageAssignmentPolicy](../api/entitlementmanagement-post-accesspackageassignmentpolicies.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Создание нового объекта accessPackageAssignmentPolicy. |
| [Получить accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Чтение свойств и связей объекта accessPackageAssignmentPolicy. |
| [Обновление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Обновление свойств объекта accessPackageAssignmentPolicy. |
| [Удаление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | Удаление accessPackageAssignmentPolicy. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageId|Строка|Идентификатор пакета доступа.|
|accessReviewSettings|[assignmentReviewSettings](assignmentreviewsettings.md)|Кто должны проанализировать и как часто назначения пакета доступа из этой политики. Это свойство является null, если отзывы не требуются.|
|canExtend|Boolean|Указывает, может ли пользователь продлить срок назначения пакета доступа после утверждения.|
|createdBy|String|Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|description|Строка|Описание политики.|
|displayName|Строка|Отображает имя политики. Поддерживает `$filter` (`eq`).|
|durationInDays|Int32|Количество дней, в течение которых назначения из этой политики будут выполняться до истечения срока их действия.|
|expirationDateTime|DateTimeOffset|Срок действия для назначений, созданных в этой политике. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String| Только для чтения.|
|modifiedBy|String|Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|requestApprovalSettings|[approvalSettings](approvalsettings.md)|Кто должны утверждать запросы на пакет доступа в этой политике.|
|requestorSettings|[requestorSettings](requestorsettings.md)|Кто этот пакет доступа можно запросить в этой политике.|
|вопросы|[коллекция accessPackageQuestion](accesspackagequestion.md)|Вопросы, заданные запросчику.|


## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| Пакет доступа с этой политикой. Только для чтения. Допускается значение null. Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "string",
    "accessPackageId": "string",
    "displayName": "string",
    "description": "string",
    "isDenyPolicy": false,
    "canExtend": false,
    "durationInDays": 365,
    "requestorSettings": {
        "scopeType": "string",
        "acceptRequests": true,
        "allowedRequestors": [{
            "@odata.type": "#microsoft.graph.userSet"
        }]
    },
    "requestApprovalSettings": {
        "isApprovalRequired": false,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": false,
        "approvalMode": "string",
        "approvalStages": [{
            "approvalStageTimeOutInDays": 14,
            "isApproverJustificationRequired": true,
            "isEscalationEnabled": true,
            "escalationTimeInMinutes": 11520,
            "primaryApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }],
            "escalationApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }]
        }]
    },
    "accessReviewSettings": null,
    "questions": [{
        "@odata.type": "#microsoft.graph.question"
    }]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

