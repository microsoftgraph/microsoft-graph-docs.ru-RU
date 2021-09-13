---
title: тип ресурса educationSubmission
description: Представление представляет ресурсы, которые человек (или группа) включит для назначения, и результаты (например, оценки или отзывы), связанные с отправкой.
author: sharad-sharma-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8b309c887d431fd4b4f23fc6418965e5857d468e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123631"
---
# <a name="educationsubmission-resource-type"></a>тип ресурса educationSubmission

Пространство имен: microsoft.graph

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
|[Настройка папки определенных ресурсов для отправки](../api/educationsubmission-setupResourcesFolder.md) |[educationSubmission](educationsubmission.md) | Создайте SharePoint папку (в заранее определенном расположении) для отправки файлов в качестве ресурсов отправки. |
|[Отправить](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|Студент использует отправку для выполнения задания. Это скопирует ресурсы в **папку submittedResources** для классификации и обновляет состояние.|
|[ото всех](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Студент использует отгрузку, чтобы переместить состояние отправки из отправленной в рабочую. Это скопирует ресурсы в **папку workingResources** для классификации и обновляет состояние.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|получатель;|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Кто этому представлению назначено.|
|returnedBy|[identitySet](identityset.md)|Пользователь, переместивший состояние этой отправки в возвращенный.|
|returnedDateTime|DateTimeOffset|Момент, когда отправка была возвращена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|resourcesFolderUrl|Строка|Папка, в которой необходимо хранить все ресурсы файла для этой отправки.|
|status|string| Только для чтения. Возможные значения: `working`, `submitted`, `released`, `returned`.|
|submittedBy|[identitySet](identityset.md)|Пользователь, переместивший ресурс в состояние отправленного.|
|submittedDateTime|DateTimeOffset|Момент времени, когда отправка была перенесена в состояние отправленного. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|unsubmittedBy|[identitySet](identityset.md)|Пользователь, переместивший ресурс из отправленного в рабочее состояние.|
|unsubmittedDateTime|DateTimeOffset|Момент времени, когда отправка была перенесена из представленного в рабочее состояние. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="relationships"></a>Отношения
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


