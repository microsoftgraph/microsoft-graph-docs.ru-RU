---
title: Тип ресурса educationUser
description: Пользователь в системе. Используемый для сферы образования вариант указания пользователя с тем же параметром `id`, который Microsoft Graph возвратит из конечной точки `/users`, не ограниченной сферой образования.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: aecf1b83c6f8c59c65c6b696aaea4b89352b91cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972340"
---
# <a name="educationuser-resource-type"></a>Тип ресурса educationUser

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Пользователь в системе. Используемый для сферы образования вариант указания пользователя с тем же параметром `id`, который Microsoft Graph возвратит из конечной точки `/users`, не ограниченной сферой образования.
Этот объект предоставляет целевое подмножество свойств из основного объекта [user], а также добавляет ряд используемых для сферы образования свойств, таких как `primaryRole`, student и teacher.

## <a name="methods"></a>Методы

| Метод                                               | Возвращаемый тип                                  | Описание                                                                   |
| :--------------------------------------------------- | :------------------------------------------- | :---------------------------------------------------------------------------- |
| [Получение educationUser](../api/educationuser-get.md)     | [educationUser]                              | Считывание свойств и связей объекта **educationUser**.             |
| [Перечисление курсов](../api/educationuser-list-classes.md) | Коллекция [educationClass]                  | Получение коллекции объектов **educationClass**, для которых пользователь является участником.    |
| [Перечисление учебных заведений](../api/educationuser-list-schools.md) | Коллекция [educationSchool]                 | Получение коллекции объектов **educationSchool**, для которых пользователь является участником. |
| [Получение пользователя](../api/educationuser-get-user.md)         | [user]                                       | Получение простого каталога **user**, который соответствует этому объекту **educationUser**. |
| [Обновление](../api/educationuser-update.md)             | [educationUser]                              | Обновление объекта **educationUser**.                                           |
| [Удаление](../api/educationuser-delete.md)             | Нет                                         | Удаление объекта **educationUser**.                                           |
| [Delta](../api/educationuser-delta.md)               | Коллекция [educationUser](educationuser.md) | Получение добавочных изменений для **едукатионусерс**.                               |

## <a name="properties"></a>Свойства

| Свойство          | Тип                                                  | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| :---------------- | :---------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                | String                                                | Уникальный идентификатор пользователя. Наследуется от [directoryObject]. Ключ. Значение null не допускается. Только для чтения.                                                                                                                                                                                                                                                                                                                                                                                                                              |
| accountEnabled    | Boolean                                               | Если учетная запись обеспечена — значение **true**, в противном случае — **false**. Это свойство обязательно указывать при создании пользователя. Поддерживает \$фильтр.                                                                                                                                                                                                                                                                                                                                                                                                   |
| assignedLicenses  | Коллекция [assignedLicense]                          | Лицензии, назначенные пользователю. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| assignedPlans     | Коллекция [assignedPlan]                             | Планы, назначенные пользователю. Только для чтения. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| businessPhones    | Коллекция строк                                     | Номера телефонов пользователя. **Примечание.** Несмотря на то что это коллекция строк, для этого свойства можно задать только один номер.                                                                                                                                                                                                                                                                                                                                                                                                |
| createdBy         | [identitySet]                                         | Объект, который создал пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| department        | String                                                | Название отдела, в котором работает пользователь. Поддерживает \$фильтр.                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| displayName       | Строка                                                | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.                                                                                                                                                                                                                                                           |
| externalSource    | `educationExternalSource`                             | Источник для создания пользователя. Возможные значения: `sis` или `manual`.                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| givenName         | String                                                | Простое имя пользователя. Поддерживает \$фильтр.                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| mail              | String                                                | SMTP-адрес пользователя, например "victor@contoso.onmicrosoft.com". Только для чтения. Поддерживает \$фильтр.                                                                                                                                                                                                                                                                                                                                                                                                                        |
| mailNickname      | String                                                | Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает \$фильтр.                                                                                                                                                                                                                                                                                                                                                                                                                          |
| mailingAddress    | [physicalAddress]                                     | Почтовый адрес пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| middleName        | String                                                | Отчество пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mobilePhone       | String                                                | Основной сотовый телефон пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Онпремисесинфо    | [Едукатиононпремисесинфо](educationonpremisesinfo.md) | Дополнительные сведения, используемые для связи пользователя AAD с аналогом Active Directory.                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| passwordPolicies  | String                                                | Задает политики паролей для пользователя. Это свойство представляет собой перечисление с возможным значением "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Два значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".                                                                                                                                                                      |
| passwordProfile   | [Passwordprofile необходима]                                     | Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.                                                                                                                                                                                                                             |
| preferredLanguage | String                                                | Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1. Пример: "ru-RU".                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| primaryRole       | string                                                | Роль по умолчанию для пользователя. Роль пользователя для отдельного курса может отличаться. Возможные значения: `student`, `teacher`, `faculty`. Поддерживает \$фильтр.                                                                                                                                                                                                                                                                                                                                                                     |
| provisionedPlans  | Коллекция [коллекция provisionedplan]                          | Планы, подготовленные для пользователя. Только для чтения. Значение NULL не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| residenceAddress  | [physicalAddress]                                     | Адрес проживания пользователя.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| student           | [educationStudent]                                    | Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| surname           | String                                                | Фамилия пользователя. Поддерживает \$фильтр.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| teacher           | [educationTeacher]                                    | Если основная роль — преподаватель, этот блок будет содержать данные, характерные для преподавателя.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| usageLocation     | String                                                | Двухбуквенный код страны (по стандарту ISO 3166). Свойство необходимо указывать для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в странах или регионах. Примеры: "RU", "JP", "GB". Значение null не допускается. Поддерживает \$фильтр.                                                                                                                                                                                                                                                               |
| userPrincipalName | String                                                | Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](organization.md). Поддерживает параметры $filter и $orderby. |
| userType          | String                                                | Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость". Поддерживает \$фильтр.                                                                                                                                                                                                                                                                                                                                                                                                       |

