---
title: Тип ресурса educationClass
description: 'Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и использует тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  '
ms.localizationpriority: medium
author: mlafleur
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d9853bf9d82240801c9853b69a60b21ad8830709
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366235"
---
# <a name="educationclass-resource-type"></a>Тип ресурса educationClass

Пространство имен: microsoft.graph

Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и использует тот же идентификатор. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

| Метод                                                   | Тип возвращаемых данных                                                 | Описание                                                                                          |
| :------------------------------------------------------- | :---------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| [Перечисление educationClasses](../api/educationclass-list.md)   | Коллекция [educationClass](../resources/educationclass.md) | Получение списка объектов [educationClass](../resources/educationclass.md) и их свойств.     |
| [Создание educationClass](../api/educationclass-post.md) | [educationClass](../resources/educationclass.md)            | Создайте объект [educationClass](../resources/educationclass.md) .                                |
| [Получение educationClass](../api/educationclass-get.md)       | [educationClass](../resources/educationclass.md)            | Чтение свойств и связей объекта [educationClass](../resources/educationclass.md) . |
| [Обновление educationClass](../api/educationclass-update.md) | [educationClass](../resources/educationclass.md)            | Обновление свойств объекта [educationClass](../resources/educationclass.md) .                 |
| [Удаление educationClass](../api/educationclass-delete.md) | Нет                                                        | Удаление объекта [educationClass](../resources/educationclass.md) .                                  |
| [Получение дельты](../api/educationclass-delta.md)                  | Коллекция [educationClass](educationclass.md)              | Получение добавочных изменений для **educationClasses**.                                          |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                           | Описание                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| id                   | String                                         | Идентификатор объекта. Наследуется от [сущности](../resources/entity.md). |
| displayName          | String                                         | Название курса.                                                 |
| mailNickname         | String                                         | Почтовое имя для отправки почты всем участникам, если это возможно.    |
| description          | String                                         | Описание курса.                                          |
| createdBy            | [identitySet](../resources/identityset.md)     | Объект, который создал курс.                                       |
| classCode            | String                                         | Код курса, используемый учебным заведением для идентификации курса.               |
| externalName         | String                                         | Название курса в системе синхронизации.                           |
| externalId           | String                                         | Идентификатор курса из системы синхронизации.                           |
| externalSource       | educationExternalSource                        | Способ создания этого курса. Возможные значения: `sis`, `manual`.  |
| externalSourceDetail | String                                         | Имя внешнего источника, из которой были созданы эти ресурсы. |
| оценка                | String                                         | Уровень оценки класса.                                          |
| term                 | [educationTerm](../resources/educationterm.md) | Срок для этого курса.                                               |

## <a name="relationships"></a>Связи

| Связь | Тип                                                          | Описание                                               |
| :----------- | :------------------------------------------------------------ | :-------------------------------------------------------- |
| assignments  | [коллекция educationAssignment](educationAssignment.md) | Все назначения, связанные с этим классом. Допускается значение null.     |
| group        | [group](../resources/group.md)                                | Базовый объект Microsoft 365 группы.                |
| members      | Коллекция [educationUser](../resources/educationuser.md)     | Все пользователи для этого курса. Допускается значение NULL.                         |
| schools      | Коллекция [educationSchool](../resources/educationschool.md) | Все учебные заведения, с которыми сопоставлен этот курс. Допускается значение NULL. |
| teachers     | Коллекция [educationUser](../resources/educationuser.md)     | Все преподаватели для этого курса. Допускается значение NULL.                      |
|assignmentCategories| [Коллекция educationCategory](educationcategory.md) | Все категории, связанные с этим классом. Допускается значение null. |
|assignmentDefaults| [Коллекция educationAssignmentDefaults](educationassignmentdefaults.md) | Задает значения по умолчанию на уровне класса, которые учитываются новыми назначениями, созданными в классе. |
|assignmentSettings| [Коллекция educationAssignmentSettings](educationassignmentsettings.md) | Задает параметры назначений на уровне класса. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationClass",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "String (identifier)",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
