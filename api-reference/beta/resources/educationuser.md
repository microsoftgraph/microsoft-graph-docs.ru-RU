---
title: Тип ресурса educationUser
description: Пользователь в системе. Используемый для сферы образования вариант указания пользователя с тем же параметром `id`, который Microsoft Graph возвратит из конечной точки `/users`, не ограниченной сферой образования.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b3e193a49d1668d43fb311c5e43a506daaa5688a
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685084"
---
# <a name="educationuser-resource-type"></a>Тип ресурса educationUser

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Пользователь в системе. Это вариант стандартного пользовательского ресурса для образовательных [] учреждений с тем же значением, `id` что `/users` и microsoft Graph из конечной точки, отличной от образовательных учреждений.

Этот объект [] предоставляет целевое подмножество `primaryRole`свойств из основного пользовательского объекта и добавляет набор свойств для образовательных учреждений, таких как , `student`и .`teacher`

## <a name="methods"></a>Методы

| Метод                                               | Возвращаемый тип                                  | Описание                                                                   |
| :--------------------------------------------------- | :------------------------------------------- | :---------------------------------------------------------------------------- |
| [Получение educationUser](../api/educationuser-get.md)     | [educationUser]                              | Считывание свойств и связей объекта **educationUser**.             |
| [Перечисление курсов](../api/educationuser-list-classes.md) | Коллекция [educationClass]                  | Получение коллекции объектов **educationClass**, для которых пользователь является участником.    |
| [Перечисление учебных заведений](../api/educationuser-list-schools.md) | Коллекция [educationSchool]                 | Получение коллекции объектов **educationSchool**, для которых пользователь является участником. |
| [Получение пользователя](../api/educationuser-get-user.md)         | [user]                                       | Получение простого каталога **user**, который соответствует этому объекту **educationUser**. |
| [Обновление](../api/educationuser-update.md)             | [educationUser]                              | Обновление объекта **educationUser**.                                           |
| [Delete](../api/educationuser-delete.md)             | Нет                                         | Удаление объекта **educationUser**.                                           |
| [Delta](../api/educationuser-delta.md)               | Коллекция [educationUser](educationuser.md) | Получение добавочных изменений для **educationUsers**.                               |

## <a name="properties"></a>Свойства

