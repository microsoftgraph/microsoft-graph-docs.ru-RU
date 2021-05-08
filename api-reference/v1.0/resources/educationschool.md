---
title: Тип ресурса educationSchool
description: 'Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.  '
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b076b38e52bb8a7eb93a9eef35c866fc58e0e29a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231859"
---
# <a name="educationschool-resource-type"></a>Тип ресурса educationSchool

Пространство имен: microsoft.graph

Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.

Наследует от [educationOrganization](../resources/educationorganization.md).

## <a name="methods"></a>Методы

| Метод                                                     | Тип возвращаемых данных                                                   | Описание                                                                                            |
| :--------------------------------------------------------- | :------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------- |
| [Перечисление educationSchools](../api/educationschool-list.md)    | Коллекция [educationSchool](../resources/educationschool.md) | Получите список объектов [educationSchool](../resources/educationschool.md) и их свойств.     |
| [Создание educationSchool](../api/educationschool-post.md) | [educationSchool](../resources/educationschool.md)            | Создание нового [объекта educationSchool.](../resources/educationschool.md)                                |
| [Получение educationSchool](../api/educationschool-get.md)       | [educationSchool](../resources/educationschool.md)            | Ознакомьтесь с свойствами и отношениями объекта [educationSchool.](../resources/educationschool.md) |
| [Обновление educationSchool](../api/educationschool-update.md) | [educationSchool](../resources/educationschool.md)            | Обновление свойств объекта [educationSchool.](../resources/educationschool.md)                 |
| [Удаление educationSchool](../api/educationschool-delete.md) | None                                                          | Удаление объекта [educationSchool](../resources/educationschool.md).                                  |
| [delta](../api/educationschool-delta.md)                   | Коллекция [educationSchool](../resources/educationschool.md) | Получите дополнительные изменения в коллекции ресурсов.                                                    |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                               | Описание                                                                                                                                                          |
| :------------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| address              | [physicalAddress](../resources/physicaladdress.md) | Адрес учебного заведения.                                                                                                                                               |
| createdBy            | [identitySet](../resources/identityset.md)         | Объект, который создал учебное заведение.                                                                                                                                       |
| description          | Строка                                             | Описание учебного заведения. Унаследованный от [educationOrganization](../resources/educationorganization.md).                                                             |
| displayName          | Строка                                             | Отображаемое имя учебного заведения. Унаследованный от [educationOrganization](../resources/educationorganization.md).                                                            |
| externalId           | String                                             | Идентификатор учебного заведения в системе синхронизации.                                                                                                                                      |
| externalPrincipalId  | String                                             | Идентификатор директора в системе синхронизации.                                                                                                                                   |
| externalSource       | educationExternalSource                            | Источник, из которых была создана эта организация. Унаследованный от [educationOrganization](../resources/educationorganization.md). Возможные значения: `sis`, `manual`. |
| externalSourceDetail | Строка                                             | Имя внешнего источника, из которого были созданы эти ресурсы.                                                                                                   |
| highestGrade         | String                                             | Самый старший класс.                                                                                                                                                |
| id                   | Строка                                             | Идентификатор объекта. Наследуется от [сущности](../resources/entity.md).                                                                                                   |
| lowestGrade          | String                                             | Самый младший класс.                                                                                                                                                 |
| phone                | String                                             | Номер телефона учебного заведения.                                                                                                                                              |
| principalEmail       | String                                             | Адрес электронной почты директора.                                                                                                                                      |
| principalName        | String                                             | Имя директора.                                                                                                                                               |
| schoolNumber         | String                                             | Номер школы.                                                                                                                                                       |

## <a name="relationships"></a>Связи

| Связь       | Тип                                                        | Описание                                       |
| :----------------- | :---------------------------------------------------------- | :------------------------------------------------ |
| administrativeUnit | [administrativeUnit](../resources/administrativeunit.md)    | The underlying administrativeUnit for this school. |
| classes            | Коллекция [educationClass](../resources/educationclass.md) | Классы, которые обучаются в учебном заведении. Допускается значение null.           |
| users              | Коллекция [educationUser](../resources/educationuser.md)   | Пользователи в учебном заведении. Допускается значение null.                    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSchool",
  "baseType": "microsoft.graph.educationOrganization",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```
