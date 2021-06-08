---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 9a96286b2f50d05289663e68e5db78d3a3696580
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787107"
---
# <a name="update-user"></a>Обновление пользователя

Пространство имен: microsoft.graph

Обновление свойств объекта [user](../resources/user.md). Не все свойства могут быть обновлены участниками или гостями с разрешениями по умолчанию без ролей администратора. [Сравните разрешения по умолчанию для участника и гостя](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions), чтобы узнать, какими свойствами они могут управлять.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | User.ReadWrite    |
|Для приложений | User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All |

>[!NOTE]
> - При обновлении свойства **passwordProfile** необходимо разрешение Directory.AccessAsUser.All.
> - Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается только для пользователей, не являющихся администраторами, или для пользователей, которым назначена одна из следующих ролей: читатель каталога, приглашающий гостей, читатель Центра сообщений или читатель отчетов. Дополнительные сведения см. в разделе "Администратор службы поддержки (паролей)" среди [встроенных ролей Azure AD](/azure/active-directory/roles/permissions-reference).  Это относится к приложениям с предоставленными разрешениями User.ReadWrite.All или Directory.ReadWrite.All (делегированными или для приложений).
> - Чтобы обновить профиль с делегированным разрешением User.ReadWrite в личной учетной записи Майкрософт, ваша личная учетная запись Майкрософт должна быть привязана к клиенту AAD.
> - Обновление свойства **личностей** требует разрешения User.ManageIdentities.All. Кроме того, добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** не допускается, если только объект **пользователя** не содержит идентификатор локальной учетной записи.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|aboutMe|String|Свободное текстовое поле, где пользователь может рассказать о себе.|
|accountEnabled|Логический| Если учетная запись обеспечена — `true`, в противном случае — `false`. Это свойство обязательно указывать при создании пользователя.    |
| ageGroup | [ageGroup](../resources/user.md#agegroup-values) | Устанавливает возрастную группу пользователя. Допустимые значения: `null`, `minor`, `notAdult` и `adult`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](../resources/user.md#legal-age-group-property-definitions). |
|birthday|DateTimeOffset|День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|businessPhones| Коллекция строк | Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.|
|city|String|Город, в котором находится пользователь.|
| companyName | String | Название организации, с которой связан пользователь. Это свойство может быть полезно для описания компании внешнего пользователя. Длина имени компании не должна превышать 64 символов. |
| consentProvidedForMinor | [consentProvidedForMinor](../resources/user.md#consentprovidedforminor-values) | Устанавливает, получено ли согласие для несовершеннолетних. Допустимые значения: `null`, `granted`, `denied` и `notRequired`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](../resources/user.md#legal-age-group-property-definitions). |
|country|String|Страна или регион, в котором находится пользователь, например `US` или `UK`.|
|department|String|Название отдела, в котором работает пользователь.|
|displayName|String|Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает `$filter` и `$orderby`.|
| employeeId | String | Идентификатор сотрудника, назначенный пользователю организацией. |
| employeeType | String | Фиксирует тип корпоративного работника. Например, `Employee`, `Contractor`, `Consultant` или `Vendor`. Возвращается только с помощью оператора `$select`. Поддерживает `$filter` с оператором `eq`.|
|givenName|String|Простое имя пользователя.|
|hireDate|DateTimeOffset|Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|interests;|Коллекция строк|Список интересов пользователя.|
|jobTitle|String|Должность пользователя.|
|почта;|String|SMTP-адрес пользователя, например `jeff@contoso.onmicrosoft.com`. Изменение этого свойства также приведет к обновлению коллекции пользователя **proxyAddresses**, которая будет включать это значение как SMTP-адрес. <br><br>Поддерживает `$filter`.|
|mailNickname|String|Псевдоним электронной почты пользователя. Это свойство должно быть указано при создании пользователя.|
|mobilePhone|String|Основной сотовый телефон пользователя.|
|mySite|String|URL-адрес личного сайта пользователя.|
|officeLocation|String|Расположение офиса на месте работы пользователя.|
|onPremisesImmutableId|String|Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD. Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен. **Важно!** В этом свойстве не допускается использование символов **$** и **_**.                            |
|otherMails|String |Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.|
|passwordPolicies|String|Задает политики паролей для пользователя. Это свойство представляет собой перечисление с возможным значением `DisableStrongPassword`. Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение `DisablePasswordExpiration`. Два значения можно указать одновременно. Пример: `DisablePasswordExpiration, DisableStrongPassword`.|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md)|Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль. Это невозможно использовать для федеративных пользователей.|
|pastProjects|Коллекция строк|Список предыдущих проектов пользователя.|
|postalCode|String|Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.|
|preferredLanguage|String|Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например `en-US`.|
|responsibilities;|Коллекция строк|Список обязанностей пользователя.|
|schools|Коллекция строк|Список учебных заведений, которые посещал пользователь.|
|skills|Коллекция строк|Список навыков пользователя.|
|state|String|Область, республика, край или округ в адресе пользователя.|
|streetAddress|String|Почтовый адрес места работы пользователя.|
|surname|String|Фамилия пользователя.|
|usageLocation|String|Двухбуквенный код страны (по стандарту ISO 3166). Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.  Примеры: `US`, `JP` и `GB`. Значение null не допускается.|
|userPrincipalName|String|Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). Поддерживает `$filter` и `$orderby`.
|userType|String|Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например `Member` и `Guest`.          |

> [!NOTE] 
> Следующие свойства не могут быть обновлены с помощью контекста только для приложений: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** и **skills**.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="example-1-update-properties-of-the-signed-in-user"></a>Пример 1. Обновление свойств вошедшего пользователя

#### <a name="request"></a>Запрос

Ниже показан пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
Ниже показан пример отклика.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a>Пример 2. Обновление свойств указанного пользователя

#### <a name="request"></a>Запрос

Ниже показан пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приводится пример отклика.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
