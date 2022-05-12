---
title: Тип ресурса educationAssignment
description: Представляет задачу или единицу работы, назначенную учащемуся или участнику команды в классе в рамках его исследования.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 679b665ff5cac12904918b3293c88262db93a0c6
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2022
ms.locfileid: "65365997"
---
# <a name="educationassignment-resource-type"></a>Тип ресурса educationAssignment

Пространство имен: microsoft.graph

Представляет задачу или единицу работы, назначенную учащемуся или участнику команды в классе в рамках его исследования. 

Создавать задания могут только преподаватели **или владельцы команд**. **Задания содержат** раздатки и задачи, над которые преподаватель хочет работать. Каждое **задание учащегося** имеет [связанную отправку](educationsubmissionresource.md) , содержащую любые трудовую работу, которую преподаватель запросил для сдания. Преподаватель может добавлять оценки и отзывы **к отправке** , сданной учащемуся.

При создании **назначения** оно находится в состоянии черновика. Учащиеся не могут видеть **задание,** **и отправки** не будут созданы. Состояние назначения можно изменить **с** помощью действия [публикации](../api/educationassignment-publish.md) . Вы не можете использовать запрос PATCH для изменения **состояния назначения** .

API назначения предоставляются в пространстве имен класса.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание ресурса задания](../api/educationassignment-post-resource.md) |[educationAssignmentResource](educationassignmentresource.md)| Создайте **объект educationAssignmentResource** , выполнив публикацию в коллекции ресурсов.|
|[Получение задания](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Чтение свойств и связей объекта **educationAssignment** .|
|[Обновление](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |Обновление объекта **educationAssignment** . |
|[Удаление](../api/educationassignment-delete.md) | Нет |Удаление объекта **educationAssignment** . |
|[публикация](../api/educationassignment-publish.md);|[educationAssignment](educationassignment.md)|Измените состояние объекта **educationAssignment** с черновика на опубликованное.|
|[Настройка папки ресурсов назначения](../api/educationassignment-setupresourcesfolder.md)| строка| Создайте SharePoint папку (в предварительно определенном расположении) для отправки файлов в качестве ресурсов назначения.|
|[Перечисление ресурсов](../api/educationassignment-list-resources.md) |[Коллекция educationAssignmentResource](educationassignmentresource.md)| Получение коллекции **объектов educationAssignmentResource** .|
|[Перечисление отправок](../api/educationassignment-list-submissions.md) |[Коллекция educationSubmission](educationsubmission.md)| Получение коллекции **объектов educationSubmission** .|
|[Перечисление категорий](../api/educationassignment-list-categories.md) |[Коллекция educationCategory](educationcategory.md)| Получение коллекции **объектов educationCategory** .|
|[Добавление категорий](../api/educationassignment-post-categories.md) |[educationCategory](educationcategory.md) | **Назначьте этому заданию объект educationCategory**, принадлежащий классу.|
|[Удаление категории](../api/educationassignment-remove-category.md) |Нет| Удалите **из этого назначения объект educationCategory** , принадлежащий классу.|
|[Присоединить rubric](../api/educationassignment-put-rubric.md)|Нет|Присоедините **существующий educationRubric** к этому назначению.|
|[Удаление rubric](../api/educationassignment-delete-rubric.md)|Нет|**Отсоедините educationRubric** от этого назначения.|
|[Получение дельты](../api/educationassignment-delta.md)|[коллекция educationAssignment](../resources/educationassignment.md)|Получение списка вновь созданных или обновленных объектов **educationAssignment** без необходимости выполнять полное чтение коллекции.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения.|
|addedStudentAction|String|Необязательное поле для управления **поведением** задания для учащихся, добавленных **после публикации** задания. Если значение не указано, по умолчанию используется `none` значение. В настоящее время поддерживается только два значения: `none` или `assignIfOpen`.|
|addToCalendarAction| educationAddToCalendarOptions|Необязательное поле для управления **поведением** задания для  добавления заданий в календари учащихся и преподавателей **при публикации** задания. Возможные значения: , , , `studentsAndTeamOwners`, и . `unknownFutureValue``studentsOnly``studentsAndPublisher``none` Обратите внимание, что для `Prefer: include-unknown-enum-members` получения следующих значений в этом развиваемом перечислении необходимо использовать заголовок [запроса](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). `studentsOnly` Значение по умолчанию — `none`.|
|allowLateSubmissions|Логическое| Определяет, могут ли учащиеся отправлять сообщения после даты выполнения. Если это свойство не указано во время создания, по умолчанию используется значение true. |
|allowStudentsToAddResourcesToSubmission|Логическое| Определяет, могут ли учащиеся добавлять собственные ресурсы в отправку  или изменять только ресурсы, добавленные преподавателем. |
|assignDateTime|DateTimeOffset|Дата, когда **назначение должно** стать активным.  В будущем задание **не будет** показано учащемуся до этой даты.  Тип **метки времени** представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| Какие пользователи или весь класс должны получать объект **отправки** **после публикации** назначения. |
|assignedDateTime|DateTimeOffset|Момент публикации **задания** для учащихся и его **отображение** на временной шкале учащихся.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|classId|String| Класс, которому **принадлежит это** назначение. |
|closeDateTime|DateTimeOffset| Дата закрытия **назначения** для **отправки**. Это необязательное поле, которое может иметь значение NULL,  если назначение не разрешаетlateSubmissions или если значение closeDateTime совпадает с dueDateTime. Но если указано, то значение closeDateTime должно быть больше или равно dueDateTime. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|createdBy|[identitySet](identityset.md)| Кто создано **назначение**. |
|createdDateTime|DateTimeOffset|Момент создания **назначения** .  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|displayName|String|Имя **назначения.**|
|dueDateTime|DateTimeOffset|Дата **окончания задания** учащихся.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|Профилирования|[educationAssignmentGradeType](educationassignmentgradetype.md)|Способ **оценки** задания. |
|Инструкции|[itemBody](itembody.md)| Инструкции по назначению.  Это вместе с отображаемое имя сообщают учащемуся, что делать. |
|lastModifiedBy|[identitySet](identityset.md)| Кто последнее изменение **назначения**. |
|lastModifiedDateTime|DateTimeOffset|Момент **последнего** изменения назначения.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|notificationChannelUrl|String|Необязательное поле для указания URL-адреса канала [для](channel.md) публикации **уведомления о** публикации назначения. Если значение не указано или равно NULL, по умолчанию `General` используется канал. Это поле применяется только к **назначениям,** где **значение assignTo** равно [educationAssignmentClassRecipient](educationassignmentclassrecipient.md). Обновление **notificationChannelUrl** не допускается после публикации назначения.|
|status|string| Состояние **назначения.**  Вы не можете установить исправление для этого значения.  Возможные значения: `draft`, `scheduled`, `published`, `assigned`.|
|webUrl|string| URL-адрес глубокой ссылки для данного **назначения**.|
|resourcesFolderUrl|строка| URL-адрес папки, в которой хранятся все файловые **ресурсы для этого** назначения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resources|[Коллекция educationAssignmentResource](educationassignmentresource.md)| Обучение объекты, связанные с этим назначением.  Только преподаватели могут изменять этот список. Допускается значение null.|
|Представлений|[Коллекция educationSubmission](educationsubmission.md)| После публикации для каждого **учащегося** есть объект отправки, представляющий его работу и оценку.  Только для чтения. Допускается значение null.|
|categories|[Коллекция educationCategory](educationcategory.md)| Если этот параметр задан, пользователи могут легко находить **назначения заданного** типа.  Только для чтения. Допускается значение null.|
|Рубрика|[educationRubric](educationrubric.md)|Если этот параметр задан, к этому назначению прикреплена **категория.**|

## <a name="json-representation"></a>Представление в формате JSON

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
  "addToCalendarAction": "string",  
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
  "status": "string",
  "webUrl": "string",
  "resourcesFolderUrl": "string"
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
