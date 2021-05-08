---
title: Создание educationSchool
description: Создание нового объекта educationSchool.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f9bf1499ef3c1d0106d9daac1bbda8f7ef25926d
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232250"
---
# <a name="create-educationschool"></a>Создание educationSchool

Пространство имен: microsoft.graph

Создание нового [объекта educationSchool.](../resources/educationschool.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается.                              |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | EduRoster.ReadWrite.All                     |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/schools
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [educationSchool.](../resources/educationschool.md)

В следующей таблице показаны свойства, необходимые при создании [educationSchool.](../resources/educationschool.md)

| Свойство             | Тип                                               | Описание                                                                                                                                                          |
| :------------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| displayName          | Строка                                             | Отображаемое имя учебного заведения. Унаследованный от [educationOrganization](../resources/educationorganization.md).                                                           |
| description          | Строка                                             | Описание учебного заведения. Унаследованный от [educationOrganization](../resources/educationorganization.md).                                                            |
| externalSource       | educationExternalSource                            | Источник, из которых была создана эта организация. Унаследованный от [educationOrganization](../resources/educationorganization.md). Возможные значения: `sis` " вручную. |
| externalSourceDetail | Строка                                             | Имя внешнего источника, из которого были созданы эти ресурсы.                                                                                                   |
| principalEmail       | String                                             | Адрес электронной почты директора.                                                                                                                                      |
| principalName        | String                                             | Имя директора.                                                                                                                                               |
| externalPrincipalId  | String                                             | Идентификатор директора в системе синхронизации.                                                                                                                                   |
| highestGrade         | String                                             | Самый старший класс.                                                                                                                                                |
| lowestGrade          | String                                             | Самый младший класс.                                                                                                                                                 |
| schoolNumber         | String                                             | Номер школы.                                                                                                                                                       |
| externalId           | String                                             | Идентификатор учебного заведения в системе синхронизации.                                                                                                                                      |
| phone                | String                                             | Номер телефона учебного заведения.                                                                                                                                              |
| fax                  | String                                             | Номер факса учебного заведения.                                                                                                                                                |
| createdBy            | [identitySet](../resources/identityset.md)         | Объект, который создал учебное заведение.                                                                                                                                       |
| address              | [physicalAddress](../resources/physicaladdress.md) | Адрес учебного заведения.                                                                                                                                               |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationSchool](../resources/educationschool.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/schools
Content-Type: application/json
Content-length: 583

{
  "@odata.type": "#microsoft.graph.educationSchool",
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
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```

### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
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
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```
