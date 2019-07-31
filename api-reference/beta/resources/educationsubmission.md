---
title: Тип ресурса educationSubmission
description: Для отправки используются назначения. Отправка представляет ресурсы, которые может включить отдельный (или группа) для назначения, а также возвращаемую оценку или отзыв.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 81c194c08ddc5ed8f5acc38ae84a5478bb7e0229
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972525"
---
# <a name="educationsubmission-resource-type"></a>Тип ресурса educationSubmission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для отправки используются назначения. Отправка представляет ресурсы, которые может включить отдельный (или группа) для назначения, а также возвращаемую оценку или отзыв.
При публикации назначения автоматически создаются отправки. Отправка владеет двумя списками ресурсов. Ресурсы представляют рабочую область пользователей и групп, а предоставленные ресурсы представляют ресурсы, которые активно включены студентами.  

>**Примечание:** Состояние доступно только для чтения, и объект перемещается через рабочий процесс с помощью действий. 

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |Чтение свойств и связей объекта **educationSubmission** .|
|[Список ресурсов](../api/educationsubmission-list-resources.md) |Коллекция [едукатионсубмиссионресаурце](educationsubmissionresource.md)| Получение коллекции объектов **едукатионсубмиссионресаурце** .|
|[Список Субмиттедресаурцес](../api/educationsubmission-list-submittedresources.md) |Коллекция [едукатионсубмиссионресаурце](educationsubmissionresource.md)| Получение коллекции объектов **едукатионсубмиссионресаурце** .|
|[обновление](../api/educationsubmission-update.md); | [educationSubmission](educationsubmission.md) |Обновление объекта **educationSubmission** . |
|[Передачи](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|Преподаватель использует возврат, чтобы показать, что оценки и отзывы могут отображаться для учащегося.|
|[Отправить](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|Для включения назначения учащийся использует функцию "послать". При этом ресурсы будут скопированы в папку **субмиттедресаурцес** для ступенчатого и обновления состояния.|
|[Отправляются](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Учащийся использует unsubmit, чтобы переместить состояние отправки от отправки к работе. При этом ресурсы будут скопированы в папку **воркингресаурцес** для ступенчатого и обновления состояния.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|feedback|[Едукатионфидбакк](educationfeedback.md)|Содержит свойство feedback, которое хранит заметки преподавателя обратно в учащихся.|
|оценка|[Едукатионассигнментграде](educationassignmentgrade.md)|Содержит сведения об оценках, которые применяют преподаватель для этой отправки.|
|id|String| Только для чтения.|
|получатель;|[ЕдукатионсубмиссионреЦипиент](educationsubmissionrecipient.md)|, Которому назначена эта отправка.|
|Релеаседби|[identitySet](identityset.md)|Пользователь, который изменил состояние этой отправки на "выпущено".|
|Релеаседдатетиме|DateTimeOffset|Момент времени, когда была выпущена отправка. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Ретурнедби|[identitySet](identityset.md)|Пользователь, который изменил состояние этой отправки на "возвращено".|
|Ретурнеддатетиме|DateTimeOffset|Момент времени, когда была возвращена отправка. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Ресаурцесфолдерурл|String|Папка, в которой должны храниться все файловые ресурсы для этой отправки.|
|status|string| Только для чтения. Возможные значения: `working`, `submitted`, `released`, `returned`.|
|Субмиттедби|[identitySet](identityset.md)|Пользователь, который переместил ресурс в отправленное состояние.|
|Субмиттеддатетиме|DateTimeOffset|Момент времени, когда отправка была перемещена в состояние отправлено. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Унсубмиттедби|[identitySet](identityset.md)|Пользователь, который переместит ресурс в рабочее состояние.|
|Унсубмиттеддатетиме|DateTimeOffset|Момент времени, когда отправка перемещается из состояния отправки в рабочее состояние. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|resources|Коллекция [едукатионсубмиссионресаурце](educationsubmissionresource.md)| Допускается значение null.|
|Субмиттедресаурцес|Коллекция [едукатионсубмиссионресаурце](educationsubmissionresource.md)| Только для чтения. Допускается значение null.|

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
    "feedback":{"@odata.type":"microsoft.graph.educationFeedback"},
    "grade":{"@odata.type":"microsoft.graph.educationAssignmentGrade"},
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
    "releasedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "releasedDateTime":"String (timestamp)"
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
