---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: jpettere
ms.localizationpriority: high
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 274ccfc249f6fcaefc4eb99321e4dccb0f1ed90b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204262"
---
# <a name="update-user"></a>Обновление пользователя

Пространство имен: microsoft.graph

Обновление свойств объекта [user](../resources/user.md). Не все свойства могут быть обновлены участниками или гостями с разрешениями по умолчанию без ролей администратора. [Сравните разрешения по умолчанию для участника и гостя](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions), чтобы узнать, какими свойствами они могут управлять.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | User.ReadWrite    |
|Для приложений | User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All |

>[!NOTE]
> - Обновление свойств **businessPhones**, **mobilePhone** или **otherMails** других пользователей разрешается, только в отношении пользователей, которые не являются администраторами, а также для пользователей, которым назначена одна из следующих ролей: "Читатель каталога", "Приглашающий гостей", "Читатель Центра сообщений" и "Читатель отчетов". Дополнительные сведения см. в разделе "Администратор службы поддержки" (администратор паролей) в статье [Встроенные роли Azure AD](/azure/active-directory/roles/permissions-reference). Это относится к приложениям с предоставленными или делегированными разрешениями User.ReadWrite.All или Directory.ReadWrite.All. Только глобальный администратор, которому назначено разрешение Directory.AccessAsUser.All, может использовать эти свойства для администраторов с более широким набором привилегий.
> - Чтобы обновить профиль с делегированным разрешением User.ReadWrite в личной учетной записи Майкрософт, ваша личная учетная запись Майкрософт должна быть привязана к клиенту AAD.
> - Обновление свойства **Удостоверения** требует разрешения User.ManageIdentities.All. Кроме того, добавление [локальной учетной записи B2C](../resources/objectidentity.md) к существующему объекту **пользователя** не допускается, если только объект **пользователя** не содержит удостоверение локальной учетной записи.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|aboutMe|String|Свободное текстовое поле, где пользователь может рассказать о себе.|
|accountEnabled|Логический| Если учетная запись обеспечена — `true`, в противном случае — `false`. Это свойство обязательно указывать при создании пользователя. Глобальный администратор, которому назначено делегированное разрешение _Directory.AccessAsUser.All_, может обновить состояние **accountEnabled** для всех администраторов в клиенте.|
| ageGroup | [ageGroup](../resources/user.md#agegroup-values) | Устанавливает возрастную группу пользователя. Допустимые значения: `null`, `Minor`, `NotAdult` и `Adult`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](../resources/user.md#legal-age-group-property-definitions). |
|birthday|DateTimeOffset|День рождения пользователя. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и формата времени UTC. Например, полночь 1 января 2014 г. в формате UTC представляется в виде `2014-01-01T00:00:00Z`.|
|businessPhones| Коллекция строк | Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.|
|city|String|Город, в котором находится пользователь.|
| CompanyName | String | Название организации, с которой связан пользователь. Это свойство может быть полезно для описания компании внешнего пользователя. Максимальная длина: 64 символа. |
| consentProvidedForMinor | [consentProvidedForMinor](../resources/user.md#consentprovidedforminor-values) | Устанавливает, получено ли согласие для несовершеннолетних. Допустимые значения: `null`, `Granted`, `Denied` и `NotRequired`. Дополнительные сведения см. в разделе [Определения свойств юридических возрастных групп](../resources/user.md#legal-age-group-property-definitions). |
|country|String|Страна или регион, в котором находится пользователь, например `US` или `UK`.|
|department|String|Название отдела, в котором работает пользователь.|
|displayName|String|Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. |
| employeeId | String | Идентификатор сотрудника, назначенный пользователю организацией. Максимальная длина составляет 16 символов. |
| employeeType | String | Фиксирует тип корпоративного работника. Например, `Employee`, `Contractor`, `Consultant` или `Vendor`. Возвращается только с помощью оператора `$select`.|
|givenName;|String|Простое имя пользователя.|
|employeeHireDate|DateTimeOffset|Дата приема пользователя на работу. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат времени UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|interests;|Коллекция строк|Список интересов пользователя.|
|jobTitle|String|Должность пользователя.|
|почта;|String|SMTP-адрес пользователя, например `jeff@contoso.onmicrosoft.com`. Изменение этого свойства также приведет к обновлению коллекции пользователя **proxyAddresses**, которая будет включать это значение как SMTP-адрес. Для учетных записей Azure AD B2C это свойство можно обновить до десяти раз, используя уникальные адреса протокола SMTP. |
|mailNickname|String|Псевдоним электронной почты пользователя. Это свойство должно быть указано при создании пользователя.|
|mobilePhone|String|Основной сотовый телефон пользователя.|
|mySite|String|URL-адрес личного сайта пользователя.|
|officeLocation|String|Расположение офиса на месте работы пользователя.|
| onPremisesExtensionAttributes | [onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md) | Содержит свойства extensionAttribute 1–15 для пользователя. Обратите внимание, что отдельные атрибуты расширения нельзя выбирать и фильтровать. Для пользователей `onPremisesSyncEnabled` исходным центром управления для этого набора свойств является локальная среда, и он предназначен только для чтения. Эти атрибуты расширения также называются настраиваемыми атрибутами 1–15 Exchange.|
|onPremisesImmutableId|String|Это свойство используется для сопоставления локальной учетной записи пользователя Active Directory с объектом пользователя Azure AD. Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен. **Важно!** При указании этого свойства не допускается использование символов **$** и **_**.                            |
|otherMails|Коллекция строк |Список дополнительных адресов электронной почты для пользователя. Например: `["bob@contoso.com", "Robert@fabrikam.com"]`.|
|passwordPolicies|String|Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением `DisableStrongPassword`, позволяющим использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Также можно указать значение `DisablePasswordExpiration`. Эти значения допускается указывать одновременно, например `DisablePasswordExpiration, DisableStrongPassword`. |
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md)|Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль. Его невозможно использовать для федеративных пользователей.<br><br> Вызывающему пользователю должно быть назначено делегированное разрешение *Directory.AccessAsUser.All* для обновления этого свойства. Это свойство не может обновляться только с разрешениями для приложений.|
|pastProjects|Коллекция строк|Список предыдущих проектов пользователя.|
|postalCode|String|Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.|
|preferredLanguage|String|Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например `en-US`. |
|responsibilities;|Коллекция строк|Список обязанностей пользователя.|
|schools|Коллекция строк|Список учебных заведений, которые посещал пользователь.|
|skills|Коллекция строк|Список навыков пользователя.|
|state|String|Область, республика, край или округ в адресе пользователя.|
|streetAddress|String|Почтовый адрес места работы пользователя.|
|surname|String|Фамилия пользователя.|
|usageLocation|String|Двухбуквенный код страны (по стандарту ISO 3166). Необходим для пользователей, которым будут назначены лицензии, в связи с юридическим требованием проверять доступность служб в разных странах. Примеры: `US`, `JP` и `GB`. Значение NULL не допускается. |
|userPrincipalName|String|Имя субъекта-пользователя (UPN) для пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](../resources/organization.md). <br>ПРИМЕЧАНИЕ. Это свойство не может содержать диакритические знаки. Разрешены только следующие символы: `A - Z`, `a - z`, `0 - 9`, ` ' . - _ ! # ^ ~`. Полный список разрешенных символов см. в [политиках имен пользователей](/azure/active-directory/authentication/concept-sspr-policy#userprincipalname-policies-that-apply-to-all-user-accounts). |
|userType|String|Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например `Member` и `Guest`.          |

> [!NOTE] 
> - Следующие свойства невозможно обновить с помощью приложения с использованием разрешений только для приложений: **aboutMe**, **birthday**, **employeeHireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** и **skills**.
> - Чтобы обновить следующие свойства, необходимо указать их в собственном запросе PATCH, не включая другие свойства, перечисленные в таблице выше: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** and **skills**.

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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-user-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-user-powershell-snippets.md)]
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-other-user-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-other-user-powershell-snippets.md)]
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


