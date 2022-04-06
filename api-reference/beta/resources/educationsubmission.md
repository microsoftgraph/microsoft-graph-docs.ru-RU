---
title: Тип ресурса educationSubmission
description: Представляет ресурсы, которые пользователь (или группа) отправляет для назначения, и результаты (например, оценки или отзывы), связанные с отправкой.
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 12618b5a852755f9c478896b6088aa1d6836a549
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685063"
---
# <a name="educationsubmission-resource-type"></a>Тип ресурса educationSubmission

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурсы, которые отдельный (или группа) совмещая [](educationassignment.md) с заданием, и результаты (например, оценки или отзывы), связанные с **отправкой**.

Отправки принадлежат **назначению**. Отправки создаются автоматически при **публикации** назначения. **Отправка** содержит два списка ресурсов. Ресурсы представляют рабочую область пользователя или группы, а отправленные ресурсы — ресурсы, которые активно сданы учащимися.  

Свойство **состояния** доступно только для чтения, а объект перемещается через рабочий процесс с помощью действий. 

Если [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) не был вызван для ресурса **educationSubmission** , свойство **resourcesFolderUrl** имеет значение `null`.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |Чтение свойств и связей объекта **educationSubmission** .|
|[Перечисление ресурсов](../api/educationsubmission-list-resources.md) |[Коллекция educationSubmissionResource](educationsubmissionresource.md)| Получение коллекции **объектов educationSubmissionResource** .|
|[Перечисление submittedResources](../api/educationsubmission-list-submittedresources.md) |[Коллекция educationSubmissionResource](educationsubmissionresource.md)| Получение коллекции **объектов educationSubmissionResource** .|
|[Перечисление результатов](../api/educationsubmission-list-outcomes.md) |[Коллекция educationOutcome](educationoutcome.md)| Получение коллекции **объектов educationOutcome** .|
|[Вернуться](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|Преподаватель использует возврат, чтобы указать, что оценки и отзывы могут отображаться для учащегося.|
|[Переназначить](../api/educationsubmission-reassign.md)|[educationSubmission](educationsubmission.md)|Переназначьте отправку учащемуся с отзывом для проверки.|
|[Настройка папки ресурсов для отправки](../api/educationsubmission-setupResourcesFolder.md) |[educationSubmission](educationsubmission.md) | Создайте SharePoint папку (в предварительно определенном расположении) для отправки файлов в качестве ресурсов отправки. |
|[Отправить](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|Учащийся использует отправку для с подачи **задания**. Это приведет к копированию ресурсов в **папку submittedResources** для проверки и обновлению состояния.|
|[отмена отправки](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Учащийся использует отмену подписки, чтобы переместить состояние отправки из отправленной в рабочую. Это приведет к копированию ресурсов в папку **workingResources** для проверки и обновлению состояния.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String|Уникальный идентификатор для отправки.|
|получатель;|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Кто назначена эта отправка.|
|returnedBy|[identitySet](identityset.md)|Пользователь, переместивший состояние этой отправки в возвращенное.|
|returnedDateTime|DateTimeOffset|Момент времени, когда была возвращена отправка. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|resourcesFolderUrl|String|Папка, в которой должны храниться все файловые ресурсы для этой отправки.|
|status|educationSubmissionStatus| Только для чтения. Возможные значения: , , , `released`, и `unknownFutureValue` `returned``reassigned`. `submitted``working` Обратите внимание, что для `Prefer: include-unknown-enum-members` получения следующих значений в этом развиваемом перечислении необходимо использовать заголовок [запроса](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). `reassigned`|
|submittedBy|[identitySet](identityset.md)|Пользователь, переместивший ресурс в отправленное состояние.|
|submittedDateTime|DateTimeOffset|Момент времени, когда отправка была перемещена в отправленное состояние. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|unsubmittedBy|[identitySet](identityset.md)|Пользователь, переместивший ресурс из отправленного в рабочее состояние.|
|unsubmittedDateTime|DateTimeOffset|Момент времени, когда отправка была перемещена из отправленного в рабочее состояние. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|reassignedBy|[identitySet](identityset.md)|Пользователь, который переназначит состояние этой отправки.|
|reassignedDateTime|DateTimeOffset|Момент времени, когда отправка была переназначена. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resources|[Коллекция educationSubmissionResource](educationsubmissionresource.md)| Допускается значение null.|
|submittedResources|[Коллекция educationSubmissionResource](educationsubmissionresource.md)| Только для чтения. Допускается значение null.|
|Результаты|[коллекция educationOutcome](educationOutcome.md) . Содержит сведения о оценках, отзывах и (или) rubrics, которые преподаватель назначает этой отправке.|Чтение и запись. Допускается значение null.|

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
    "unsubmittedDateTime":"String (timestamp)",
    "reassignedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "reassignedDateTime":"String (timestamp)"
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


