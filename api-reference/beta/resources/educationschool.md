---
title: Тип ресурса educationSchool
description: 'Учебное заведение. В настоящее время ресурс **educationSchool** соответствует ресурсу administrativeUnit и использует тот же идентификатор.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 893f01fffcc606c85cec30789ec94dd658b2a4b2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334200"
---
# <a name="educationschool-resource-type"></a>Тип ресурса educationSchool

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Учебное заведение. В настоящее время ресурс **educationSchool** соответствует ресурсу [administrativeUnit](administrativeunit.md) и использует тот же идентификатор.  

Этот ресурс является подтипом [educationOrganization](educationorganization.md).




## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение](../api/educationschool-get.md) | [educationSchool](educationschool.md) |Считывание свойств и отношений объекта **educationSchool**.|
|[Добавление класса](../api/educationschool-post-classes.md) |[educationClass](educationclass.md)| Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.|
|[Перечисление классов](../api/educationschool-list-classes.md) |Коллекция [educationClass](educationclass.md)| Получение коллекции объектов **educationClass**.|
|[Удаление класса](../api/educationschool-delete-classes.md) |[educationClass](educationclass.md)| Удаление **educationClass** из учебного заведения через свойство навигации classes.|
|[Добавление пользователя](../api/educationschool-post-users.md) |[educationUser](educationuser.md)| Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.|
|[Перечисление пользователей](../api/educationschool-list-users.md) |Коллекция [educationUser](educationuser.md)| Получение коллекции объектов **educationUser**.|
|[Удаление пользователя](../api/educationschool-delete-users.md) |[educationUser](educationuser.md)| Удаление **educationUser** из учебного заведения через свойство навигации **users**.|
|[Получение administrativeUnit](../api/educationschool-get-administrativeunit.md) |[administrativeUnit](administrativeunit.md)| Получение **administrativeUnit** , соответствующего этому **educationSchool**.|
|[Обновление](../api/educationschool-update.md) | [educationSchool](educationschool.md) |Обновление объекта **educationSchool**. |
|[Delete](../api/educationschool-delete.md) | Нет |Удаление объекта **educationSchool**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка|GUID этого учебного заведения.|
|displayName| String| Отображаемое имя учебного заведения.| 
|description| Строка | Описание учебного заведения.| 
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


## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|classes|Коллекция [educationClass](educationclass.md)| Классы, которые обучаются в учебном заведении. Допускается значение null.|
|users|Коллекция [educationUser](educationuser.md)| Пользователи в учебном заведении. Допускается значение null.|

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
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
