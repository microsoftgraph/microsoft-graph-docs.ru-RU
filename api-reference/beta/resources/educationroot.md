---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 91f0162402b8c87042fab622710d314f27d6f4e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523514"
---
# <a name="educationroot-resource-type"></a>Тип ресурса educationRoot

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|classes|Коллекция [educationClass](educationclass.md)| Только для чтения. Допускается значение null.|
|me|[educationUser](educationuser.md)| Только для чтения. Допускается значение null.|
|schools|Коллекция [educationSchool](educationschool.md)| Только для чтения. Допускается значение null.|
|users|Коллекция [educationUser](educationuser.md)| Только для чтения. Допускается значение NULL.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationroot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
