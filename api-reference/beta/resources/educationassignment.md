---
title: Тип ресурса educationAssignment
description: Ресурс **educationAssignment** представляет задачу или единицу работы, назначенную студенту или участнику команды в классе в ходе их изучения. Только преподаватели и владельцы групп могут создавать назначения. Назначения содержат раздаточные материалы и задачи, с которыми обучающий хочет работать. Каждое назначение учащихся имеет связанную отправку, которая содержит все действия, которые попросят включить в свой преподаватель. Преподаватели могут добавлять оценки и отзывы о возможностях отправки, включенных студентом.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d7e614ac3f706886d893cc3f9cbb61d81d5db3cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502818"
---
# <a name="educationassignment-resource-type"></a>Тип ресурса educationAssignment

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **educationAssignment** представляет задачу или единицу работы, назначенную студенту или участнику команды в классе в ходе их изучения. Только преподаватели и владельцы групп могут создавать назначения. Назначения содержат раздаточные материалы и задачи, с которыми обучающий хочет работать. Каждое назначение учащихся имеет связанную [отправку](educationsubmissionresource.md) , которая содержит все действия, которые попросят включить в свой преподаватель. Преподаватели могут добавлять оценки и отзывы о возможностях отправки, включенных студентом.

При создании назначения он находится в состоянии черновика. Слушатели не будут создавать назначения и отправку. Вы можете изменить состояние назначения с помощью действия " [опубликовать](../api/educationassignment-publish.md) ". Вы не можете использовать запрос PATCH для изменения состояния назначения.

API назначения представлены в пространстве имен класса.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список ресурсов](../api/educationassignment-list-resources.md) |Коллекция [едукатионассигнментресаурце](educationassignmentresource.md)| Получение коллекции объектов **едукатионассигнментресаурце** .|
|[Отправка списка](../api/educationassignment-list-submissions.md) |Коллекция [educationSubmission](educationsubmission.md)| Получение коллекции объектов **educationSubmission** .|
|[Перечисление категорий](../api/educationassignment-list-categories.md) |Коллекция [едукатионкатегори](educationcategory.md)| Получение коллекции объектов **едукатионкатегори** .|
|[Создание ресурса задания](../api/educationassignment-post-resources.md) |[едукатионассигнментресаурце](educationassignmentresource.md)| Создание нового **едукатионассигнментресаурце** путем публикации в коллекции ресурсов.|
|[Получение задания](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Чтение свойств и связей объекта **educationAssignment** .|
|[обновление](../api/educationassignment-update.md). | [educationAssignment](educationassignment.md) |Обновление объекта **educationAssignment** . |
|[удаление](../api/educationassignment-delete.md); | Нет |Удаление объекта **educationAssignment** . |
|[Добавление категорий](../api/educationassignment-add-categories.md) |[едукатионкатегори](educationcategory.md) | Назначьте **едукатионкатегори** , принадлежащую классу, этому назначению.|
|[Удаление категории](../api/educationassignment-remove-category.md) |Нет| Удаление **едукатионкатегори** , относящегося к классу, из этого назначения.|
|[Присоединение Rubric](../api/educationassignment-put-rubric.md)|Нет|Присоединение существующего **едукатионрубрик** к этому назначению.|
|[Удаление Rubric](../api/educationassignment-delete-rubric.md)|Нет|Отсоедините **едукатионрубрик** от этого назначения.|
|[публикация](../api/educationassignment-publish.md);|[educationAssignment](educationassignment.md)|Изменение состояния объекта **educationAssignment** с черновика на "Опубликовано".|
|[Получение URL-адреса папки ресурсов](../api/educationassignment-getresourcesfolderurl.md)| строка| Папка OneDrive, в которую следует поместить файловые ресурсы, которые должны быть частью ресурса назначения. Файлы должны находиться в этой папке для добавления в качестве ресурса.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения.|
|алловлатесубмиссионс|Логический| Определяет, могут ли студенты быть отправлены после даты выполнения. Если во время создания это свойство не задано, по умолчанию используется значение true. |
|алловстудентстоаддресаурцестосубмиссион|Логический| Определяет, могут ли студенты добавлять собственные ресурсы в отправку или изменять только ресурсы, добавленные преподавателем. |
|ассигндатетиме|DateTimeOffset|Дата, когда назначение должно стать активным.  Если в будущем, назначение не отображается студенту до этой даты.  Тип **timestamp** представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|ассигнто|[едукатионассигнментреЦипиент](educationassignmentrecipient.md)| Какой пользователь или весь класс должен получать объект отправки после публикации назначения. |
|ассигнеддатетиме|DateTimeOffset|Время, когда назначение было опубликовано для учащихся, а Назначение отображается на временной шкале учащихся.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|classId|String| Класс, к которому относится данное назначение. |
|клоседатетиме|DateTimeOffset| Дата, когда назначение будет закрыто для отправки. Это необязательное поле, которое может иметь значение null, если назначение не Алловлатесубмиссионс или Клоседатетиме совпадает с Дуедатетиме. Но если этот параметр указан, то значение Клоседатетиме должно быть больше или равно значению Дуедатетиме. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|createdBy|[identitySet](identityset.md)| Кто создал назначение. |
|createdDateTime|DateTimeOffset|Время создания назначения.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|displayName|Строка|Имя назначения.|
|dueDateTime|DateTimeOffset|Дата, когда срок назначения студентов.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|снижения|[едукатионассигнментградетипе](educationassignmentgradetype.md)|Как будет выполняться оценка назначения. |
|выполнен|[itemBody](itembody.md)| Инструкции для назначения.  Вместе с отображаемым именем сообщите слушателю, что нужно сделать. |
|lastModifiedBy|[identitySet](identityset.md)| , Который последним изменил назначение. |
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения назначения.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|status|string| Состояние **назначения**.  Вы не можете исправить это значение.  Возможные значения: `draft`, `scheduled`, `published`, `assigned`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resources|Коллекция [едукатионассигнментресаурце](educationassignmentresource.md)| Обучающие объекты, связанные с этим назначением.  Только преподаватели могут изменять этот список. Допускается значение null.|
|отправок|Коллекция [educationSubmission](educationsubmission.md)| После публикации для каждого учащегося существует объект отправки, представляющий свою работу и оценку.  Только для чтения. Допускается значение null.|
|categories|Коллекция [едукатионкатегори](educationcategory.md)| Если задано, позволяет пользователям легко находить назначения определенного типа.  Только для чтения. Допускается значение null.|
|Rubric|[едукатионрубрик](educationrubric.md)|Если этот параметр установлен, Rubric подключается к этому назначению.|

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
