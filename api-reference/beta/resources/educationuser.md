---
title: Тип ресурса educationUser
description: Пользователь в системе. Используемый для сферы образования вариант указания пользователя с тем же параметром `id`, который Microsoft Graph возвратит из конечной точки `/users`, не ограниченной сферой образования.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: a577fae0896ca4f32b0266f5353e963ce0c7d35a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822752"
---
# <a name="educationuser-resource-type"></a>Тип ресурса educationUser

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
|assignedPlans|Коллекция [assignedPlan](assignedplan.md)|Планы, назначенные пользователю. Только для чтения. Значение NULL не допускается. |
|businessPhones|Коллекция строк|Номера телефонов пользователя. **Примечание.** Несмотря на то что это коллекция строк, для этого свойства можно задать только один номер.|
|createdBy|[identitySet](identityset.md)| Объект, который создал пользователя. |
|department|String|Название отдела, в котором работает пользователь. Поддерживает параметр $filter.|
|displayName|String|Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.|
|externalSource|`educationExternalSource`| Источник для создания пользователя. Возможные значения: `sis`, `manual`, `unkownFutureValue`.|
|givenName|String|Имя пользователя. Поддерживает параметр $filter.|
|id|String|Уникальный идентификатор пользователя. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение NULL не допускается. Только для чтения.|
|mail|String|SMTP-адрес пользователя, например "victor@contoso.onmicrosoft.com". Только для чтения. Поддерживает параметр $filter.|
|mailingAddress|[physicalAddress](physicaladdress.md)| Почтовый адрес пользователя.|
|mailNickname|String|Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает параметр $filter.|
|middleName| String | Отчество пользователя.|
|mobilePhone|String|Основной номер мобильного телефона пользователя.|
|passwordPolicies|String|Задает политики паролей для пользователя. Это свойство представляет собой перечисление с возможным значением "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Два значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.|
|preferredLanguage|String|Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1. Пример: "ru-RU".|
|primaryRole|string| Роль по умолчанию для пользователя. Роль пользователя для отдельного курса может отличаться. Возможные значения: `student`, `teacher`, `enum_sentinel`. Поддерживает параметр $filter.|
|provisionedPlans|Коллекция [ProvisionedPlan](provisionedplan.md)|Планы, подготовленные для пользователя. Только для чтения. Значение NULL не допускается. |
|residenceAddress|[physicalAddress](physicaladdress.md)| Адрес проживания пользователя.|
|student|[educationStudent](educationstudent.md)| Если основная роль — student, этот блок будет содержать данные, касающиеся учащегося.|
|surname|String|Фамилия пользователя. Поддерживает параметр $filter.|
|teacher|[educationTeacher](educationteacher.md)| Если основная роль — teacher, этот блок будет содержать данные, касающиеся преподавателя.|
|usageLocation|String|Двухбуквенный код страны (по стандарту ISO 3166). Свойство необходимо указывать для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в странах или регионах. Примеры: "RU", "JP", "GB". Значение NULL не допускается. Поддерживает параметр $filter.|
|userPrincipalName|String|Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](organization.md). Поддерживает параметры $filter и $orderby.
|userType|String|Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например "Участник" и "Гость". Поддерживает параметр $filter.          |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|classes|Коллекция [educationClass](educationclass.md)| Курсы пользователя. Допускается значение NULL.|
|schools|Коллекция [educationSchool](educationschool.md)| Учебные заведения пользователя. Допускается значение NULL.|
|assignments| [educationAssignment](educationassignment.md)| Список заданий для пользователя. Допускается значение NULL.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "givenName": "string",
  "middleName": "string",
  "surname": "string",
  "mail": "string",
  "mobilePhone": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalSource": "string",
  "mailingAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "primaryRole": "string",
  "residenceAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "student": {"@odata.type": "microsoft.graph.educationStudent"},
  "teacher": {"@odata.type": "microsoft.graph.educationTeacher"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
