---
title: тип ресурса accessPackageAssignmentPolicy
description: Политика назначения пакета доступа указывает политику, по которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0f0d6e7e90898592fbd3a1ba43a18e7953c4d892
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336391"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>тип ресурса accessPackageAssignmentPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-overview.md) политика назначения пакетов доступа указывает политику, по которой субъекты могут запрашивать или получать пакет доступа с помощью назначения пакета доступа. Пакет доступа может иметь нулевую или несколько политик. При получении запроса субъекта субъекту соответствует каждая политика, чтобы найти политику (если таково) с requestorSettings, которые включают этот субъект. Затем политика определяет, требуется ли для запроса утверждение, продолжительность назначения пакета доступа и требуется ли регулярное рассмотрение назначения.

Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md) , который ссылается на политику назначения пакета доступа и пакета доступа.


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
|displayName|String|Отображает имя политики. Поддерживает `$filter` (`eq`).|
|durationInDays|Int32|Количество дней, в течение которых назначения из этой политики будут выполняться до истечения срока их действия.|
|expirationDateTime|DateTimeOffset|Срок действия для назначений, созданных в этой политике. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String| Только для чтения.|
|modifiedBy|String|Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|requestApprovalSettings|[approvalSettings](approvalsettings.md)|Кто должны утверждать запросы на пакет доступа в этой политике.|
|requestorSettings|[requestorSettings](requestorsettings.md)|Кто этот пакет доступа можно запросить в этой политике.|
|вопросы|[коллекция accessPackageQuestion](accesspackagequestion.md)|Вопросы, заданные запросчику.|


## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| Пакет доступа с этой политикой. Только для чтения. Допускается значение null. Поддерживает `$expand`.|
|customExtensionHandlers|[коллекция customExtensionHandler](../resources/customextensionhandler.md)| Коллекция этапов выполнения одного или более пользовательских расширений рабочего процесса пакета доступа. Поддерживает `$expand`.| 



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
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "id": "String (identifier)",
  "accessPackageId": "String",
  "displayName": "String",
  "description": "String",
  "canExtend": "Boolean",
  "durationInDays": "Integer",
  "expirationDateTime": "String (timestamp)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "questions": [
    {
      "@odata.type": "microsoft.graph.accessPackageMultipleChoiceQuestion"
    }
  ],
  "requestorSettings": {
    "@odata.type": "microsoft.graph.requestorSettings"
  },
  "requestApprovalSettings": {
    "@odata.type": "microsoft.graph.approvalSettings"
  },
  "accessReviewSettings": {
    "@odata.type": "microsoft.graph.assignmentReviewSettings"
  }
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

