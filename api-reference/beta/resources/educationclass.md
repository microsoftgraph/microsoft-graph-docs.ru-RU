---
title: Тип ресурса educationClass
description: Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и использует тот же идентификатор.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 50302c03f9ccd1bd1b1ea38717be539a0731941b
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685097"
---
# <a name="educationclass-resource-type"></a>Тип ресурса educationClass

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет курс в учебном заведении. Ресурс **educationClass** в настоящее время соответствует Microsoft 365 [и] использует тот же идентификатор.
Учащиеся являются обычными участниками класса, а преподаватели являются владельцами и имеют соответствующие права.

> [!IMPORTANT]
> Чтобы Microsoft 365 работать правильно, преподаватели должны быть членами коллекций преподавателей и участников.

## <a name="methods"></a>Методы

| Метод                                                                  | Возвращаемый тип                                    | Описание                                                                               |
| :---------------------------------------------------------------------- | :--------------------------------------------- | :---------------------------------------------------------------------------------------- |
| [Получение educationClass](../api/educationclass-get.md)                      | [educationClass]                               | Считывание свойств и связей объекта **educationClass**.                        |
| [Добавление участника](../api/educationclass-post-members.md)                     | [educationUser]                                | Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации members.  |
| [Перечисление участников](../api/educationclass-list-members.md)                   | Коллекция [educationUser]                     | Получение коллекции объектов **educationUser**.                                               |
| [Удаление учащегося](../api/educationclass-delete-members.md)               | [educationUser]                                | Удаление **educationUser** для курса с использованием свойства навигации members.       |
| [Перечисление учебных заведений](../api/educationclass-list-schools.md)                   | Коллекция [educationSchool]                   | Получение коллекции объектов **educationSchool**.                                             |
| [Добавление преподавателя](../api/educationclass-post-teachers.md)                   | [educationUser]                                | Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации teachers. |
| [Перечисление преподавателей](../api/educationclass-list-teachers.md)                 | Коллекция [educationUser]                     | Получение списка преподавателей для курса.                                                     |
| [Удаление преподавателя](../api/educationclass-delete-teachers.md)              | [educationUser]                                | Удаление **educationUser** для курса с использованием свойства навигации teachers.      |
| [Создание educationAssignment](../api/educationclass-post-assignments.md) | [educationAssignment]                          | Создайте объект **educationAssignment** , выполнив публикацию в коллекции заданий.            |
| [Перечисление заданий](../api/educationclass-list-assignments.md)           | [educationAssignmentcollection]                | Получение коллекции **объектов educationAssignment** .                                         |
| [Получение группы](../api/educationclass-get-group.md)                         | [group]                                        | Получение группы Microsoft 365 **,** соответствующей этому **классу educationClass**.              |
| [Создание educationCategory](../api/educationclass-post-category.md)      | [educationCategory]                            | Создайте для **этого класса новую educationCategory** .                                        |
| [Перечисление категорий](../api/educationclass-list-categories.md)             | [Коллекция educationCategory]                 | Получение списка объектов **educationCategory** , принадлежащих этому классу.                      |
| [Обновление](../api/educationclass-update.md)                               | [educationClass]                               | Обновление объекта **educationClass**.                                                         |
| [Delete](../api/educationclass-delete.md)                               | Нет                                           | Удаление объекта **educationClass**.                                                         |
| [Получение дельты](../api/educationclass-delta.md)                                 | Коллекция [educationClass](educationclass.md) | Получение добавочных изменений для **educationClasses**.                                          |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                  | Описание                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                                | Уникальный идентификатор для курса.                                                                                                                                     |
| classCode            | String                                | Код курса, используемый учебным заведением для идентификации курса.                                                                                                                 |
| Курс               | [educationCourse](educationcourse.md) | Сведения о курсе для класса.                                                                                                                                     |
| createdBy            | [identitySet]                         | Сущность, создавшего класс.                                                                                                                                         |
| description          | String                                | Описание курса.                                                                                                                                            |
| displayName          | String                                | Название курса.                                                                                                                                                   |
| externalId           | String                                | Идентификатор курса из системы синхронизации.                                                                                                                             |
| externalName         | String                                | Название курса в системе синхронизации.                                                                                                                             |
| externalSource       | String                                | Тип внешнего источника, из которой был создан этот ресурс (автоматически определяется из `externalSourceDetail`). Возможные значения: `sis`, `lms` или `manual`. |
| externalSourceDetail | String                                | Имя внешнего источника, из которой были созданы эти ресурсы.                                                                                                   |
| оценка                | String                                | Уровень оценки класса.                                                                                                                                            |
| mailNickname         | String                                | Почтовое имя для отправки почты всем участникам, если это возможно.                                                                                                      |
| term                 | [educationTerm]                       | Термин для класса.                                                                                                                                                  |

## <a name="relationships"></a>Связи

| Связь | Тип                             | Описание                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| assignments  | [коллекция educationAssignment] | Все назначения, связанные с этим классом. Допускается значение null.     |
| members      | Коллекция [educationUser]       | Все пользователи для этого курса. Допускается значение NULL.                         |
| schools      | Коллекция [educationSchool]     | Все учебные заведения, с которыми сопоставлен этот курс. Допускается значение NULL. |
| teachers     | Коллекция [educationUser]       | Все преподаватели для этого курса. Допускается значение NULL.                      |
|assignmentCategories| [Коллекция educationCategory](educationcategory.md) | Все категории, связанные с этим классом. Допускается значение null. |
|assignmentDefaults| [Коллекция educationAssignmentDefaults](educationassignmentdefaults.md) | Задает значения по умолчанию на уровне класса, которые учитываются новыми назначениями, созданными в классе. |
|assignmentSettings| [Коллекция educationAssignmentSettings](educationassignmentsettings.md) | Задает параметры назначений на уровне класса. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "classCode": "String",
  "course": { "@odata.type": "microsoft.graph.educationCourse" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "grade": "string",
  "id": "String (identifier)",
  "mailNickname": "String",
  "term": { "@odata.type": "microsoft.graph.educationTerm" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.educationClass",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]

}-->

[класс education]: educationclass.md
[educationuser]: educationuser.md
[educationassignment]: educationassignment.md
[educationcourse]: educationcourse.md
[educationcategory]: educationcategory.md
[educationschool]: educationschool.md
[educationterm]: educationterm.md
[набор удостоверений]: identityset.md
[group]: group.md


