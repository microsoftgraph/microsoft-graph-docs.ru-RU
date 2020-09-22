---
title: Тип ресурса educationSchool
description: 'Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2ed10fd9be0a49fbf25acac635cf29b1759c31eb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032658"
---
# <a name="educationschool-resource-type"></a>Тип ресурса educationSchool

Пространство имен: microsoft.graph

Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.  

## <a name="methods"></a>Методы

| Метод                                                   | Возвращаемый тип                                    | Описание                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [получение](../api/educationschool-get.md);                     | [educationSchool](educationschool.md)          | Считывание свойств и отношений объекта **educationSchool**.                         |
| [Добавление класса](../api/educationschool-post-classes.md)      | [educationClass](educationclass.md)            | Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.  |
| [Перечисление классов](../api/educationschool-list-classes.md)   | Коллекция [educationClass](educationclass.md) | Получение коллекции объектов **educationClass**.                                               |
| [Удаление класса](../api/educationschool-delete-classes.md) | [educationClass](educationclass.md)            | Удаление **educationClass** из учебного заведения через свойство навигации classes.       |
| [Добавление пользователя](../api/educationschool-post-users.md)         | [educationUser](educationuser.md)              | Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**. |
| [Перечисление пользователей](../api/educationschool-list-users.md)       | Коллекция [educationUser](educationuser.md)   | Получение коллекции объектов **educationUser**.                                                |
| [Удаление пользователя](../api/educationschool-delete-users.md)    | [educationUser](educationuser.md)              | Удаление **educationUser** из учебного заведения через свойство навигации **users**.      |
| [Обновление](../api/educationschool-update.md)               | [educationSchool](educationschool.md)          | Обновление объекта **educationSchool**.                                                       |
| [удаление](../api/educationschool-delete.md);               | Нет                                           | Удаление объекта **educationSchool**.                                                       |

## <a name="properties"></a>Свойства

| Свойство            | Тип                                  | Описание                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| id                  | String                                | GUID этого учебного заведения.                                                               |
| displayName         | String                                | Отображаемое имя учебного заведения.                                                        |
| description         | String                                | Описание учебного заведения.                                                         |
| status              | string                                | Только для чтения. Допустимые значения: `inactive`, `active`, `expired`, `deleteable`. |
| externalSource      | едукатионекстерналсаурце               | Только для чтения.  Допустимые значения: `sis`, `manual`, `unknownFutureValue`.        |
| principalEmail      | String                                | Адрес электронной почты директора.                                                    |
| principalName       | String                                | Имя директора.                                                             |
| externalPrincipalId | String                                | Идентификатор директора в системе синхронизации.                                                 |
| highestGrade        | String                                | Самый старший класс.                                                              |
| lowestGrade         | String                                | Самый младший класс.                                                               |
| schoolNumber        | String                                | Номер школы.                                                                     |
| externalId          | String                                | Идентификатор учебного заведения в системе синхронизации.                                                    |
| phone               | String                                | Номер телефона учебного заведения.                                                            |
| address             | [physicalAddress](physicaladdress.md) | Адрес учебного заведения.                                                             |
| createdBy           | [identitySet](identityset.md)         | Объект, который создал учебное заведение.                                                     |

## <a name="relationships"></a>Связи

| Связь | Тип                                           | Описание                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| classes      | Коллекция [educationClass](educationclass.md) | Классы, которые обучаются в учебном заведении. Допускается значение null. |
| users        | Коллекция [educationUser](educationuser.md)   | Пользователи в учебном заведении. Допускается значение null.          |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

