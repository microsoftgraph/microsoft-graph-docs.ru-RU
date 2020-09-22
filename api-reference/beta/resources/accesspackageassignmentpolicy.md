---
title: Тип ресурса Акцесспаккажеассигнментполици
description: Политика назначения пакетов Access определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ccf3e1bb94bb1f6186e39cdaa91fa2dbe3a4344d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031739"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>Тип ресурса Акцесспаккажеассигнментполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)политика назначения пакетов Access определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access. Пакет Access может иметь не более одного или нескольких политик. При получении запроса от субъекта субъект сравнивается с каждой политикой, чтобы найти политику (если она есть) с Рекуесторсеттингс, включающей в себя эту тему. После этого политика определяет, требуется ли для запроса утверждение, продолжительность назначения пакета Access, а также должно ли назначение регулярно проверяться.

Чтобы назначить пользователя пакету доступа, [Создайте акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) , который ссылается на политику назначения пакетов доступа и пакетов доступа.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список АкцесспаккажеассигнментполиЦиес](../api/accesspackageassignmentpolicy-list.md) | Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md) | Получение списка объектов Акцесспаккажеассигнментполици. |
| [Создание Акцесспаккажеассигнментполици](../api/accesspackageassignmentpolicy-post.md) | [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md) | Создание нового объекта Акцесспаккажеассигнментполици. |
| [Получение Акцесспаккажеассигнментполици](../api/accesspackageassignmentpolicy-get.md) | [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md) | Чтение свойств и связей объекта Акцесспаккажеассигнментполици. |
| [Обновление Акцесспаккажеассигнментполици](../api/accesspackageassignmentpolicy-update.md)|[акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md) | Обновление свойств объекта Акцесспаккажеассигнментполици. |
| [Удаление Акцесспаккажеассигнментполици](../api/accesspackageassignmentpolicy-delete.md) | | Удаление Акцесспаккажеассигнментполици. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|акцесспаккажеид|String|Идентификатор пакета Access.|
|акцессревиевсеттингс|[ассигнментревиевсеттингс](assignmentreviewsettings.md)|Кто должен проверить и как часто назначений для пакета доступа из этой политики. Это свойство имеет значение null, если проверка не требуются.|
|canExtend|Boolean|Указывает, может ли пользователь продлить продолжительность назначения пакета доступа после утверждения.|
|createdBy|String|Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|description|String|Описание политики.|
|displayName|String|Отображаемое имя политики.|
|дуратиониндайс|Int32|Количество дней, в течение которых назначения из этой политики последний раз до истечения срока действия.|
|expirationDateTime|DateTimeOffset|Срок действия для назначений, созданных в этой политике. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения.|
|модифиедби|String|Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|рекуестаппровалсеттингс|[аппровалсеттингс](approvalsettings.md)|Кто должен утверждать запросы на пакет Access в этой политике.|
|рекуесторсеттингс|[рекуесторсеттингс](requestorsettings.md)|Кто может запрашивать этот пакет Access из этой политики.|


## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|акцесспаккаже|[акцесспаккаже](accesspackage.md)| Пакет Access с этой политикой. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
    "displayName": "All Users",
    "description": "All users can request for access to the directory.",
    "isDenyPolicy": false,
    "canExtend": false,
    "durationInDays": 365,
    "requestorSettings" : {
      "scopeType": "AllExistingDirectorySubjects",
      "acceptRequests": true,
      "allowedRequestors": []
    },
    "requestApprovalSettings" : {
      "isApprovalRequired": false,
      "isApprovalRequiredForExtension": false,
      "isRequestorJustificationRequired": false,
      "approvalMode": "NoApproval",
      "approvalStages": []
    },
    "accessReviewSettings" : null
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


