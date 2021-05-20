---
title: тип ресурса educationSubmission
description: Отправки принадлежат назначению. Представление представляет ресурсы, которые человек (или группа) включит для назначения, и возвращаемую оценку/обратную связь.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9450770a78b8effd1ad11717297a7e1ad7e6e874
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547678"
---
# <a name="educationsubmission-resource-type"></a>тип ресурса educationSubmission

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление представляет ресурсы, которые человек (или группа) включит для назначения, и результаты (например, оценки или отзывы), связанные с отправкой.

Отправки принадлежат назначению. Отправки создаются автоматически при публикации назначения. Отправка содержит два списка ресурсов. Ресурсы представляют рабочую зону пользователя или группы, а представленные ресурсы представляют ресурсы, которые активно были переданы учащимися.  

Свойство **status** является только для чтения, а объект перемещается через рабочий процесс с помощью действий. 

Если [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) не был вызван на ресурс **educationSubmission,** свойство **resourcesFolderUrl** `null` является .

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |Чтение свойств и связей объекта **educationSubmission.**|
|[Список ресурсов](../api/educationsubmission-list-resources.md) |[коллекция educationSubmissionResource](educationsubmissionresource.md)| Получите **коллекцию объектов educationSubmissionResource.**|
|[Список, представленныйРесурсеи](../api/educationsubmission-list-submittedresources.md) |[коллекция educationSubmissionResource](educationsubmissionresource.md)| Получите **коллекцию объектов educationSubmissionResource.**|
|[Результаты списка](../api/educationsubmission-list-outcomes.md) |[коллекция educationOutcome](educationoutcome.md)| Получите **коллекцию объектов educationOutcome.**|
|[возвращение](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|Учитель использует возврат, чтобы указать, что оценки/отзывы могут быть показаны учащемуся.|
|[setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) |[educationSubmission](educationsubmission.md) | Запуск создания папки SharePoint, в которой все ресурсы на основе файлов (Word, Excel и так далее) должны быть загружены для данной отправки. |
|[Отправить](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|Студент использует отправку для выполнения задания. Это скопирует ресурсы в **папку submittedResources** для классификации и обновляет состояние.|
|[ото всех](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Студент использует отгрузку, чтобы переместить состояние отправки из отправленной в рабочую. Это скопирует ресурсы в **папку workingResources** для классификации и обновляет состояние.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|получатель;|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Кто этому представлению назначено.|
|releasedBy (deprecated)|[identitySet](identityset.md)|Пользователь, переместивший состояние этой отправки в освобожденный.|
|releasedDateTime (отстает)|DateTimeOffset|Момент, когда отправка была выпущена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|returnedBy|[identitySet](identityset.md)|Пользователь, переместивший состояние этой отправки в возвращенный.|
|returnedDateTime|DateTimeOffset|Момент, когда отправка была возвращена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|resourcesFolderUrl|String|Папка, в которой необходимо хранить все ресурсы файла для этой отправки.|
|status|string| Только для чтения. Возможные значения: `working`, `submitted`, `released`, `returned`.|
|submittedBy|[identitySet](identityset.md)|Пользователь, переместивший ресурс в состояние отправленного.|
|submittedDateTime|DateTimeOffset|Момент времени, когда отправка была перенесена в состояние отправленного. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|unsubmittedBy|[identitySet](identityset.md)|Пользователь, переместивший ресурс из отправленного в рабочее состояние.|
|unsubmittedDateTime|DateTimeOffset|Момент времени, когда отправка была перенесена из представленного в рабочее состояние. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resources|[коллекция educationSubmissionResource](educationsubmissionresource.md)| Допускается значение null.|
|submittedResources|[коллекция educationSubmissionResource](educationsubmissionresource.md)| Только для чтения. Допускается значение null.|
|результаты|[коллекция educationOutcome.](educationOutcome.md) Содержит сведения о оценках, отзывах и/или рубриках, которые преподаватель назначает этому представлению.|Read-Write. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
    "id":"String (identifier)",
    "recipient":{"@odata.type":"microsoft.graph.educationSubmissionRecipient"},
    "returnedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "returnedDateTime":"String (timestamp)",
    "resourcesFolderUrl":"String",
    "status":"string",
    "submittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "submittedDateTime":"String (timestamp)",
    "unsubmittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "unsubmittedDateTime":"String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


