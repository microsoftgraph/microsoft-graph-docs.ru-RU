---
title: тип ресурса accessPackageAssignmentRequest
description: Запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 83218058d375a9f78a24b2af837c39fb5ee77a2c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720440"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>тип ресурса accessPackageAssignmentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем или от имени пользователя, который хочет получить назначение пакета доступа. Если запрос является успешным, с любыми необходимыми утверждениями, пользователь получает назначение пакета доступа и является субъектом этого назначения пакета доступа.  Azure AD также создает запросы на назначение пакетов доступа автоматически для отслеживания удаления доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [accessPackageAssignmentRequest collection](accesspackageassignmentrequest.md) | Извлечение списка объектов accesspackageassignmentrequest. |
| [Создание accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Создание нового accessPackageAssignmentRequest. |
| [Получить accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | Чтение свойств и связей объекта accessPackageAssignmentRequest. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|completedDate|DateTimeOffset|Дата окончания обработки , успешной или неудачной, запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|id|String| Только для чтения.|
|isValidationOnly|Boolean|True, если запрос не обрабатывается для назначения.|
|обоснование|String|Предоставлено обоснование запроса.|
|requestState|String|Один `PendingApproval` из `Canceled` , , , , , или  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` . Только для чтения.|
|requestStatus|String|Дополнительные сведения о состоянии обработки запросов. Только для чтения.|
|requestType|String|Один `UserAdd` из `UserRemove` , , или `AdminAdd` `AdminRemove` `SystemRemove` . Запрос от самого пользователя будет иметь requestType или `UserAdd` `UserRemove` . Только для чтения.|
|schedule|[requestSchedule](requestschedule.md)| Диапазон дат, которые должен быть назначен запросчику. Только для чтения.|
|accessPackageAssignment|[accessPackageAssignment](accesspackageassignment.md)| Для requestType или , это назначение пакета `UserAdd` `AdminAdd` доступа, запрашиваемого для создания.  Для requestType или , это свойство существующего `UserRemove` `AdminRemove` `SystemRemove` `id` назначения, которые будут удалены.|
|ответы|[коллекция accessPackageAnswer](accesspackageanswer.md)|Ответы, предоставленные запрашивателем для [доступа кPackageQuestions,](accesspackagequestion.md) заданные им во время запроса.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|запросчик|[accessPackageSubject](accesspackagesubject.md)| Субъекту, который запрашивал или, если прямое назначение, было назначено. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
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

