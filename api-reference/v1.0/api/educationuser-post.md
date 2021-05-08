---
title: Создание educationUser
description: Создание нового объекта educationUser.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b26e0530fd4beea6d2f604fa46f891e154fefa61
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232286"
---
# <a name="create-educationuser"></a>Создание educationUser

Пространство имен: microsoft.graph

Создание нового [объекта educationUser.](../resources/educationuser.md)

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
POST /education/users
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [educationUser.](../resources/educationuser.md)

В следующей таблице показаны свойства, необходимые при создании [educationUser.](../resources/educationuser.md)

| Свойство             | Тип                                                               | Описание                                                                                                                                                                                                                                                                                                                                                 |
| :------------------- | :----------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled       | Логический                                                            | Если учетная запись обеспечена — значение **true**, в противном случае — **false**. Это свойство обязательно указывать при создании пользователя. Поддерживает параметр $filter.                                                                                                                                                                                                                               |
| assignedLicenses     | Коллекция [assignedLicense](../resources/assignedlicense.md)      | Лицензии, назначенные пользователю. Значение null не допускается.                                                                                                                                                                                                                                                                                                   |
| assignedPlans        | Коллекция [assignedPlan](../resources/assignedplan.md)            | Планы, назначенные пользователю. Только для чтения. Значение null не допускается.                                                                                                                                                                                                                                                                                           |
| businessPhones       | Коллекция строк                                                  | Номера телефонов пользователя. **Примечание.** Несмотря на то что это коллекция строк, для этого свойства можно задать только один номер.                                                                                                                                                                                                                           |
| createdBy            | [identitySet](../resources/identityset.md)                         | Объект, который создал пользователя.                                                                                                                                                                                                                                                                                                                                |
| department           | String                                                             | Название отдела, в котором работает пользователь. Поддерживает параметр $filter.                                                                                                                                                                                                                                                                                      |
| displayName          | String                                                             | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.                                                                                      |
| externalSource       | educationExternalSource                                            | Источник для создания пользователя. Возможные значения: `sis`, `manual`.                                                                                                                                                                                                                                                                                     |
| externalSourceDetail | Строка                                                             | Имя внешнего источника, из которого были созданы эти ресурсы.                                                                                                                                                                                                                                                                                          |
| givenName            | String                                                             | Простое имя пользователя. Поддерживает параметр $filter.                                                                                                                                                                                                                                                                                                  |
| mail                 | String                                                             | SMTP-адрес пользователя, например "victor@contoso.onmicrosoft.com". Только для чтения. Поддерживает параметр $filter.                                                                                                                                                                                                                                                    |
| mailingAddress       | [physicalAddress](../resources/physicaladdress.md)                 | Почтовый адрес пользователя.                                                                                                                                                                                                                                                                                                                                       |
| mailNickname         | String                                                             | Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает параметр $filter.                                                                                                                                                                                                                                                      |
| middleName           | String                                                             | Отчество пользователя.                                                                                                                                                                                                                                                                                                                                    |
| mobilePhone          | String                                                             | Основной сотовый телефон пользователя.                                                                                                                                                                                                                                                                                                         |
| onPremisesInfo       | [educationOnPremisesInfo](../resources/educationonpremisesinfo.md) | Дополнительные сведения, используемые для связи пользователя AAD с его аналогом Active Directory.                                                                                                                                                                                                                                                               |
| passwordPolicies     | String                                                             | Задает политики паролей для пользователя. Это свойство представляет собой перечисление с возможным значением DisableStrongPassword. Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение DisablePasswordExpiration. Два значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword". |
| passwordProfile      | [passwordProfile](../resources/passwordprofile.md)                 | Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.                                                        |
| preferredLanguage    | String                                                             | Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1. Пример: "ru-RU".                                                                                                                                                                                                                                                                    |
| primaryRole          | educationUserRole                                                  | Роль по умолчанию для пользователя. Роль пользователя для отдельного курса может отличаться. Возможные значения: `student`, `teacher`, `none`.                                                                                                                                                                                                                      |
| provisionedPlans     | Коллекция [provisionedPlan](../resources/provisionedplan.md)      | Планы, подготовленные для пользователя. Только для чтения. Значение NULL не допускается.                                                                                                                                                                                                                                                                                       |
| residenceAddress     | [physicalAddress](../resources/physicaladdress.md)                 | Адрес проживания пользователя.                                                                                                                                                                                                                                                                                                                                   |
| student              | [educationStudent](../resources/educationstudent.md)               | Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.                                                                                                                                                                                                                                                                              |
| surname              | String                                                             | Фамилия пользователя. Поддерживает параметр $filter.                                                                                                                                                                                                                                                                                            |
| teacher              | [educationTeacher](../resources/educationteacher.md)               | Если основной ролью является учитель, этот блок будет содержать определенные данные учителя.                                                                                                                                                                                                                                                                              |
| usageLocation        | String                                                             | Двухбуквенный код страны (по стандарту ISO 3166). Свойство необходимо указывать для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в странах или регионах. Примеры: "RU", "JP", "GB". Значение null не допускается. Поддерживает параметр $filter.                                                                                           |
| userPrincipalName    | String                                                             | Имя участника-пользователя.                                                                                                                                                                                                                                                                                                                  |
| userType             | String                                                             | Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость". Поддерживает параметр $filter.                                                                                                                                                                                                                                   |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationUser](../resources/educationuser.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/users
Content-Type: application/json
Content-length: 1585

{
  "@odata.type": "#microsoft.graph.educationUser",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
}
```

### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "90eedea1-dea1-90ee-a1de-ee90a1deee90",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
}
```