| Свойство             | Тип                         | Описание                                                                                                                                                                                   |
| :------------------- | :--------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                       | Уникальный идентификатор пользователя. Наследуется от [directoryObject]. Ключ. Значение null не допускается. Только для чтения.                                                                                           |
| accountEnabled       | Логический                      | Если учетная запись обеспечена — значение **true**, в противном случае — **false**. Это свойство обязательно указывать при создании пользователя. Поддерживает фильтр \$.                                                                |
| assignedLicenses     | Коллекция [assignedLicense] | Лицензии, назначенные пользователю. Значение null не допускается.                                                                                                                                     |
| assignedPlans        | Коллекция [assignedPlan]    | Планы, назначенные пользователю. Только для чтения. Значение null не допускается.                                                                                                                             |
| businessPhones       | Коллекция строк            | Номера телефонов пользователя. **Примечание.** Несмотря на то что это коллекция строк, для этого свойства можно задать только один номер.                                                             |
| createdBy            | [identitySet]                | Объект, который создал пользователя.                                                                                                                                                                  |
| department           | String                       | Название отдела, в котором работает пользователь. Поддерживает фильтр \$.                                                                                                                       |
| displayName          | String                       | Имя пользователя, отображаемое в адресной книге. Поддерживает параметры $filter и $orderby.                                                                                                           |
| externalSource       | String                       | Тип внешнего источника, из которой был создан этот ресурс (автоматически определяется из `externalSourceDetail`). Возможные значения: `sis`, `lms` или `manual`.                          |
| externalSourceDetail | String                       | Имя внешнего источника, из которой были созданы эти ресурсы.                                                                                                                            |
| givenName;            | String                       | Простое имя пользователя. Поддерживает фильтр \$.                                                                                                                                   |
| почта;                 | String                       | SMTP-адрес пользователя, например "victor@contoso.onmicrosoft.com". Только для чтения. Поддерживает фильтр \$.                                                                                     |
| mailNickname         | String                       | Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает фильтр \$.                                                                                       |
| mailingAddress       | [physicalAddress]            | Почтовый адрес пользователя. Примечание. `type` Они не `postOfficeBox` поддерживаются для `educationUser` ресурсов.                                                                                       |
| middleName           | String                       | Отчество пользователя.                                                                                                                                                                      |
| mobilePhone          | String                       | Основной сотовый телефон пользователя.                                                                                                                                           |
| onPremisesInfo       | [educationOnPremisesInfo]    | Дополнительные сведения, используемые для AAD пользователя с его аналогом Active Directory.                                                                                                 |
| passwordPolicies     | String                       | Задает политики паролей для пользователя. Дополнительные [сведения см] . в разделе "Стандартный ресурс пользователя".                                                                                                |
| passwordProfile      | [passwordProfile]            | Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Дополнительные [сведения см] . в разделе "Стандартный ресурс пользователя". |
| preferredLanguage    | String                       | Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1. Пример: "ru-RU".                                                                                                      |
| primaryRole          | string                       | Роль по умолчанию для пользователя. Роль пользователя для отдельного курса может отличаться. Возможные значения: `student`, `teacher`, `faculty`. Поддерживает фильтр \$.                                  |
| provisionedPlans     | Коллекция [provisionedPlan] | Планы, подготовленные для пользователя. Только для чтения. Значение NULL не допускается.                                                                                                                         |
| relatedContacts      | [Коллекция relatedContact]  | Связанные записи, связанные с пользователем. Возможные связи: `parent`, `relative`, `aide`, `doctor`, `guardian`, `other``child``unknownFutureValue`                                    |
| residenceAddress     | [physicalAddress]            | Адрес проживания пользователя. Примечание. `type` Они не `postOfficeBox` поддерживаются для `educationUser` ресурсов.                                                                                   |
| student              | [educationStudent]           | Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.                                                                                                                |
| surname              | String                       | Фамилия пользователя. Поддерживает фильтр \$.                                                                                                                             |
| teacher              | [educationTeacher]           | Если основной ролью является преподаватель, этот блок будет содержать конкретные данные преподавателя.                                                                                                                |
| usageLocation        | String                       | Двухбуквенный код страны ([ISO 3166 Alpha-2]). Требуется для пользователей, которым будут назначены лицензии. Значение null не допускается. Поддерживает фильтр \$.                                                            |
| userPrincipalName    | String                       | Имя участника-пользователя (UPN) для пользователя. Поддерживает параметры $filter и $orderby. Дополнительные [сведения см] . в разделе "Стандартный ресурс пользователя".                                                               |
| userType             | String                       | Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость". Поддерживает фильтр \$.                                                                    |

> [!IMPORTANT]
> При использовании областей делегированных разрешений Graph возвращает только ограниченный набор свойств: `id`, , `primaryRole`, `accountEnabled`, `displayName`, , `userType``givenName``student/externalId``surname``onPremisesInfo``userPrincipalName``teacher/externalId`. Если приложению требуются дополнительные свойства, необходимо использовать области разрешений приложения.

## <a name="relationships"></a>Связи

| Связь  | Тип                         | Описание                                  |
| :------------ | :--------------------------- | :------------------------------------------- |
| assignments   | [educationAssignment]        | Список назначений для пользователя. Допускается значение null.  |
| classes       | Коллекция [educationClass]  | Курсы пользователя. Допускается значение NULL. |
| schools       | Коллекция [educationSchool] | Учебные заведения пользователя. Допускается значение NULL. |
| taughtClasses | Коллекция [educationClass]  | Классы, для которых пользователь является преподавателем.     |
|Рубрики|[Коллекция educationRubric](educationrubric.md)|Если этот параметр задан, к назначению прикреплена категория оценки.|

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
  ]

}-->

[educationuser]: educationuser.md
[класс education]: educationclass.md
[educationschool]: educationschool.md
[educationassignment]: educationassignment.md
[educationteacher]: educationteacher.md
[educationstudent]: educationstudent.md
[relatedcontact]: relatedcontact.md
[physicaladdress]: physicaladdress.md
[provisionedplan]: provisionedplan.md
[passwordprofile]: passwordprofile.md
[набор удостоверений]: identityset.md
[assignedplan]: assignedplan.md
[assignedlicense]: assignedlicense.md
[user]: user.md
[directoryobject]: directoryobject.md
[educationonpremisesinfo]: educationonpremisesinfo.md
[iso 3166 alpha-2]: https://www.iso.org/obp/ui/#search
[rfc 822]: https://tools.ietf.org/html/rfc822


