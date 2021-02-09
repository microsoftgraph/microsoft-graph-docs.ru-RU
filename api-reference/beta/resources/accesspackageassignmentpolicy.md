---
title: Тип ресурса accessPackageAssignmentPolicy
description: Политика назначения пакета доступа определяет политику, с помощью которой субъекты могут запрашивать или получать доступ к пакету доступа через назначение пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 34716752715399d1e16f7edeb609eace4c9b9b0b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155617"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>Тип ресурса accessPackageAssignmentPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](entitlementmanagement-root.md)политика назначения пакета доступа определяет политику, с помощью которой субъекты могут запрашивать или получать пакет доступа через назначение пакета доступа. Пакет доступа может иметь ноль или несколько политик. При получении запроса от субъекта тема со встречена с каждой политикой, чтобы найти политику (если таково) с requestorSettings, включающие эту тему. Затем политика определяет, требуется ли утверждение запроса, продолжительность назначения пакета доступа и требуется ли регулярно проверять назначение.

Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/accesspackageassignmentrequest-post.md) который ссылается на пакет доступа и политику назначения пакета доступа.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | [Коллекция accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Получить список объектов accessPackageAssignmentPolicy. |
| [Создание accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Создание объекта accessPackageAssignmentPolicy. |
| [Get accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Чтение свойств и связей объекта accessPackageAssignmentPolicy. |
| [Обновление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | Обновление свойств объекта accessPackageAssignmentPolicy. |
| [Удаление accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | Удаление accessPackageAssignmentPolicy. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageId|String|ИД пакета доступа.|
|accessReviewSettings|[assignmentReviewSettings](assignmentreviewsettings.md)|Кто должен и как часто проверяются назначения пакета доступа из этой политики. Это свойство имеет null, если проверки не требуются.|
|canExtend|Boolean|Указывает, может ли пользователь продлить срок назначения пакета доступа после утверждения.|
|createdBy|String|Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|description|String|Описание политики.|
|displayName|String|Отображаемого имени политики.|
|durationInDays|Int32|Количество дней, в течение которых назначения из этой политики продлятся до истечения срока их действия.|
|expirationDateTime|DateTimeOffset|Дата окончания срока действия для назначений, созданных в этой политике. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|modifiedBy|String|Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|requestApprovalSettings|[approvalSettings](approvalsettings.md)|Кто должен утверждать запросы на пакет доступа в этой политике.|
|requestorSettings|[requestorSettings](requestorsettings.md)|Кто может запросить этот пакет доступа из этой политики.|
|вопросы|[Коллекция accessPackageQuestion](accesspackagequestion.md)|Вопросы, которые представляют запросителем.|


## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| Пакет доступа с этой политикой. Только для чтения. Допускается значение null.|

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