### <a name="example-3-update-the-passwordprofile-of-a-user-to-reset-their-password"></a>Пример 3. Обновление passwordProfile пользователя для сброса его пароля

В приведенном ниже примере показан запрос на сброс пароля другого пользователя. Вызывающему пользователю должно быть назначено делегированное разрешение *Directory.AccessAsUser.All* для обновления этого свойства.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user_passwordProfile"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "passwordProfile": {
    "forceChangePasswordNextSignIn": false,
    "password": "xWwvJ]6NMw+bWH-d"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-passwordprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-passwordprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-passwordprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-passwordprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-user-passwordprofile-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-user-passwordprofile-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-4-add-or-update-the-values-of-a-schema-extension-for-a-user"></a>Пример 4. Добавление или обновление значений расширения схемы для пользователя

Можно обновить или назначить значение одному свойству или всем свойствам в расширении.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e
Content-type: application/json

{
    "ext55gb1l09_msLearnCourses": {
        "courseType": "Admin"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-schemaextension-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-schemaextension-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

>**Примечание.** Чтобы удалить значение расширения схемы из пользовательского объекта, задайте для свойства значение `null`. Например:
>
>```http
>PATCH https://graph.microsoft.com/v1.0/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e
>Content-type: application/json
>
>{
>    "ext55gb1l09_msLearnCourses": null
>}
>```

## <a name="see-also"></a>Дополнительные ресурсы

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](/graph/extensibility-open-users)
- [Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](/graph/extensibility-schema-groups)

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
