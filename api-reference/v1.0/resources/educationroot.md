---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: cb3f84c3417b2007485cabfa1a1078660f025f5e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840525"
---
# <a name="educationroot-resource-type"></a>Тип ресурса educationRoot

Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)). Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание educationClass](../api/educationroot-post-classes.md) |[educationClass](educationclass.md)| Создание объекта **educationClass** путем публикации в коллекции курсов.|
|[Перечисление курсов](../api/educationroot-list-classes.md) |Коллекция [educationClass](educationclass.md)| Получение коллекции объектов **educationClass**.|
|[Создание educationSchool](../api/educationroot-post-schools.md) |[educationSchool](educationschool.md)| Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.|
|[Перечисление учебных заведений](../api/educationroot-list-schools.md) |Коллекция [educationSchool](educationschool.md)| Получение коллекции объектов **educationSchool**.|
|[Создание educationUser](../api/educationroot-post-users.md) |[educationUser](educationuser.md)| Создание **educationUser** путем публикации в коллекции пользователей.|
|[Перечисление пользователей](../api/educationroot-list-users.md) |Коллекция [educationUser](educationuser.md)| Получение коллекции объектов **educationUser**.|

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|classes|Коллекция [educationClass](educationclass.md)| Только для чтения. Допускается значение NULL.|
|me|[educationUser](educationuser.md)| Только для чтения. Допускается значение NULL.|
|schools|Коллекция [educationSchool](educationschool.md)| Только для чтения. Допускается значение NULL.|
|users|Коллекция [educationUser](educationuser.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
