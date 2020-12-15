---
title: Тип ресурса educationAssignment
description: Ресурс **educationAssignment** представляет задачу или единицу работы, назначенную учащемуся или участнику группы в классе в рамках своего обучения. Только преподаватели или владельцы команд могут создавать задания. Задания содержат раздатки и задачи, над которые преподаватель хочет работать. Каждое назначение учащегося имеет связанную отправку, которая содержит любые трудоемкие задачи, которые его преподаватель хочет включить. Преподаватель может добавлять оценки и отзывы в отправку, включенную учащимся.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5215a1a36664216d680d07187514ebed69ba0b84
ms.sourcegitcommit: 86d427ac670ebc3fdcf8e06541218bb74d39279d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49675999"
---
# <a name="educationassignment-resource-type"></a>Тип ресурса educationAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **educationAssignment** представляет задачу или единицу работы, назначенную учащемуся или участнику группы в классе в рамках своего обучения. Только преподаватели или владельцы команд могут создавать задания. Задания содержат раздатки и задачи, над которые преподаватель хочет работать. Каждое назначение учащегося имеет связанную [отправку,](educationsubmissionresource.md) которая содержит любые трудоемкие задачи, которые его преподаватель хочет включить. Преподаватель может добавлять оценки и отзывы в отправку, включенную учащимся.

После создания назначения оно находится в состоянии черновика. Учащиеся не могут видеть назначение и отправки не будут созданы. Состояние назначения можно изменить с помощью действия [публикации.](../api/educationassignment-publish.md) Изменить состояние назначения с помощью запроса PATCH нельзя.

API назначения могут быть открыты в пространстве имен класса.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список ресурсов](../api/educationassignment-list-resources.md) |[Коллекция educationAssignmentResource](educationassignmentresource.md)| Получите **коллекцию объектов educationAssignmentResource.**|
|[Отправки списков](../api/educationassignment-list-submissions.md) |[коллекция educationSubmission](educationsubmission.md)| Получите **коллекцию объектов educationSubmission.**|
|[Перечисление категорий](../api/educationassignment-list-categories.md) |[коллекция educationCategory](educationcategory.md)| Получите **коллекцию объектов educationCategory.**|
|[Создание ресурса задания](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| Создание нового **educationAssignmentResource путем** публикации в коллекции ресурсов.|
|[Получение задания](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Чтение свойств и связей объекта **educationAssignment.**|
|[Обновление](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |Обновление объекта **educationAssignment.** |
|[удаление](../api/educationassignment-delete.md); | Нет |Удаление объекта **educationAssignment.** |
|[Добавление категорий](../api/educationassignment-add-categories.md) |[educationCategory](educationcategory.md) | **Назначьте этому назначению educationCategory,** принадлежащее классу.|
|[Удаление категории](../api/educationassignment-remove-category.md) |Нет| Удалите **из этого задания educationCategory,** принадлежащего классу.|
|[Прикрепление рубрики](../api/educationassignment-put-rubric.md)|Нет|Присоединить существующее **educationRubric** к этому назначению.|
|[Удаление рубрики](../api/educationassignment-delete-rubric.md)|Нет|**Отсоединять educationRubric** от этого назначения.|
|[публикация](../api/educationassignment-publish.md);|[educationAssignment](educationassignment.md)|Измените состояние объекта **educationAssignment** с черновика на опубликованное.|
|[Получение URL-адреса папки ресурсов](../api/educationassignment-getresourcesfolderurl.md)| Строка| Папка OneDrive, в которую следует поместить ресурсы на основе файлов, чтобы быть частью ресурса назначения. Файлы должны быть расположены в этой папке, чтобы добавить их в качестве ресурса.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения.|
|addedStudentAction|String|Необязательное поле для управления поведением заданий для учащихся, добавляемого после публикации задания. Если значение не указано, по умолчанию `none` задано значение. В настоящее время поддерживается только два значения: `none` или `assignIfOpen` .|
|allowLateSubmissions|Логический| Определяет, могут ли учащиеся отправлять данные после даты окончания срока действия. Если это свойство не указано во время создания, по умолчанию задано значение true. |
|allowStudentsToAddResourcesToSubmission|Логический| Указывает, могут ли учащиеся добавлять собственные ресурсы в отправку или изменять только ресурсы, добавленные преподавателем. |
|assignDateTime|DateTimeOffset|Дата, когда назначение должно активться.  Если в будущем, задание не будет показано учащемуся до этой даты.  Тип **Timestamp** представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| Какие пользователи или весь класс должны получить объект отправки после публикации назначения. |
|assignedDateTime|DateTimeOffset|Момент публикации задания для учащихся и его показ на временной шкале учащихся.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|classId|String| Класс, которому принадлежит это назначение. |
|closeDateTime|DateTimeOffset| Дата закрытия назначения для отправки. Это необязательное поле, которое может иметь null, если назначение не разрешаетLateSubmissions или если closeDateTime является тем же, что и dueDateTime. Но если задан, то closeDateTime должен быть больше или равен dueDateTime. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|createdBy|[identitySet](identityset.md)| Кто создал назначение. |
|createdDateTime|DateTimeOffset|Момент создания назначения.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|displayName|String|Имя назначения.|
|dueDateTime|DateTimeOffset|Дата окончания задания для учащихся.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|grading|[educationAssignmentGradeType](educationassignmentgradetype.md)|Как будет оклассовка назначения. |
|инструкции|[itemBody](itembody.md)| Инструкции по назначению.  Это вместе с отображаемой именем сообщает учащемуся, что делать. |
|lastModifiedBy|[identitySet](identityset.md)| Кто последним изменил назначение. |
|lastModifiedDateTime|DateTimeOffset|Момент последнего изменения назначения.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|notificationChannelUrl|String|Необязательное поле для указания URL-адреса [канала для](channel.md) публикации уведомления о публикации назначения. Если значение не указано или значение null, по умолчанию для `General` канала. Это поле применяется только к назначениям, для которых **значение assignTo** — [educationAssignmentClassRecipient.](educationassignmentclassrecipient.md) Обновление **notificationChannelUrl** запрещено после публикации назначения.|
|status|string| Состояние **назначения.**  Это значение не может быть исправлено.  Возможные значения: `draft`, `scheduled`, `published`, `assigned`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resources|[Коллекция educationAssignmentResource](educationassignmentresource.md)| Учебные объекты, связанные с этим назначением.  Изменить этот список могут только преподаватели. Допускается значение null.|
|submissions|[коллекция educationSubmission](educationsubmission.md)| После публикации существует объект отправки для каждого учащегося, представляющего его работу и оценку.  Только для чтения. Допускается значение null.|
|categories|[коллекция educationCategory](educationcategory.md)| Если этот тип задан, пользователи могут легко находить назначения заданного типа.  Только для чтения. Допускается значение null.|
|rubric|[educationRubric](educationrubric.md)|При задании рубрика ограды, прикрепленная к этому назначению.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "addedStudentAction": "string",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "String (timestamp)",
  "classId": "String",
  "closeDateTime": "String (timestamp)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "dueDateTime": "String (timestamp)",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "instructions": {"@odata.type": "microsoft.graph.itemBody"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "notificationChannelUrl": "string",
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
  "suppressions": []
}
-->