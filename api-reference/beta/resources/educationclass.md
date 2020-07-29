---
title: Тип ресурса educationClass
description: Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и использует тот же идентификатор.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f4410518feca7c84e6093b9ff739feae99b631c5
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509590"
---
# <a name="educationclass-resource-type"></a>Тип ресурса educationClass

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет курс в учебном заведении. В настоящее время ресурс **educationClass** соответствует [группе] Microsoft 365 и использует тот же идентификатор.
Студенты являются обычными участниками класса, а преподаватели являются владельцами и имеют соответствующие права.

> [!IMPORTANT]
> Для правильной работы Microsoft 365 преподаватели должны быть членами обеих коллекций преподавателей и Members.

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
| [Создание educationAssignment](../api/educationclass-post-assignments.md) | [educationAssignment]                          | Создание нового **educationAssignment** путем публикации в коллекции назначений.            |
| [Перечисление заданий](../api/educationclass-list-assignments.md)           | Коллекция [educationAssignment]                | Получение коллекции объектов **educationAssignment** .                                         |
| [Получение группы](../api/educationclass-get-group.md)                         | [group]                                        | Получите **группу** Microsoft 365, соответствующую этой **educationClass**.              |
| [Создание Едукатионкатегори](../api/educationclass-post-category.md)      | [едукатионкатегори]                            | Создание нового **едукатионкатегори** для этого класса.                                        |
| [Перечисление категорий](../api/educationclass-list-categories.md)             | Коллекция [едукатионкатегори]                 | Получение списка объектов **едукатионкатегори** , принадлежащих этому классу.                      |
| [Обновление](../api/educationclass-update.md)                               | [educationClass]                               | Обновление объекта **educationClass**.                                                         |
| [удаление](../api/educationclass-delete.md);                               | Нет                                           | Удаление объекта **educationClass**.                                                         |
| [Delta](../api/educationclass-delta.md)                                 | Коллекция [educationClass](educationclass.md) | Получение добавочных изменений для **едукатионклассес**                                          |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                  | Описание                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | Строка                                | Уникальный идентификатор для курса.                                                                                                                                     |
| classCode            | Строка                                | Код курса, используемый учебным заведением для идентификации курса.                                                                                                                 |
| курсе               | [едукатионкаурсе](educationcourse.md) | Сведения о курсе для класса                                                                                                                                     |
| createdBy            | [identitySet]                         | Объект, который создал курс.                                                                                                                                         |
| description          | String                                | Описание курса.                                                                                                                                            |
| displayName          | Строка                                | Название курса.                                                                                                                                                   |
| externalId           | Строка                                | Идентификатор курса из системы синхронизации.                                                                                                                             |
| externalName         | String                                | Название курса в системе синхронизации.                                                                                                                             |
| externalSource       | Строка                                | Тип внешнего источника, из которого был создан ресурс (определяется автоматически `externalSourceDetail` ). Возможные значения: `sis` , `lms` , или `manual` . |
| екстерналсаурцедетаил | Строка                                | Имя внешнего источника, из которого были созданы ресурсы.                                                                                                   |
| оценка                | String                                | Уровень категории класса.                                                                                                                                            |
| mailNickname         | String                                | Почтовое имя для отправки почты всем участникам, если это возможно.                                                                                                      |
| term                 | [educationTerm]                       | Термин для класса.                                                                                                                                                  |

## <a name="relationships"></a>Связи

| Связь | Тип                             | Описание                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| assignments  | Коллекция [educationAssignment] | Все назначения, связанные с этим классом. Допускается значение null.     |
| members      | Коллекция [educationUser]       | Все пользователи для этого курса. Допускается значение null.                         |
| schools      | Коллекция [educationSchool]     | Все учебные заведения, с которыми сопоставлен этот курс. Допускается значение null. |
| teachers     | Коллекция [educationUser]       | Все преподаватели для этого курса. Допускается значение NULL.                      |

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
    "Error: Resource educationClass has documented navigation properties, but we thought it was a complex type!",
    "Resource educationClass has documented navigation properties, but we thought it was a complex type!"
  ]

}-->

[educationclass]: educationclass.md
[educationuser]: educationuser.md
[educationassignment]: educationassignment.md
[educationcourse]: educationcourse.md
[едукатионкатегори]: educationcategory.md
[educationschool]: educationschool.md
[едукатионтерм]: educationterm.md
[Identity]: identityset.md
[group]: group.md
