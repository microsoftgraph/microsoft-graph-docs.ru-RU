---
title: Тип ресурса educationSubmission
description: Отправка сообщений о принадлежат назначения. Отправка представляет ресурсы, отдельных пользователей (или групп) включить в для назначения и марки/отзыв, который возвращается.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: aeeb1355da2ffcb0ebf561af2ecd15ac93221e26
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521427"
---
# <a name="educationsubmission-resource-type"></a>Тип ресурса educationSubmission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отправка сообщений о принадлежат назначения. Отправка представляет ресурсы, отдельных пользователей (или групп) включить в для назначения и марки/отзыв, который возвращается.
Отправка сообщений о создаются автоматически при публикации назначения. Отправка несет ответственность за два списка ресурсов. Ресурсы представляют работу область, пока отправляемого ресурсы предоставляют ресурсы, которые активно была отключена с студентов пользователей и групп.  

>**Примечание:** Состояние только для чтения и объект перемещается через рабочего процесса с помощью действия. 

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |Чтение свойства и связи объекта **educationSubmission** .|
|[Список ресурсов](../api/educationsubmission-list-resources.md) |[educationSubmissionResource](educationsubmissionresource.md) коллекции| Получение коллекции объектов **educationSubmissionResource** .|
|[Список submittedResources](../api/educationsubmission-list-submittedresources.md) |[educationSubmissionResource](educationsubmissionresource.md) коллекции| Получение коллекции объектов **educationSubmissionResource** .|
|[Update](../api/educationsubmission-update.md) | [educationSubmission](educationsubmission.md) |Обновление объекта **educationSubmission** . |
|Возврат|[educationSubmission](educationsubmission.md)|Преподаватель использует return для указания, что оценки и отзывы будут показаны студента.|
|submit|[educationSubmission](educationsubmission.md)|Отправка используется для включения в назначении студента. Это будет копировать ресурсы в папке **submittedResources** для ранжирования и обновляет сведения о состоянии.|
|[Unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Студента использует unsubmit для перемещения state подачи из добавленных назад в рабочее. Это будет копировать ресурсы в папке **workingResources** для ранжирования и обновляет сведения о состоянии.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Отзывы|[educationFeedback](educationfeedback.md)|Содержит свойство свои отзывы и предложения, которое хранит учителя примечания к студентов.|
|оценка|[educationAssignmentGrade](educationassignmentgrade.md)|Содержит сведения о марки назначает преподавателей для этой отправки.|
|id|String| Только для чтения.|
|Recipient|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Назначенный этой отправки.|
|Выпустил|[identitySet](identityset.md)|Пользователь, который перемещены состояние в этом отправки освободить.|
|releasedDateTime|DateTimeOffset|Момент времени, когда была выпущена подачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|returnedBy|[identitySet](identityset.md)|Пользователь, который перемещены состояние в этом отправки возвращено.|
|returnedDateTime|DateTimeOffset|Момент времени, когда был возвращен подачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|resourcesFolderUrl|String|Папка, где должны храниться все файловые ресурсы в этом отправки.|
|status|string| Только для чтения. Возможные значения: `working`, `submitted`, `released`, `returned`.|
|submittedBy|[identitySet](identityset.md)|Пользователь, который перемещены в отправленных состояние ресурса.|
|submittedDateTime|DateTimeOffset|Момент времени, когда подачи был перемещен в отправленных состояние. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|unsubmittedBy|[identitySet](identityset.md)|Пользователь, перемещены ресурса из отправленных в рабочее состояние.|
|unsubmittedDateTime|DateTimeOffset|Момент времени, когда подачи был перемещен из отправленных в рабочее состояние. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resources|[educationSubmissionResource](educationsubmissionresource.md) коллекции| Допускается значение null.|
|submittedResources|[educationSubmissionResource](educationsubmissionresource.md) коллекции| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "grade": {"@odata.type": "microsoft.graph.educationAssignmentGrade"},
  "id": "String (identifier)",
  "recipient": {"@odata.type": "microsoft.graph.educationSubmissionRecipient"},
  "returnedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "returnedDateTime": "String (timestamp)",
  "resourcesFolderUrl": "String",
  "status": "string",
  "submittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "submittedDateTime": "String (timestamp)",
  "unsubmittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "unsubmittedDateTime": "String (timestamp)"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
