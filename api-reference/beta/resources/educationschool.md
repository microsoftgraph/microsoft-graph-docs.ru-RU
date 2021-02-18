---
title: Тип ресурса educationSchool
description: 'Учебное заведения. Ресурс **educationSchool** в настоящее время соответствует ресурсу administrativeUnit и имеет один и тот же ИД.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f8481ad876cd5c4c9a2f1bc8ca67297c647475ba
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292639"
---
# <a name="educationschool-resource-type"></a>Тип ресурса educationSchool

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Учебное заведения. Ресурс **educationSchool** в настоящее время соответствует [ресурсу administrativeUnit](administrativeunit.md) и имеет один и тот же ИД.

Этот ресурс является подтипом [educationOrganization.](educationorganization.md)

## <a name="methods"></a>Методы

| Метод                                                                     | Возвращаемый тип                                      | Описание                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [получение](../api/educationschool-get.md);                                       | [educationSchool](educationschool.md)            | Считывание свойств и отношений объекта **educationSchool**.                         |
| [Добавление класса](../api/educationschool-post-classes.md)                        | [educationClass](educationclass.md)              | Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.  |
| [Перечисление классов](../api/educationschool-list-classes.md)                     | Коллекция [educationClass](educationclass.md)   | Получение коллекции объектов **educationClass**.                                               |
| [Удаление класса](../api/educationschool-delete-classes.md)                   | [educationClass](educationclass.md)              | Удаление **educationClass** из учебного заведения через свойство навигации classes.       |
| [Добавление пользователя](../api/educationschool-post-users.md)                           | [educationUser](educationuser.md)                | Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**. |
| [Перечисление пользователей](../api/educationschool-list-users.md)                         | Коллекция [educationUser](educationuser.md)     | Получение коллекции объектов **educationUser**.                                                |
| [Удаление пользователя](../api/educationschool-delete-users.md)                      | [educationUser](educationuser.md)                | Удаление **educationUser** из учебного заведения через свойство навигации **users**.      |
| [Get administrativeUnit](../api/educationschool-get-administrativeunit.md) | [administrativeUnit](administrativeunit.md)      | Получите **administrativeUnit,** соответствующий этому **educationSchool.**                |
| [Обновление](../api/educationschool-update.md)                                 | [educationSchool](educationschool.md)            | Обновление объекта **educationSchool**.                                                       |
| [удаление](../api/educationschool-delete.md);                                 | Нет                                             | Удаление объекта **educationSchool**.                                                       |
| [Delta](../api/educationschool-delta.md)                                   | Коллекция [educationSchool](educationschool.md) | Получить добавонные изменения для **educationSchools**                                            |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                  | Описание                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                                | GUID этого учебного заведения.                                                                                                                                                 |
| address              | [physicalAddress](physicaladdress.md) | Адрес учебного заведения.                                                                                                                                               |
| createdBy            | [identitySet](identityset.md)         | Объект, который создал учебное заведение.                                                                                                                                       |
| description          | String                                | Описание учебного заведения.                                                                                                                                           |
| displayName          | String                                | Отображаемое имя учебного заведения.                                                                                                                                          |
| externalId           | String                                | Идентификатор учебного заведения в системе синхронизации.                                                                                                                                      |
| externalPrincipalId  | String                                | Идентификатор директора в системе синхронизации.                                                                                                                                   |
| externalSource       | String                                | Тип внешнего источника, из который был создан этот ресурс (автоматически определяется `externalSourceDetail` из). Возможные значения: `sis`, `lms` или `manual`. |
| externalSourceDetail | String                                | Имя внешнего источника, из которого были созданы эти ресурсы.                                                                                                   |
| highestGrade         | String                                | Самый старший класс.                                                                                                                                                |
| lowestGrade          | String                                | Самый младший класс.                                                                                                                                                 |
| phone                | String                                | Номер телефона учебного заведения.                                                                                                                                              |
| principalEmail       | String                                | Адрес электронной почты директора.                                                                                                                                      |
| principalName        | String                                | Имя директора.                                                                                                                                               |
| schoolNumber         | String                                | Номер школы.                                                                                                                                                       |

## <a name="relationships"></a>Связи

| Связь | Тип                                           | Описание                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| classes      | Коллекция [educationClass](educationclass.md) | Классы, которые обучаются в учебном заведении. Допускается значение null. |
| users        | Коллекция [educationUser](educationuser.md)   | Пользователи в учебном заведении. Допускается значение null.          |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
"blockType": "resource",
"keyProperty": "id",
"optionalProperties": [

],
"@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "address": { "@odata.type": "microsoft.graph.physicalAddress" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalPrincipalId": "String",
  "externalSource": "string",
  "highestGrade": "String",
  "id": "String (identifier)",
  "lowestGrade": "String",
  "phone": "String",
  "principalEmail": "String",
  "principalName": "String",
  "schoolNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


