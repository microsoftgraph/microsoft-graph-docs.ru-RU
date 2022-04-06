---
title: Тип ресурса educationUser
description: Представляет пользователя в системе. Это определенный для образования вариант пользователя с тем же ИД, который microsoft Graph возвращает из конечной точки /пользователей, не относя к образованию.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d1e7ffe90690b35b25537a9ca23d9b8f05d9817c
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588542"
---
# <a name="educationuser-resource-type"></a>Тип ресурса educationUser

Пространство имен: microsoft.graph

Пользователь в системе. Это определенный для образования вариант пользователя с тем же идом, который microsoft Graph `/users` вернется из конечной точки, не определенной для образования. Этот объект предоставляет целевой подмножество свойств из основного [](../resources/user.md) объекта пользователя и добавляет набор свойств, определенных для образования, таких как **primaryRole**, **student** и **teacher** data.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

| Метод                                                           | Тип возвращаемых данных                                                 | Описание                                                                                        |
| :--------------------------------------------------------------- | :---------------------------------------------------------- | :------------------------------------------------------------------------------------------------- |
| [Перечисление EducationUsers](../api/educationuser-list.md)              | Коллекция [educationUser](../resources/educationuser.md)   | Получите список объектов [educationUser](../resources/educationuser.md) и их свойств.     |
| [Создание educationUser](../api/educationuser-post.md)             | [educationUser](../resources/educationuser.md)              | Создание нового [объекта educationUser](../resources/educationuser.md) .                                |
| [Получение educationUser](../api/educationuser-get.md)                 | [educationUser](../resources/educationuser.md)              | Ознакомьтесь с свойствами и отношениями объекта [educationUser](../resources/educationuser.md) . |
| [Обновление educationUser](../api/educationuser-update.md)           | [educationUser](../resources/educationuser.md)              | Обновление свойств объекта [educationUser](../resources/educationuser.md) .                 |
| [Удаление educationUser](../api/educationuser-delete.md)           | Нет                                                        | Удаление объекта [educationUser](../resources/educationuser.md).                                   |
| [delta](../api/educationuser-delta.md)                           | Коллекция [educationUser](../resources/educationuser.md)   | Получите дополнительные изменения в коллекции ресурсов.                                                |
| [Список taughtClasses](../api/educationuser-list-taughtclasses.md) | Коллекция [educationClass](../resources/educationclass.md) | Получите ресурсы **educationClass** из свойства **навигации taughtClasses** .                       |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                                               | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| :------------------- | :----------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled       | Логический                                                            | Если учетная запись обеспечена — `True`, в противном случае — `false`. Это свойство обязательно указывать при создании пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                |
| assignedLicenses     | Коллекция [assignedLicense](../resources/assignedlicense.md)      | Лицензии, назначенные пользователю. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| assignedPlans        | Коллекция [assignedPlan](../resources/assignedplan.md)            | Планы, назначенные пользователю. Только для чтения. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| businessPhones       | Коллекция строк                                                  | Номера телефонов пользователя. **Примечание.** Несмотря на то что это коллекция строк, для этого свойства можно задать только один номер.                                                                                                                                                                                                                                                                                                                                                                                                        |
| createdBy            | [identitySet](../resources/identityset.md)                         | Объект, создавший пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| department           | String                                                             | Название отдела, в котором работает пользователь. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| displayName          | String                                                             | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает `$filter` и `$orderby`.                                                                                                                                                                                                                                                               |
| externalSource       | educationExternalSource                                            | Источник для создания пользователя. Возможные значения: `sis`, `manual`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| externalSourceDetail | Строка                                                             | Имя внешнего источника, из которого был создан этот ресурс.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| givenName            | String                                                             | Простое имя пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| id                   | String                                                             | Идентификатор объекта. Наследуется от [сущности](../resources/entity.md).                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| почта;                 | String                                                             | SMTP-адрес пользователя, например `jeff@contoso.onmicrosoft.com`. Только для чтения. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| mailingAddress       | [physicalAddress](../resources/physicaladdress.md)                 | Адрес электронной почты пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| mailNickname         | String                                                             | Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| middleName           | String                                                             | Среднее имя пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| mobilePhone          | String                                                             | Основной сотовый телефон пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| onPremisesInfo       | [educationOnPremisesInfo](../resources/educationonpremisesinfo.md) | Дополнительные сведения, используемые для связи Azure Active Directory пользователя с его коллегой Active Directory.                                                                                                                                                                                                                                                                                                                                                                                                                          |
| passwordPolicies     | String                                                             | Задает политики паролей для пользователя. Это свойство представляет собой перечисление с возможным значением `DisableStrongPassword`. Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение `DisablePasswordExpiration`. Эти два могут быть указаны вместе; например: `DisablePasswordExpiration, DisableStrongPassword`.                                                                                                                                                                              |
| passwordProfile      | [passwordProfile](../resources/passwordprofile.md)                 | Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.                                                                                                                                                                                                                                     |
| preferredLanguage    | String                                                             | Предпочтительный язык для пользователя, который должен следовать коду ISO 639-1, например. `en-US`                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| primaryRole          | educationUserRole                                                  | Роль по умолчанию для пользователя. Роль пользователя для отдельного курса может отличаться. Возможные значения: `student`, `teacher`, `none`, `unknownFutureValue`.                                                                                                                                                                                                                                                                                                                                                                             |
| provisionedPlans     | Коллекция [provisionedPlan](../resources/provisionedplan.md)      | Планы, подготовленные для пользователя. Только для чтения. Значение NULL не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| relatedContacts      | [коллекция relatedContact]                                        | Связанные записи, связанные с пользователем. Только для чтения.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| residenceAddress     | [physicalAddress](../resources/physicaladdress.md)                 | Адрес, где живет пользователь.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| showInAddressList    | Логический                                                            | `True`если глобальный список Outlook адресов должен содержать этого пользователя; в противном случае . `false` Если не задано, будет считаться, что присвоено значение `true`. Для пользователей, приглашенных через диспетчер приглашений, этому свойству присваивается значение `false`.                                                                                                                                                                                                                                                                                                               |
| student              | [educationStudent](../resources/educationstudent.md)               | Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| surname              | String                                                             | Фамилия пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| teacher              | [educationTeacher](../resources/educationteacher.md)               | Если основной ролью является учитель, этот блок будет содержать определенные данные учителя.                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| usageLocation        | String                                                             | Двухбуквенный код страны (по стандарту ISO 3166). Свойство необходимо указывать для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в странах или регионах. Примеры: `US`, `JP` и `GB`. Значение null не допускается. Поддерживает `$filter`.                                                                                                                                                                                                                                                                      |
| userPrincipalName    | String                                                             | Имя участника-пользователя. UpN — это имя входа в интернет-стиле для пользователя, основанное на стандарте RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат , `alias@domain`где домен должен присутствовать в коллекции проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Проверенные домены для клиента можно получить из свойства **verifiedDomains** [организации](organization.md). Поддерживает `$filter` и `$orderby`. |
| userType             | String                                                             | Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например `Member` и `Guest`. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                              |

> [!IMPORTANT]
> При использовании областей делегирования разрешений Microsoft Graph возвращает только ограниченный набор свойств: **id**, **primaryRole**, **accountEnabled**, **displayName**, **givenName**, **surname**, **userPrincipalName**, **userType**, **onPremisesInfo**, **student/externalId**, **teacher/externalId**. Если вашему приложению необходимы дополнительные свойства, необходимо использовать области разрешений приложения.

## <a name="relationships"></a>Связи

| Связь  | Тип                                                                  | Описание                                       |
| :------------ | :-------------------------------------------------------------------- | :------------------------------------------------ |
| assignments   | [коллекция educationAssignment](../resources/educationassignment.md) | Назначения, принадлежащие пользователю.             |
| classes       | Коллекция [educationClass](../resources/educationclass.md)           | Курсы пользователя. Допускается значение NULL.      |
| schools       | Коллекция [educationSchool](../resources/educationschool.md)         | Учебные заведения пользователя. Допускается значение NULL.      |
| taughtClasses | Коллекция [educationClass](../resources/educationclass.md)           | Классы, для которых пользователь является преподавателем.          |
| user          | [user](../resources/user.md)                                          | Пользователь каталога, соответствующий этому пользователю. |

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
