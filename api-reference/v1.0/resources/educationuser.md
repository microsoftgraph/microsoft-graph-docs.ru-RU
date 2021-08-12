---
title: Тип ресурса educationUser
description: Пользователь в системе. Используемый для сферы образования вариант указания пользователя с тем же параметром `id`, который Microsoft Graph возвратит из конечной точки `/users`, не ограниченной сферой образования.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 51693581e9af42aaae6c4e3f3961e0751818fa18522c53b7f4cef72afb4a14d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124495"
---
# <a name="educationuser-resource-type"></a>Тип ресурса educationUser

Пространство имен: microsoft.graph

Пользователь в системе. Используемый для сферы образования вариант указания пользователя с тем же параметром `id`, который Microsoft Graph возвратит из конечной точки `/users`, не ограниченной сферой образования. Этот объект предоставляет целевое подмножество свойств из основного объекта [user](../resources/user.md), а также добавляет ряд используемых для сферы образования свойств, таких как `primaryRole`, student и teacher.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы

| Метод                                                           | Тип возвращаемых данных                                                 | Описание                                                                                        |
| :--------------------------------------------------------------- | :---------------------------------------------------------- | :------------------------------------------------------------------------------------------------- |
| [Перечисление EducationUsers](../api/educationuser-list.md)              | Коллекция [educationUser](../resources/educationuser.md)   | Получите список объектов [educationUser](../resources/educationuser.md) и их свойств.     |
| [Создание educationUser](../api/educationuser-post.md)           | [educationUser](../resources/educationuser.md)              | Создание нового [объекта educationUser.](../resources/educationuser.md)                                |
| [Получение educationUser](../api/educationuser-get.md)                 | [educationUser](../resources/educationuser.md)              | Ознакомьтесь с свойствами и отношениями объекта [educationUser.](../resources/educationuser.md) |
| [Обновление educationUser](../api/educationuser-update.md)           | [educationUser](../resources/educationuser.md)              | Обновление свойств объекта [educationUser.](../resources/educationuser.md)                 |
| [Удаление educationUser](../api/educationuser-delete.md)           | Нет                                                        | Удаление объекта [educationUser](../resources/educationuser.md).                                  |
| [delta](../api/educationuser-delta.md)                           | Коллекция [educationUser](../resources/educationuser.md)   | Получите дополнительные изменения в коллекции ресурсов.                                                |
| [Список taughtClasses](../api/educationuser-list-taughtclasses.md) | Коллекция [educationClass](../resources/educationclass.md) | Получите ресурсы educationClass из свойства навигации taughtClasses.                       |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                                               | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| :------------------- | :----------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled       | Логический                                                            | Если учетная запись обеспечена — `True`, в противном случае — `false`. Это свойство обязательно указывать при создании пользователя. Поддерживает параметр $filter.                                                                                                                                                                                                                                                                                                                                                                                                    |
| assignedLicenses     | Коллекция [assignedLicense](../resources/assignedlicense.md)      | Лицензии, назначенные пользователю. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| assignedPlans        | Коллекция [assignedPlan](../resources/assignedplan.md)            | Планы, назначенные пользователю. Только для чтения. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| businessPhones       | Коллекция строк                                                  | Номера телефонов пользователя. **Примечание.** Несмотря на то что это коллекция строк, для этого свойства можно задать только один номер.                                                                                                                                                                                                                                                                                                                                                                                                |
| createdBy            | [identitySet](../resources/identityset.md)                         | Объект, который создал пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| department           | String                                                             | Название отдела, в котором работает пользователь. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| displayName          | String                                                             | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает `$filter` и `$orderby`.                                                                                                                                                                                                                                                           |
| externalSource       | educationExternalSource                                            | Источник для создания пользователя. Возможные значения: `sis`, `manual`.                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| externalSourceDetail | String                                                             | Имя внешнего источника, из которого были созданы эти ресурсы.                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| givenName            | String                                                             | Простое имя пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| id                   | String                                                             | Идентификатор объекта. Унаследованный от [сущности](../resources/entity.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| почта;                 | String                                                             | АДРЕС SMTP для пользователя; например, jeff@contoso.onmicrosoft.com. Только для чтения. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mailingAddress       | [physicalAddress](../resources/physicaladdress.md)                 | Почтовый адрес пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| mailNickname         | String                                                             | Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                           |
| middleName           | String                                                             | Отчество пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mobilePhone          | String                                                             | Основной сотовый телефон пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| onPremisesInfo       | [educationOnPremisesInfo](../resources/educationonpremisesinfo.md) | Дополнительные сведения, используемые для связи пользователя Azure AD с его коллегой Active Directory.                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| passwordPolicies     | String                                                             | Задает политики паролей для пользователя. Это свойство представляет собой перечисление с возможным значением `DisableStrongPassword`. Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение `DisablePasswordExpiration`. Эти два могут быть указаны вместе; например: `DisablePasswordExpiration, DisableStrongPassword` .                                                                                                                                                                      |
| passwordProfile      | [passwordProfile](../resources/passwordprofile.md)                 | Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.                                                                                                                                                                                                                             |
| preferredLanguage    | String                                                             | Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1. Пример: "ru-RU".                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| primaryRole          | educationUserRole                                                  | Роль по умолчанию для пользователя. Роль пользователя для отдельного курса может отличаться. Возможные значения: `student`, `teacher`, `none`, `unknownFutureValue`.                                                                                                                                                                                                                                                                                                                                                                     |
| provisionedPlans     | Коллекция [provisionedPlan](../resources/provisionedplan.md)      | Планы, подготовленные для пользователя. Только для чтения. Значение NULL не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| residenceAddress     | [physicalAddress](../resources/physicaladdress.md)                 | Адрес проживания пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| showInAddressList    | Логический                                                            | Значение true, если глобальный список адресов Outlook должен содержать этого пользователя. В противном случае используется значение false. Если не задано, будет считаться, что присвоено значение true. Для пользователей, приглашенных через диспетчер приглашений, этому свойству присваивается значение false.                                                                                                                                                                                                                                                                                                               |
| student              | [educationStudent](../resources/educationstudent.md)               | Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| surname              | String                                                             | Фамилия пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| teacher              | [educationTeacher](../resources/educationteacher.md)               | Если основной ролью является учитель, этот блок будет содержать определенные данные учителя.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| usageLocation        | String                                                             | Двухбуквенный код страны (по стандарту ISO 3166). Свойство необходимо указывать для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в странах или регионах. Примеры: "RU", "JP", "GB". Значение null не допускается. Поддерживает `$filter`.                                                                                                                                                                                                                                                                |
| userPrincipalName    | String                                                             | Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](organization.md). Поддерживает `$filter` и `$orderby`. |
| userType             | String                                                             | Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость". Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                        |

