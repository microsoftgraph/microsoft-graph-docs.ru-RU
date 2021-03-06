---
title: тип ресурса educationAssignment
description: Ресурс **educationAssignment** представляет задачу или единицу работы, назначенную учащемуся или члену группы в классе в рамках их обучения. Только преподаватели или владельцы команд могут создавать назначения. Задания содержат раздатки и задачи, над которые учитель хочет работать. Каждое назначение студента имеет связанное представление, содержаще любую работу, которую его учитель попросил включить. Преподаватель может добавить оценки и отзывы к отправке, включаемой студентом.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6cbeb1ac7f7462716afbe9b2e7f98cece48a479b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722463"
---
# <a name="educationassignment-resource-type"></a>тип ресурса educationAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **educationAssignment** представляет задачу или единицу работы, назначенную учащемуся или члену группы в классе в рамках их обучения. Только преподаватели или владельцы команд могут создавать назначения. Задания содержат раздатки и задачи, над которые учитель хочет работать. Каждое назначение студента имеет связанное [представление,](educationsubmissionresource.md) содержаще любую работу, которую его учитель попросил включить. Преподаватель может добавить оценки и отзывы к отправке, включаемой студентом.

Когда создается назначение, оно находится в состоянии Draft. Учащиеся не могут видеть назначения и отправки не будут созданы. Можно изменить состояние назначения с помощью действия [публикации.](../api/educationassignment-publish.md) Вы не можете использовать запрос PATCH для изменения состояния назначения.

API назначения выставляются в пространстве имен класса.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список ресурсов](../api/educationassignment-list-resources.md) |[коллекция educationAssignmentResource](educationassignmentresource.md)| Получите **коллекцию объектов educationAssignmentResource.**|
|[Отправки списков](../api/educationassignment-list-submissions.md) |[коллекция educationSubmission](educationsubmission.md)| Получите **коллекцию объектов educationSubmission.**|
|[Перечисление категорий](../api/educationassignment-list-categories.md) |[коллекция educationCategory](educationcategory.md)| Получите **коллекцию объектов educationCategory.**|
|[Создание ресурса задания](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| Создайте **новое образованиеAssignmentResource,** разместив в коллекции ресурсов.|
|[Получение задания](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Чтение свойств и связей объекта **educationAssignment.**|
|[Обновление](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |Обновление **объекта educationAssignment.** |
|[Удаление](../api/educationassignment-delete.md) | Нет |Удаление **объекта educationAssignment.** |
|[Добавление категорий](../api/educationassignment-add-categories.md) |[educationCategory](educationcategory.md) | **Назначьте этому назначению** учебноекатегорию, принадлежащее классу.|
|[Удаление категории](../api/educationassignment-remove-category.md) |Нет| Удалите из этого назначения учебноекатегорию, принадлежащее классу. |
|[Прикрепить рубрику](../api/educationassignment-put-rubric.md)|Нет|Прикрепить **существующее educationRubric к** этому назначению.|
|[Удаление рубрики](../api/educationassignment-delete-rubric.md)|Нет|**Отсоединить educationRubric** от этого назначения.|
|[публикация](../api/educationassignment-publish.md);|[educationAssignment](educationassignment.md)|Изменение состояния объекта **educationAssignment** с черновика на опубликованный.|
|[Получение URL-адреса папки ресурсов](../api/educationassignment-getresourcesfolderurl.md)| Строка| Папка OneDrive, в которую следует поместить ресурсы на основе файлов, чтобы быть частью ресурса назначения. Файлы должны быть размещены в этой папке, чтобы добавить их в качестве ресурса.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения.|
|addedStudentAction|String|Необязательное поле для управления поведением назначения для студентов, добавленных после публикации назначения. Если не указано, значение по `none` умолчанию. В настоящее время поддерживает только два значения: `none` или `assignIfOpen` .|
|allowLateSubmissions|Boolean| Определяет, могут ли студенты отправлять их после даты. Если это свойство не указано во время создания, оно по умолчанию указывает значение true. |
|allowStudentsToAddResourcesToSubmission|Boolean| Определяет, могут ли учащиеся добавлять собственные ресурсы в отправку или изменять только ресурсы, добавленные преподавателем. |
|assignDateTime|DateTimeOffset|Дата, когда назначение должно стать активным.  Если в будущем назначение не отображается учащемуся до этой даты.  Тип **Timestamp** представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| Какие пользователи или весь класс должны получать объект отправки после публикации назначения. |
|assignedDateTime|DateTimeOffset|Момент публикации задания для учащихся и его назначение указывается на временной шкале учащихся.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|classId|String| Класс, которому принадлежит это назначение. |
|closeDateTime|DateTimeOffset| Дата закрытия назначения для отправки. Это необязательное поле, которое может быть недействительным, если назначение не позволяет использоватьLateSubmissions или когда closeDateTime является таким же, как dueDateTime. Но если указано, то closeDateTime должен быть больше или равен dueDateTime. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|createdBy|[identitySet](identityset.md)| Кто создал назначение. |
|createdDateTime|DateTimeOffset|Момент создания назначения.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|displayName|String|Имя назначения.|
|dueDateTime|DateTimeOffset|Дата назначения учащихся.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|классификация|[educationAssignmentGradeType](educationassignmentgradetype.md)|Оценка назначения. |
|инструкции|[itemBody](itembody.md)| Инструкции по назначению.  Это вместе с именем отображения сообщает студенту, что делать. |
|lastModifiedBy|[identitySet](identityset.md)| Кто в последний раз изменил назначение. |
|lastModifiedDateTime|DateTimeOffset|Момент, когда назначение было изменено в последний раз.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|notificationChannelUrl|String|Необязательное поле для указания URL-адреса [канала для](channel.md) публикации уведомления о публикации назначения. Если не указано или не указано значение null, по умолчанию передается `General` каналу. Это поле применяется только к назначениям, где **значение assignTo** — [educationAssignmentClassRecipient](educationassignmentclassrecipient.md). Обновление **уведомленияChannelUrl** не допускается после публикации назначения.|
|status|string| Состояние **назначения**.  Это значение не может быть исправлено.  Возможные значения: `draft`, `scheduled`, `published`, `assigned`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resources|[коллекция educationAssignmentResource](educationassignmentresource.md)| Изучение объектов, связанных с этим назначением.  Изменить этот список могут только преподаватели. Допускается значение null.|
|отправки|[коллекция educationSubmission](educationsubmission.md)| После публикации для каждого учащегося будет размещен объект отправки, представляющий его работу и оценку.  Только для чтения. Допускается значение null.|
|categories|[коллекция educationCategory](educationcategory.md)| При наборе позволяет пользователям легко находить назначения того или иного типа.  Только для чтения. Допускается значение null.|
|рубрики|[educationRubric](educationrubric.md)|При наборе к этому назначению прилагается рубрика классификации.|

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
  "addedStudentAction": "none",
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
  "notificationChannelUrl": null,
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