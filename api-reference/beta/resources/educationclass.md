---
title: Тип ресурса educationClass
description: 'Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Office 365, для него используется тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: dfce83c99ec886a01c2c52c3bae58c91b12fa0b0
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536172"
---
# <a name="educationclass-resource-type"></a>Тип ресурса educationClass

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Office 365, для него используется тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение educationClass](../api/educationclass-get.md) | [educationClass](educationclass.md) |Считывание свойств и связей объекта **educationClass**.|
|[Добавление участника](../api/educationclass-post-members.md) |[educationUser](educationuser.md)| Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации members.|
|[Перечисление участников](../api/educationclass-list-members.md) |Коллекция [educationUser](educationuser.md)| Получение коллекции объектов **educationUser**.|
|[Удаление учащегося](../api/educationclass-delete-members.md) |[educationUser](educationuser.md)| Удаление **educationUser** для курса с использованием свойства навигации members.|
|[Перечисление учебных заведений](../api/educationclass-list-schools.md) |Коллекция [educationSchool](educationschool.md)| Получение коллекции объектов **educationSchool**.|
|[Добавление преподавателя](../api/educationclass-post-teachers.md) |[educationUser](educationuser.md)| Добавление нового объекта **educationUser** для курса путем публикации в свойстве навигации teachers.|
|[Перечисление преподавателей](../api/educationclass-list-teachers.md) |Коллекция [educationUser](educationuser.md)| Получение списка преподавателей для курса.|
|[Удаление преподавателя](../api/educationclass-delete-teachers.md) |[educationUser](educationuser.md)| Удаление **educationUser** для курса с использованием свойства навигации teachers.|
|[Создание educationAssignment](../api/educationclass-post-assignments.md) |[educationAssignment](../resources/educationassignment.md)| Создание нового **educationAssignment** путем публикации в коллекции назначений.|
|[Перечисление заданий](../api/educationclass-list-assignments.md) |Коллекция [educationAssignment](../resources/educationassignment.md)| Получение коллекции объектов **educationAssignment** .|
|[Получение группы](../api/educationclass-get-group.md) |[group](group.md)| Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.|
|[Создание Едукатионкатегори](../api/educationclass-post-category.md) | [Едукатионкатегори](educationcategory.md) | Создание нового **едукатионкатегори** для этого класса.|
|[Перечисление категорий](../api/educationclass-list-categories.md) | Коллекция [едукатионкатегори](educationcategory.md) | Получение списка объектов **едукатионкатегори** , принадлежащих этому классу.|
|[Обновление](../api/educationclass-update.md) | [educationClass](educationclass.md)    |Обновление объекта **educationClass**. |
|[Удаление](../api/educationclass-delete.md) | Нет |Удаление объекта **educationClass**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id| Строка| Уникальный идентификатор для курса.|
|description|String| Описание курса.|
|displayName|Строка| Название курса.|
|mailNickname|String| Почтовое имя для отправки почты всем участникам, если это возможно. |
|createdBy|[identitySet](identityset.md)| Объект, который создал курс. |
|classCode|String| Код курса, используемый учебным заведением для идентификации курса.|
|externalId|String| Идентификатор курса из системы синхронизации. |
|externalName|String|Название курса в системе синхронизации.|
|externalSource|string| Способ создания этого курса. Возможные значения: `sis`, `manual`, `unknownFutureValue`.|
|term|[educationTerm](educationterm.md)|Срок для этого курса.|


## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|members|Коллекция [educationUser](../resources/educationuser.md)| Все пользователи для этого курса. Допускается значение null.|
|schools|Коллекция [educationSchool](../resources/educationschool.md)| Все учебные заведения, с которыми сопоставлен этот курс. Допускается значение null.|
|teachers|Коллекция [educationUser](../resources/educationuser.md)|  Все преподаватели для этого курса. Допускается значение NULL.|
|assignments|Коллекция [educationAssignment](../resources/educationassignment.md)| Все назначения, связанные с этим классом. Допускается значение null.|
|categories|Коллекция [едукатионкатегори](../resources/educationassignment.md)| Все категории, связанные с этим классом. Допускается значение null.|

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
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
