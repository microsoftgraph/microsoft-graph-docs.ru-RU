---
title: Тип ресурса educationUser
description: Пользователь в системе. Используемый для сферы образования вариант указания пользователя с тем же параметром `id`, который Microsoft Graph возвратит из конечной точки `/users`, не ограниченной сферой образования.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4a1caaa7d81540f6a90052b13f04d7d3e5bf77da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463567"
---
# <a name="educationuser-resource-type"></a>Тип ресурса educationUser

Пользователь в системе. Используемый для сферы образования вариант указания пользователя с тем же параметром `id`, который Microsoft Graph возвратит из конечной точки `/users`, не ограниченной сферой образования.
Этот объект предоставляет целевое подмножество свойств из основного объекта [user](user.md), а также добавляет ряд используемых для сферы образования свойств, таких как `primaryRole`, student и teacher.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение educationUser](../api/educationuser-get.md) | [educationUser](educationuser.md) |Считывание свойств и связей объекта **educationUser**.|
|[Перечисление курсов](../api/educationuser-list-classes.md) |Коллекция [educationClass](educationclass.md)| Получение коллекции объектов **educationClass**, для которых пользователь является участником.|
|[Перечисление учебных заведений](../api/educationuser-list-schools.md) |Коллекция [educationSchool](educationschool.md)| Получение коллекции объектов **educationSchool**, для которых пользователь является участником.|
|[Получение пользователя](../api/educationuser-get-user.md) |[user](user.md)| Получение простого каталога **user**, который соответствует этому объекту **educationUser**.|
|[Обновление](../api/educationuser-update.md) | [educationUser](educationuser.md)   |Обновление объекта **educationUser**. |
|[Удаление](../api/educationuser-delete.md) | Нет |Удаление объекта **educationUser**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| Если учетная запись обеспечена — значение **true**, в противном случае — **false**. Это свойство обязательно указывать при создании пользователя. Поддерживает параметр $filter.    |
|assignedLicenses|Коллекция [assignedLicense](assignedlicense.md)|Лицензии, назначенные пользователю. Значение null не допускается.            |
|assignedPlans|Коллекция [assignedPlan](assignedplan.md)|Планы, назначенные пользователю. Только для чтения. Значение null не допускается. |
|businessPhones|Коллекция строк|Номера телефонов пользователя. **Примечание.** Несмотря на то что это коллекция строк, для этого свойства можно задать только один номер.|
|createdBy|[identitySet](identityset.md)| Объект, который создал пользователя. |
|department|String|Название отдела, в котором работает пользователь. Поддерживает параметр $filter.|
|displayName|String|Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.|
|externalSource|`educationExternalSource`| Источник для создания пользователя. Допустимые значения: `sis`, `manual`, `unkownFutureValue`.|
|givenName|String|Простое имя пользователя. Поддерживает параметр $filter.|
|id|Строка|Уникальный идентификатор пользователя. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|mail|String|SMTP-адрес пользователя, например "victor@contoso.onmicrosoft.com". Только для чтения. Поддерживает параметр $filter.|
|mailingAddress|[physicalAddress](physicaladdress.md)| Почтовый адрес пользователя.|
|mailNickname|String|Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает параметр $filter.|
|middleName| String | Отчество пользователя.|
|mobilePhone|String|Основной сотовый телефон пользователя.|
|passwordPolicies|String|Задает политики паролей для пользователя. Это свойство представляет собой перечисление с возможным значением "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Два значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.|
|preferredLanguage|String|Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1. Пример: "ru-RU".|
|primaryRole|Едукатионусерроле| Роль по умолчанию для пользователя. Роль пользователя для отдельного курса может отличаться. Допустимые значения: `student`, `teacher`, `unknownFutureValue`. Поддерживает параметр $filter.|
|provisionedPlans|Коллекция [ProvisionedPlan](provisionedplan.md)|Планы, подготовленные для пользователя. Только для чтения. Значение null не допускается. |
|Релатедконтактс|Коллекция [релатедконтакт](relatedcontact.md)|Набор контактов, относящихся к пользователю.  Это необязательное свойство должно быть указано в предложении $select и может извлекаться только для отдельного пользователя.|
|residenceAddress|[physicalAddress](physicaladdress.md)| Адрес проживания пользователя.|
|student|[educationStudent](educationstudent.md)| Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.|
|surname|String|Фамилия пользователя. Поддерживает параметр $filter.|
|teacher|[educationTeacher](educationteacher.md)| Если основная роль — teacher, этот блок будет содержать данные, касающиеся преподавателя.|
|usageLocation|String|Двухбуквенный код страны (по стандарту ISO 3166). Свойство необходимо указывать для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в странах или регионах. Примеры: "RU", "JP", "GB". Значение null не допускается. Поддерживает параметр $filter.|
|userPrincipalName|String|Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](organization.md). Поддерживает параметры $filter и $orderby.
|userType|String|Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость". Поддерживает параметр $filter.          |

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|classes|Коллекция [educationClass](educationclass.md)| Курсы пользователя. Допускается значение null.|
|schools|Коллекция [educationSchool](educationschool.md)| Учебные заведения пользователя. Допускается значение NULL.|
|assignments| [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta)| Список назначений для пользователя. Допускается значение null.|
|user|[user](user.md)| Пользователь каталога, соответствующий этому пользователю.|

>**Примечание.** Ресурс **educationassignment** доступен в бета-версии. Если вы его используете, периодически просматривайте [журнал изменений](/graph/changelog). Когда ресурсы API Microsoft Graph выпускаются для конечной точки 1.0, этот выпуск регистрируется в журнале изменений. Если для приложения используется ресурс **educationassignment**, необходимо объявить URL-адреса базового запроса, как показано в приведенном ниже блоке кода.  
```JavaScript
var v1BaseUrl = “https://graph.microsoft.com/v1.0/education”;
var betaBaseUrl = “https://graph.microsoft.com/beta/education”;  // for administrativeUnit and educationOrganization
```


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "id": "string",
  "accountEnabled": true,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["555-555-6568"],
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "middleName": "string",
  "surname": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalSource": "string",
  "mailingAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "preferredLanguage": "string",
  "primaryRole": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "residenceAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "student": {"@odata.type": "microsoft.graph.educationStudent"},
  "teacher": {"@odata.type": "microsoft.graph.educationTeacher"},
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string"
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
    "Error: microsoft.graph.educationUser/assignments:
      Referenced type microsoft.graph.educationAssignment is not defined in the doc set! Potential suggestion: UNKNOWN",
    "Warning: /api-reference/v1.0/resources/educationuser.md/microsoft.graph.educationUser:
      Property 'relatedContacts' found in markdown table but not in resource definition."
  ],
  "tocPath": ""
}-->
