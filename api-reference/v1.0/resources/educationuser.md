---
title: Тип ресурса educationUser
description: Представляет пользователя в системе. Это вариант пользователя для образовательных учреждений с тем же идентификатором, который microsoft Graph будет возвращать из конечной точки /users, не относяской к образовательным службам.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dbd01d673242a7d12ca4b73e054feae13170c74c
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685231"
---
# <a name="educationuser-resource-type"></a>Тип ресурса educationUser

Пространство имен: microsoft.graph

Пользователь в системе. Это вариант пользователя для образовательных учреждений с тем же идентификатором, который microsoft Graph `/users` возвращает из конечной точки, отличной от образовательных учреждений. Этот объект предоставляет целевое подмножество свойств из основного [](../resources/user.md) пользовательского объекта и добавляет набор свойств для образовательных учреждений, таких как **primaryRole**, **учащийся** и **данные** преподавателя.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

| Метод                                                           | Тип возвращаемых данных                                                 | Описание                                                                                        |
| :--------------------------------------------------------------- | :---------------------------------------------------------- | :------------------------------------------------------------------------------------------------- |
| [Перечисление EducationUsers](../api/educationuser-list.md)              | Коллекция [educationUser](../resources/educationuser.md)   | Получение списка объектов [educationUser](../resources/educationuser.md) и их свойств.     |
| [Создание educationUser](../api/educationuser-post.md)             | [educationUser](../resources/educationuser.md)              | Создайте объект [educationUser](../resources/educationuser.md) .                                |
| [Получение educationUser](../api/educationuser-get.md)                 | [educationUser](../resources/educationuser.md)              | Чтение свойств и связей объекта [educationUser](../resources/educationuser.md) . |
| [Обновление educationUser](../api/educationuser-update.md)           | [educationUser](../resources/educationuser.md)              | Обновление свойств объекта [educationUser](../resources/educationuser.md) .                 |
| [Удаление educationUser](../api/educationuser-delete.md)           | Нет                                                        | Удаление объекта [educationUser](../resources/educationuser.md).                                   |
| [delta](../api/educationuser-delta.md)                           | Коллекция [educationUser](../resources/educationuser.md)   | Получение добавочных изменений в коллекции ресурсов.                                                |
| [Перечисление taughtClasses](../api/educationuser-list-taughtclasses.md) | Коллекция [educationClass](../resources/educationclass.md) | Получите ресурсы **educationClass** из свойства **навигации taughtClasses** .                       |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                                               | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| :------------------- | :----------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled       | Логический                                                            | Если учетная запись обеспечена — `True`, в противном случае — `false`. Это свойство обязательно указывать при создании пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                |
| assignedLicenses     | Коллекция [assignedLicense](../resources/assignedlicense.md)      | Лицензии, назначенные пользователю. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| assignedPlans        | Коллекция [assignedPlan](../resources/assignedplan.md)            | Планы, назначенные пользователю. Только для чтения. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| businessPhones       | Коллекция строк                                                  | Номера телефонов пользователя. **Примечание.** Несмотря на то что это коллекция строк, для этого свойства можно задать только один номер.                                                                                                                                                                                                                                                                                                                                                                                                        |
| createdBy            | [identitySet](../resources/identityset.md)                         | Сущность, создавшего пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| department           | String                                                             | Название отдела, в котором работает пользователь. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| displayName          | String                                                             | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает `$filter` и `$orderby`.                                                                                                                                                                                                                                                               |
| externalSource       | educationExternalSource                                            | Источник для создания пользователя. Возможные значения: `sis`, `manual`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| externalSourceDetail | String                                                             | Имя внешнего источника, из которой был создан этот ресурс.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| givenName;            | String                                                             | Простое имя пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| id                   | String                                                             | Идентификатор объекта. Наследуется от [сущности](../resources/entity.md).                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| почта;                 | String                                                             | SMTP-адрес пользователя, например `jeff@contoso.onmicrosoft.com`. Только для чтения. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| mailingAddress       | [physicalAddress](../resources/physicaladdress.md)                 | Адрес электронной почты пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| mailNickname         | String                                                             | Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| middleName           | String                                                             | Отчество пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| mobilePhone          | String                                                             | Основной сотовый телефон пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| onPremisesInfo       | [educationOnPremisesInfo](../resources/educationonpremisesinfo.md) | Дополнительные сведения, используемые для связывания Azure Active Directory с его аналогом Active Directory.                                                                                                                                                                                                                                                                                                                                                                                                                          |
| passwordPolicies     | String                                                             | Задает политики паролей для пользователя. Это свойство представляет собой перечисление с возможным значением `DisableStrongPassword`. Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение `DisablePasswordExpiration`. Эти два параметра можно указать вместе; например: `DisablePasswordExpiration, DisableStrongPassword`.                                                                                                                                                                              |
| passwordProfile      | [passwordProfile](../resources/passwordprofile.md)                 | Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.                                                                                                                                                                                                                                     |
| preferredLanguage    | String                                                             | Предпочтительный язык для пользователя, который должен следовать коду ISO 639-1, `en-US`например.                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| primaryRole          | educationUserRole                                                  | Роль по умолчанию для пользователя. Роль пользователя для отдельного курса может отличаться. Возможные значения: `student`, `teacher`, `none`, `unknownFutureValue`.                                                                                                                                                                                                                                                                                                                                                                             |
| provisionedPlans     | Коллекция [provisionedPlan](../resources/provisionedplan.md)      | Планы, подготовленные для пользователя. Только для чтения. Значение NULL не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| relatedContacts      | [Коллекция relatedContact]                                        | Связанные записи, связанные с пользователем. Только для чтения.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| residenceAddress     | [physicalAddress](../resources/physicaladdress.md)                 | Адрес, где находится пользователь.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| showInAddressList    | Логический                                                            | `True`Значение , если Outlook глобальный список адресов должен содержать этого пользователя; в противном случае . `false` Если не задано, будет считаться, что присвоено значение `true`. Для пользователей, приглашенных через диспетчер приглашений, этому свойству присваивается значение `false`.                                                                                                                                                                                                                                                                                                               |
| student              | [educationStudent](../resources/educationstudent.md)               | Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| surname              | String                                                             | Фамилия пользователя. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| teacher              | [educationTeacher](../resources/educationteacher.md)               | Если основной ролью является преподаватель, этот блок будет содержать конкретные данные преподавателя.                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| usageLocation        | String                                                             | Двухбуквенный код страны (по стандарту ISO 3166). Свойство необходимо указывать для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в странах или регионах. Примеры: `US`, `JP` и `GB`. Значение null не допускается. Поддерживает `$filter`.                                                                                                                                                                                                                                                                      |
| userPrincipalName    | String                                                             | Имя участника-пользователя. Имя участника-пользователя — это имя входа в Интернет для пользователя, основанное на стандарте RFC 822 в Интернете. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат : домен `alias@domain`должен присутствовать в коллекции проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить из свойства **verifiedDomains** [организации](organization.md). Поддерживает `$filter` и `$orderby`. |
| userType             | String                                                             | Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например `Member` и `Guest`. Поддерживает `$filter`.                                                                                                                                                                                                                                                                                                                                                                                                              |