>[!IMPORTANT]
>При использовании делегированных областей разрешений Graph будет возвращать только `id`ограниченный набор свойств:, `primaryRole`, `accountEnabled`, `displayName` `givenName` `surname` `userPrincipalName`,,,, `userType`,. `onPremisesInfo` Если для приложения требуются дополнительные свойства, необходимо использовать области разрешений приложения.

## <a name="relationships"></a>Отношения

| Отношение  | Тип                         | Описание                                  |
| :------------ | :--------------------------- | :------------------------------------------- |
| assignments   | [educationAssignment]        | Список назначений для пользователя. Допускается значение null.  |
| classes       | Коллекция [educationClass]  | Курсы пользователя. Допускается значение NULL. |
| schools       | Коллекция [educationSchool] | Учебные заведения пользователя. Допускается значение NULL. |
| Таугхтклассес | Коллекция [educationClass]  | Классы, для которых пользователь является преподавателем.     |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "accountEnabled": true,
  "assignedLicenses": [{ "@odata.type": "microsoft.graph.assignedLicense" }],
  "assignedPlans": [{ "@odata.type": "microsoft.graph.assignedPlan" }],
  "businessPhones": ["String"],
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "department": "String",
  "displayName": "String",
  "externalSource": "string",
  "givenName": "String",
  "id": "String (identifier)",
  "mail": "String",
  "mailNickname": "String",
  "mailingAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
  "middleName": "String",
  "mobilePhone": "String",
  "officeLocation": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  },
  "passwordPolicies": "String",
  "passwordProfile": { "@odata.type": "microsoft.graph.passwordProfile" },
  "preferredLanguage": "String",
  "primaryRole": "string",
  "provisionedPlans": [{ "@odata.type": "microsoft.graph.provisionedPlan" }],
  "residenceAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
  "student": { "@odata.type": "microsoft.graph.educationStudent" },
  "surname": "String",
  "teacher": { "@odata.type": "microsoft.graph.educationTeacher" },
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource educationUser has documented navigation properties, but we thought it was a complex type!" 
  ]

}-->

[educationuser]: educationuser.md
[educationclass]: educationclass.md
[educationschool]: educationschool.md
[educationassignment]: educationassignment.md
[educationteacher]: educationteacher.md
[educationstudent]: educationstudent.md
[relatedcontact]: relatedcontact.md
[PhysicalAddress]: physicaladdress.md
[Коллекция provisionedplan]: provisionedplan.md
[passwordprofile необходима]: passwordprofile.md
[Identity]: identityset.md
[Коллекция assignedplan]: assignedplan.md
[Коллекция assignedlicense]: assignedlicense.md
[user]: user.md
[directoryobject]: directoryobject.md
