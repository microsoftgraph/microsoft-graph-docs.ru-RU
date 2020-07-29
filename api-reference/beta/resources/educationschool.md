---
title: Тип ресурса educationSchool
description: 'Учебное заведение. В настоящее время ресурс **educationSchool** соответствует ресурсу administrativeUnit и использует тот же идентификатор.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 32ed190f39d84e4c756d265527f4f0a8bcaf73f5
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509814"
---
# <a name="educationschool-resource-type"></a>Тип ресурса educationSchool

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Учебное заведение. В настоящее время ресурс **educationSchool** соответствует ресурсу [administrativeUnit](administrativeunit.md) и использует тот же идентификатор.

Этот ресурс является подтипом [educationOrganization](educationorganization.md).

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
| [Получение administrativeUnit](../api/educationschool-get-administrativeunit.md) | [administrativeUnit](administrativeunit.md)      | Получение **administrativeUnit** , соответствующего этому **educationSchool**.                |
| [Обновление](../api/educationschool-update.md)                                 | [educationSchool](educationschool.md)            | Обновление объекта **educationSchool**.                                                       |
| [удаление](../api/educationschool-delete.md);                                 | Нет                                             | Удаление объекта **educationSchool**.                                                       |
| [Delta](../api/educationschool-delta.md)                                   | Коллекция [educationSchool](educationschool.md) | Получение добавочных изменений для **едукатионсчулс**                                            |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                  | Описание                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | Строка                                | GUID этого учебного заведения.                                                                                                                                                 |
| address              | [physicalAddress](physicaladdress.md) | Адрес учебного заведения.                                                                                                                                               |
| createdBy            | [identitySet](identityset.md)         | Объект, который создал учебное заведение.                                                                                                                                       |
| description          | String                                | Описание учебного заведения.                                                                                                                                           |
| displayName          | Строка                                | Отображаемое имя учебного заведения.                                                                                                                                          |
| externalId           | String                                | Идентификатор учебного заведения в системе синхронизации.                                                                                                                                      |
| externalPrincipalId  | Строка                                | Идентификатор директора в системе синхронизации.                                                                                                                                   |
| externalSource       | Строка                                | Тип внешнего источника, из которого был создан ресурс (определяется автоматически `externalSourceDetail` ). Возможные значения: `sis` , `lms` , или `manual` . |
| екстерналсаурцедетаил | Строка                                | Имя внешнего источника, из которого были созданы ресурсы.                                                                                                   |
| highestGrade         | Строка                                | Самый старший класс.                                                                                                                                                |
| lowestGrade          | Строка                                | Самый младший класс.                                                                                                                                                 |
| phone                | String                                | Номер телефона учебного заведения.                                                                                                                                              |
| principalEmail       | Строка                                | Адрес электронной почты директора.                                                                                                                                      |
| principalName        | Строка                                | Имя директора.                                                                                                                                               |
| schoolNumber         | Строка                                | Номер школы.                                                                                                                                                       |

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
    "Error: Resource educationSchool has documented navigation properties, but we thought it was a complex type!"
  ]
}-->