> [!IMPORTANT]
> При использовании областей делегированных разрешений Microsoft Graph возвращает только ограниченный набор свойств: **id**, **primaryRole**, **accountEnabled**, **displayName**, **givenName**, **surname**, **userPrincipalName**, **userType**, **onPremisesInfo**, **student/externalId**, **teacher/externalId**. Если приложению требуются дополнительные свойства, необходимо использовать области разрешений приложения.

## <a name="relationships"></a>Связи


| Связь  | Тип                                                          | Описание                                    |
| :------------ | :------------------------------------------------------------ | :--------------------------------------------- |
| assignments   | [коллекция educationAssignment](../resources/educationassignment.md)   | Назначения, принадлежащие пользователю.   |
| classes       | Коллекция [educationClass](../resources/educationclass.md)   | Курсы пользователя. Допускается значение NULL.   |
| schools       | Коллекция [educationSchool](../resources/educationschool.md) | Учебные заведения пользователя. Допускается значение NULL.   |
| taughtClasses | Коллекция [educationClass](../resources/educationclass.md)   | Классы, для которых пользователь является преподавателем.       |
| user          | [user](../resources/user.md)                                  | Пользователь каталога, соответствующий этому пользователю. |
|Рубрики|[Коллекция educationRubric](educationrubric.md)|Если этот параметр задан, к назначению прикреплена категория оценки.|


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
