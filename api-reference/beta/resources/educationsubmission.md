---
title: Тип ресурса educationSubmission
description: Отправка сообщений о принадлежат назначения. Отправка представляет ресурсы, отдельных пользователей (или групп) включить в для назначения и марки/отзыв, который возвращается.
ms.openlocfilehash: f0b1cc9ccd169d29c31eb96bb6305f6d7cdcd6b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075481"
---
# <a name="educationsubmission-resource-type"></a>Тип ресурса educationSubmission

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
|[Возврат](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|Преподаватель использует return для указания, что оценки и отзывы будут показаны студента.|
|[Отправить](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|Отправка используется для включения в назначении студента. Это будет копировать ресурсы в папке **submittedResources** для ранжирования и обновляет сведения о состоянии.|
|[Unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Студента использует unsubmit для перемещения state подачи из добавленных назад в рабочее. Это будет копировать ресурсы в папке **workingResources** для ранжирования и обновляет сведения о состоянии.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|свои отзывы и предложения|[educationFeedback](educationfeedback.md)|Содержит свойство свои отзывы и предложения, которое хранит учителя примечания к студентов.|
|оценка|[educationAssignmentGrade](educationassignmentgrade.md)|Содержит сведения о марки назначает преподавателей для этой отправки.|
|id|String| Только для чтения.|
|Получатель|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Назначенный этой отправки.|
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

## <a name="relationships"></a>Связи
| Связь | Тип   |Description|
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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->