---
title: Тип ресурса educationClass
description: Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и имеет один и тот же ИД.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d699e137ad2a80c5a53aa258f986aad968734269
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292911"
---
# <a name="educationclass-resource-type"></a>Тип ресурса educationClass

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет курс в учебном заведении. Ресурс **educationClass** в настоящее время соответствует группе Microsoft 365 [] и имеет один и тот же ИД.
Учащиеся являются обычными участниками класса, а преподаватели — владельцами и имеют соответствующие права.

> [!IMPORTANT]
> Чтобы опытом Microsoft 365 работал правильно, преподаватели должны быть членами коллекций преподавателей и участников.

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
| [Создание educationAssignment](../api/educationclass-post-assignments.md) | [educationAssignment]                          | Создание нового **educationAssignment путем** публикации в коллекции назначений.            |
| [Перечисление заданий](../api/educationclass-list-assignments.md)           | [коллекция educationAssignment]                | Получите **коллекцию объектов educationAssignment.**                                         |
| [Получение группы](../api/educationclass-get-group.md)                         | [group]                                        | Получите группу Microsoft  365, соответствующую этому **educationClass.**              |
| [Создание educationCategory](../api/educationclass-post-category.md)      | [educationCategory]                            | Создайте новую **educationCategory для** этого класса.                                        |
| [Перечисление категорий](../api/educationclass-list-categories.md)             | [коллекция educationCategory]                 | Получите список объектов **educationCategory,** принадлежащих этому классу.                      |
| [Обновление](../api/educationclass-update.md)                               | [educationClass]                               | Обновление объекта **educationClass**.                                                         |
| [удаление](../api/educationclass-delete.md);                               | Нет                                           | Удаление объекта **educationClass**.                                                         |
| [Delta](../api/educationclass-delta.md)                                 | Коллекция [educationClass](educationclass.md) | Получить добавонные изменения **для educationClasses**                                          |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                  | Описание                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                                | Уникальный идентификатор для курса.                                                                                                                                     |
| classCode            | String                                | Код курса, используемый учебным заведением для идентификации курса.                                                                                                                 |
| course               | [educationS](educationcourse.md) | Сведения о курсах для класса                                                                                                                                     |
| createdBy            | [identitySet]                         | Объект, который создал курс.                                                                                                                                         |
| description          | String                                | Описание курса.                                                                                                                                            |
| displayName          | String                                | Название курса.                                                                                                                                                   |
| externalId           | String                                | Идентификатор курса из системы синхронизации.                                                                                                                             |
| externalName         | String                                | Название курса в системе синхронизации.                                                                                                                             |
| externalSource       | String                                | Тип внешнего источника, из который был создан этот ресурс (автоматически определяется `externalSourceDetail` из). Возможные значения: `sis`, `lms` или `manual`. |
| externalSourceDetail | String                                | Имя внешнего источника, из которого были созданы эти ресурсы.                                                                                                   |
| оценка                | String                                | Уровень класса.                                                                                                                                            |
| mailNickname         | String                                | Почтовое имя для отправки почты всем участникам, если это возможно.                                                                                                      |
| term                 | [educationTerm]                       | Термин для класса.                                                                                                                                                  |

## <a name="relationships"></a>Связи

| Связь | Тип                             | Описание                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| assignments  | [коллекция educationAssignment] | Все назначения, связанные с этим классом. Допускается значение null.     |
| members      | Коллекция [educationUser]       | Все пользователи для этого курса. Допускается значение NULL.                         |
| schools      | Коллекция [educationSchool]     | Все учебные заведения, с которыми сопоставлен этот курс. Допускается значение NULL. |
| teachers     | Коллекция [educationUser]       | Все преподаватели для этого курса. Допускается значение null.                      |

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

[educationclass]: educationclass.md
[educationuser]: educationuser.md
[educationassignment]: educationassignment.md
[educationcourse]: educationcourse.md
[educationcategory]: educationcategory.md
[educationschool]: educationschool.md
[educationterm]: educationterm.md
[identityset]: identityset.md
[group]: group.md


