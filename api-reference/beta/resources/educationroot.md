---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8084b1aae61ffb9e9982fbf8b5f4b8e430a85da1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972567"
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

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
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
  "suppressions": []
}
-->
