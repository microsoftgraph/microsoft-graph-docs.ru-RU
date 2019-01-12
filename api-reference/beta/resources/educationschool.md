---
title: Тип ресурса educationSchool
description: 'Учебное заведение. Ресурс **EducationSchool** в настоящее время соответствует ресурсу administrativeUnit, и у них общий идентификатор.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 17a5c3ad2f28e802bb6cad3a97d1cb723b3407d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918247"
---
# <a name="educationschool-resource-type"></a>Тип ресурса educationSchool

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Учебное заведение. Ресурс **EducationSchool** в настоящее время соответствует ресурсу [administrativeUnit](administrativeunit.md), и у них общий идентификатор.  

Этот ресурс — подтип [educationOrganization](educationorganization.md).




## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get](../api/educationschool-get.md) | [educationSchool](educationschool.md) |Считывание свойств и отношений объекта **educationSchool**.|
|[Добавление класса](../api/educationschool-post-classes.md) |[educationClass](educationclass.md)| Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.|
|[Перечисление классов](../api/educationschool-list-classes.md) |Коллекция [educationClass](educationclass.md)| Получение коллекции объектов **educationClass**.|
|[Удаление класса](../api/educationschool-delete-classes.md) |[educationClass](educationclass.md)| Удаление **educationClass** из учебного заведения через свойство навигации classes.|
|[Добавление пользователя](../api/educationschool-post-users.md) |[educationUser](educationuser.md)| Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.|
|[Перечисление пользователей](../api/educationschool-list-users.md) |Коллекция [educationUser](educationuser.md)| Получение коллекции объектов **educationUser**.|
|[Удаление пользователя](../api/educationschool-delete-users.md) |[educationUser](educationuser.md)| Удаление **educationUser** из учебного заведения через свойство навигации **users**.|
|[Получение administrativeUnit](../api/educationschool-get-administrativeunit.md) |[administrativeUnit](administrativeunit.md)| Получение элемента **administrativeUnit**, соответствующего учебному заведению **educationSchool**.|
|[Обновление](../api/educationschool-update.md) | [educationSchool](educationschool.md) |Обновление объекта **educationSchool**. |
|[Удаление](../api/educationschool-delete.md) | None |Удаление объекта **educationSchool**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String|GUID этого учебного заведения.|
|displayName| String| Отображаемое имя учебного заведения.| 
|описание| String | Описание учебного заведения.| 
|status| string| Только для чтения. Возможные значения: `inactive`, `active`, `expired`, `deleteable`.|
|externalSource| string| Только для чтения.  Возможные значения: `sis`, `manual`, `unknownFutureValue`.|
|principalEmail| String| Адрес электронной почты директора.|
|principalName| String | Имя директора.|
|externalPrincipalId| String | Идентификатор директора в системе синхронизации. |
|highestGrade|String| Самый старший класс. |
|lowestGrade|String| Самый младший класс. |
|schoolNumber|String| Номер школы.|
|externalId|String| Идентификатор учебного заведения в системе синхронизации. |
|phone|String| Номер телефона учебного заведения. |
|fax|String| Номер факса учебного заведения. |
|address|[physicalAddress](physicaladdress.md)| Адрес учебного заведения.|
|createdBy|[identitySet](identityset.md)|Объект, который создал учебное заведение.|


## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|classes|Коллекция [educationClass](educationclass.md)| Классы, которые обучаются в учебном заведении. Допускается значение null.|
|users|Коллекция [educationUser](educationuser.md)| Пользователи в учебном заведении. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "fax": "String",
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
