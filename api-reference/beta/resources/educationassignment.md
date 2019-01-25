---
title: Тип ресурса educationAssignment
description: Представляет ресурс **educationAssignment** задачи или единицы трудозатрат, назначенных участником группы или учебы в классе как часть изучение. Только для преподавателей или владельцев группы могут создавать назначений. Назначения содержат раздаточные материалы и задачи, которые преподаватель хочет учебы для работы на. Каждое назначение учебы имеет связанные отправки, которая содержит все данные, которые их учитель предложено включены. Преподаватель можно добавить показатели и свои отзывы и предложения для предоставления включена по студента.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 68bb881800e1c63acb588e39bb64e1d02e005cc3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508960"
---
# <a name="educationassignment-resource-type"></a>Тип ресурса educationAssignment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурс **educationAssignment** задачи или единицы трудозатрат, назначенных участником группы или учебы в классе как часть изучение. Только для преподавателей или владельцев группы могут создавать назначений. Назначения содержат раздаточные материалы и задачи, которые преподаватель хочет учебы для работы на. Каждое назначение учебы имеет связанные [отправки](educationsubmissionresource.md) , который содержит все данные, которые их учитель предложено включены. Преподаватель можно добавить показатели и свои отзывы и предложения для предоставления включена по студента.

При создании назначения находится в состоянии черновика. Студентов не могут просматривать назначения и отправка сообщений о не будут созданы. Состояние назначения можно изменить с помощью действия [публикации](../api/educationassignment-publish.md) . Запрос на исправление нельзя использовать для изменения состояния назначения.

Назначение API-интерфейсы, предоставляемые в пространстве имен классов.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение назначения](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Чтение свойства и связи объекта **educationAssignment** .|
|[Создание назначения ресурсов](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| Создайте новый **educationAssignmentResource** , отправку сообщений в коллекцию ресурсов.|
|[Список ресурсов](../api/educationassignment-list-resources.md) |[educationAssignmentResource](educationassignmentresource.md) коллекции| Получение коллекции объектов **educationAssignmentResource** .|
|[Отправка сообщений о списка](../api/educationassignment-list-submissions.md) |[educationSubmission](educationsubmission.md) коллекции| Получение коллекции объектов **educationSubmission** .|
|[Update](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |Обновление объекта **educationAssignment** . |
|[Delete](../api/educationassignment-delete.md) | Нет |Удаление объекта **educationAssignment** . |
|[Publish](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|Измените состояние объекта **educationAssignment** из черновика для публикации.|
|[Получение URL-адрес папки ресурсов](../api/educationassignment-getresourcesfolderurl.md)| string| Папка OneDrive, в котором необходимо разместить файловым ресурсам входить в состав назначения ресурса. Файлы должны быть расположены в папке будет добавлена в качестве ресурса.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения.|
|allowLateSubmissions|Логическое| Определяет ли студентов можно отправлять после даты выполнения. Если это свойство не указан во время создания, по умолчанию используется значение true. |
|allowStudentsToAddResourcesToSubmission|Логическое| Определяет ли студентов может добавлять собственные ресурсы отправку или если они можно изменять только ресурсы, добавленные преподаватель. |
|assignDateTime|DateTimeOffset|Дата, когда назначение станет активной.  Если в будущем, назначение не отображается для студента до указанной даты.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| Какие пользователи или всего класса должны получить объект отправки после публикации назначения. |
|assignedDateTime|DateTimeOffset|Тогда, когда назначения была опубликована для студентов и назначения отображается на временной шкалы студентов.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|classId|String| Класс, которому принадлежит этот назначения. |
|createdBy|[identitySet](identityset.md)| Создатель назначения. |
|createdDateTime|DateTimeOffset|Тогда, когда при создании назначения.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|displayName|String|Имя назначения.|
|dueDateTime|DateTimeOffset|Дата назначения студентов срок выполнения.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Оценка успеваемости|[educationAssignmentGradeType](educationassignmentgradetype.md)|Как будет выражаемым числом назначения. |
|Инструкции|[itemBody](itembody.md)| Инструкции для назначения.  Это вместе с отображаемым именем сообщить студент возможные действия. |
|lastModifiedBy|[identitySet](identityset.md)| Кто последнего изменения назначения. |
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения назначения некоторое время.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|status|string| Состояние **назначения**.  Вы не можете применить исправление это значение.  Возможные значения: `draft`, `published`, `assigned`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resources|[educationAssignmentResource](educationassignmentresource.md) коллекции| Изучение объектов, которые связаны с этой назначения.  Только учителя можно изменить этот список. Допускается значение null.|
|сданные работы.|[educationSubmission](educationsubmission.md) коллекции| После публикации существует объект отправки для каждого student, представляющее марки и работе.  Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "String (timestamp)",
  "classId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "dueDateTime": "String (timestamp)",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "instructions": {"@odata.type": "microsoft.graph.itemBody"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
