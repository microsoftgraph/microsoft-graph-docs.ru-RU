---
title: Тип ресурса educationClass
description: 'Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и имеет один и тот же ID. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.  '
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3d1d6eb24e9d9b21ed8e828488ae306ec5c4bae549e51ecf0e69d63c5319e3a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160060"
---
# <a name="educationclass-resource-type"></a>Тип ресурса educationClass

Пространство имен: microsoft.graph

Представляет курс в учебном заведении. Ресурс **educationClass** соответствует группе Microsoft 365 и имеет один и тот же ID. Учащиеся — постоянные участники курса, а преподаватели являются владельцами и обладают соответствующими правами. Чтобы решения для Office работали правильно, преподаватели должны быть включены как в коллекцию teachers, так и в коллекцию members.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы

| Метод                                                   | Тип возвращаемых данных                                                 | Описание                                                                                          |
| :------------------------------------------------------- | :---------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| [Перечисление educationClasses](../api/educationclass-list.md)   | Коллекция [educationClass](../resources/educationclass.md) | Получите список объектов [educationClass](../resources/educationclass.md) и их свойств.     |
| [Создание educationClass](../api/educationclass-post.md) | [educationClass](../resources/educationclass.md)            | Создание нового [объекта educationClass.](../resources/educationclass.md)                                |
| [Получение educationClass](../api/educationclass-get.md)       | [educationClass](../resources/educationclass.md)            | Ознакомьтесь с свойствами и отношениями объекта [educationClass.](../resources/educationclass.md) |
| [Update educationClass](../api/educationclass-update.md) | [educationClass](../resources/educationclass.md)            | Обновление свойств объекта [educationClass.](../resources/educationclass.md)                 |
| [Удаление educationClass](../api/educationclass-delete.md) | Нет                                                        | Удаление [объекта educationClass.](../resources/educationclass.md)                                  |
| [delta](../api/educationclass-delta.md)                  | Коллекция [educationClass](../resources/educationclass.md) | Получите дополнительные изменения в коллекции ресурсов.                                                  |

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
| externalSourceDetail | String                                         | Имя внешнего источника, из которого были созданы эти ресурсы. |
| оценка                | String                                         | Уровень класса.                                          |
| term                 | [educationTerm](../resources/educationterm.md) | Срок для этого курса.                                               |

## <a name="relationships"></a>Связи

| Связь | Тип                                                          | Описание                                               |
| :----------- | :------------------------------------------------------------ | :-------------------------------------------------------- |
| group        | [group](../resources/group.md)                                | Объект Microsoft 365 группы.                |
| members      | Коллекция [educationUser](../resources/educationuser.md)     | Все пользователи для этого курса. Допускается значение NULL.                         |
| schools      | Коллекция [educationSchool](../resources/educationschool.md) | Все учебные заведения, с которыми сопоставлен этот курс. Допускается значение NULL. |
| teachers     | Коллекция [educationUser](../resources/educationuser.md)     | Все преподаватели для этого курса. Допускается значение null.                      |

## <a name="json-representation"></a>Представление JSON

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
