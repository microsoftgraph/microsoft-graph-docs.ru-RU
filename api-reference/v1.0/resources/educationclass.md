---
title: Тип ресурса educationClass
description: 'Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и использует тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 57e3204e15755e9ec7ce0150f46c6f0409ca3120
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032693"
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
|[удаление](../api/educationclass-delete.md); | Нет |Удаление объекта **educationClass**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id| String| Уникальный идентификатор для курса.|
|description|String| Описание курса.|
|displayName|String| Название курса.|
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
|members|Коллекция [educationUser](../resources/educationuser.md)| Все пользователи для этого курса. Допускается значение NULL.|
|schools|Коллекция [educationSchool](../resources/educationschool.md)| Все учебные заведения, с которыми сопоставлен этот курс. Допускается значение NULL.|
|teachers|Коллекция [educationUser](../resources/educationuser.md)|  Все преподаватели для этого курса. Допускается значение NULL.|
|group|[group](../resources/group.md)| Группа каталогов, соответствующая этому классу.|

## <a name="json-representation"></a>Представление JSON

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

