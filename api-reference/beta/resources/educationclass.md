---
title: Тип ресурса educationClass
description: Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Office 365, для него используется тот же идентификатор.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0bc9fa375e3f22087fbf268933370d8a6222654e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006369"
---
# <a name="educationclass-resource-type"></a>Тип ресурса educationClass

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Office 365, для него используется тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Для правильной работы Office 365 преподаватели должны быть членами обеих коллекций преподавателей и Members.

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
| [Получение группы](../api/educationclass-get-group.md)                         | [group]                                        | Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.                 |
| [Создание Едукатионкатегори](../api/educationclass-post-category.md)      | [Едукатионкатегори]                            | Создание нового **едукатионкатегори** для этого класса.                                        |
| [Перечисление категорий](../api/educationclass-list-categories.md)             | Коллекция [едукатионкатегори]                 | Получение списка объектов **едукатионкатегори** , принадлежащих этому классу.                      |
| [Обновление](../api/educationclass-update.md)                               | [educationClass]                               | Обновление объекта **educationClass**.                                                         |
| [Удаление](../api/educationclass-delete.md)                               | Нет                                           | Удаление объекта **educationClass**.                                                         |
| [Delta](../api/educationclass-delta.md)                                 | Коллекция [educationClass](educationclass.md) | Получение добавочных изменений для **едукатионклассес**                                          |

## <a name="properties"></a>Свойства

| Свойство       | Тип                                  | Описание                                                                             |
| :------------- | :------------------------------------ | :-------------------------------------------------------------------------------------- |
| id             | Строка                                | Уникальный идентификатор для курса.                                                        |
| classCode      | String                                | Код курса, используемый учебным заведением для идентификации курса.                                    |
| курсе         | [Едукатионкаурсе](educationcourse.md) | Сведения о курсе для класса                                                        |
| createdBy      | [identitySet]                         | Объект, который создал курс.                                                            |
| description    | String                                | Описание курса.                                                               |
| displayName    | Строка                                | Название курса.                                                                      |
| externalId     | String                                | Идентификатор курса из системы синхронизации.                                                |
| externalName   | String                                | Название курса в системе синхронизации.                                                |
| externalSource | string                                | Способ создания этого курса. Возможные значения: `sis`, `manual`, `unknownFutureValue`. |
| mailNickname   | String                                | Почтовое имя для отправки почты всем участникам, если это возможно.                         |
| term           | [educationTerm]                       | Термин для класса.                                                                     |

## <a name="relationships"></a>Отношения

| Отношение | Тип                             | Описание                                               |
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
