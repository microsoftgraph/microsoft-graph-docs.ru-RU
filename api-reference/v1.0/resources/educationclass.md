---
title: Тип ресурса educationClass
description: 'Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и использует тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 78280017d71fe0cbcaa84ec22905da6848f45f98
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897885"
---
# <a name="educationclass-resource-type"></a>Тип ресурса educationClass

Пространство имен: microsoft.graph

Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и использует тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  


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
|[Получение группы](../api/educationclass-get-group.md) |[group](group.md)| Получите **группу** Microsoft 365, соответствующую этой **educationClass**.|
|[Обновление](../api/educationclass-update.md) | [educationClass](educationclass.md)    |Обновление объекта **educationClass**. |
|[Delete](../api/educationclass-delete.md) | Нет |Удаление объекта **educationClass**. |

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
|externalSource|едукатионекстерналсаурце| Способ создания этого курса. Допустимые значения: `sis`, `manual`, `unknownFutureValue`.|
|term|[educationTerm](educationterm.md)|Срок для этого курса.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|members|Коллекция [educationUser](../resources/educationuser.md)| Все пользователи для этого курса. Допускается значение null.|
|schools|Коллекция [educationSchool](../resources/educationschool.md)| Все учебные заведения, с которыми сопоставлен этот курс. Допускается значение NULL.|
|teachers|Коллекция [educationUser](../resources/educationuser.md)|  Все преподаватели для этого курса. Допускается значение NULL.|
|group|[group](../resources/group.md)| Группа каталогов, соответствующая этому классу.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