> [!IMPORTANT]
> При использовании областей делегирования разрешений Graph возвращает только ограниченный набор свойств: `id` `primaryRole` , , `accountEnabled` `displayName` `givenName` `surname` `userPrincipalName` `userType` `onPremisesInfo` `student/externalId` `teacher/externalId` . Если вашему приложению необходимы дополнительные свойства, необходимо использовать области разрешений приложения.

## <a name="relationships"></a>Связи

| Связь  | Тип                                                          | Описание                                    |
| :------------ | :------------------------------------------------------------ | :--------------------------------------------- |
| classes       | Коллекция [educationClass](../resources/educationclass.md)   | Курсы пользователя. Допускается значение NULL.   |
| schools       | Коллекция [educationSchool](../resources/educationschool.md) | Учебные заведения пользователя. Допускается значение NULL.   |
| taughtClasses | Коллекция [educationClass](../resources/educationclass.md)   | Классы, для которых пользователь является преподавателем.       |
| пользователь          | [user](../resources/user.md)                                  | Пользователь каталога, соответствующий этому пользователю. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "String (identifier)",
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
  "businessPhones": ["String"],
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
   ],
  "tocPath": ""
}-->

[educationuser]: educationuser.md
[educationclass]: educationclass.md
[educationschool]: educationschool.md
[educationassignment]: /graph/api/resources/educationassignment?view=graph-rest-beta
[educationteacher]: educationteacher.md
[educationstudent]: educationstudent.md
[relatedcontact]: relatedcontact.md
[physicaladdress]: physicaladdress.md
[provisionedplan]: provisionedplan.md
[passwordprofile]: passwordprofile.md
[identityset]: identityset.md
[assignedplan]: assignedplan.md
[assignedlicense]: assignedlicense.md
[user]: user.md
[directoryobject]: directoryobject.md

