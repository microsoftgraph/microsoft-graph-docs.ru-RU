---
title: Тип ресурса accessPackageAssignmentRequest
description: Запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9ecaa9b77a92dc6393b3c7231976937e36502c8d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719757"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>Тип ресурса accessPackageAssignmentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа, или от его имени. В случае успешного выполнения запроса с любыми необходимыми утверждениями пользователь получает назначение пакета доступа и является субъектом этого назначения пакета доступа.  Azure AD также автоматически создает запросы на назначение пакета доступа для отслеживания удаления доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [Коллекция accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Получить список объектов accesspackageassignmentrequest. |
| [Создание accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Создайте новый accessPackageAssignmentRequest. |
| [Get accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Чтение свойств и связей объекта accessPackageAssignmentRequest. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|completedDate|DateTimeOffset|Дата окончания обработки (успешного или неудачного) запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|id|String| Только для чтения.|
|isValidationOnly|Boolean|Имеет true, если запрос не обрабатывается для назначения.|
|обоснование|String|Предоставленная запросителем обоснование.|
|requestState|String|Один из `PendingApproval` , , , или `Canceled`  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` . Только для чтения.|
|requestStatus|String|Дополнительные сведения о состоянии обработки запроса. Только для чтения.|
|requestType|String|Один из `UserAdd` , , , или `UserRemove` `AdminAdd` `AdminRemove` `SystemRemove` . Запрос от самого пользователя будет иметь requestType или `UserAdd` `UserRemove` . Только для чтения.|
|schedule|[requestSchedule](requestschedule.md)| Диапазон дат, в которые должен быть назначен доступ запрашиваемой информации. Только для чтения.|
|accessPackageAssignment|[accessPackageAssignment](accesspackageassignment.md)| Для requestType или , это назначение пакета доступа `UserAdd` `AdminAdd` запрашивается для создания.  Для объекта requestType или , это свойство существующего `UserRemove` `AdminRemove` `SystemRemove` `id` назначения, который необходимо удалить.|
|answers|[Коллекция accessPackageAnswer](accesspackageanswer.md)|Ответы, предоставленные запрашивателем [для accessPackageQuestions,](accesspackagequestion.md) которые запрашивали их во время запроса.|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|requestor|[accessPackageSubject](accesspackagesubject.md)| Субъект, запросивший или, если прямое назначение, был назначен. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "createdDateTime": "string",
    "completedDate": "string",
    "id": "string",
    "requestType": "string",
    "requestState": "string",
    "requestStatus": "string",
    "isValidationOnly": false,
    "justification": "string",
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "string",
        "answeredQuestion": {
            "id": "string",
            "text": {
                "defaultText": "string",
                "localizedTexts": [{
                    "text": "string",
                    "languageCode": "string"
                }]
            },
            "isRequired": true,
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": true
        }
    }]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

