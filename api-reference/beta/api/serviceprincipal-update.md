---
title: Обновление serviceprincipal
description: Обновление свойств объекта serviceprincipal.
author: sureshja
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: applications
ms.openlocfilehash: e6ef2e9fde5946d224fa356937b699eefe7c73e6
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225251"
---
# <a name="update-serviceprincipal"></a>Обновление servicePrincipal

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [servicePrincipal](../resources/serviceprincipal.md).

> [!IMPORTANT]
> Использование метода PATCH для настройки [**passwordCredential**](../resources/passwordcredential.md) не поддерживается. Используйте методы [addPassword](./serviceprincipal-addpassword.md) и [removePassword](./serviceprincipal-removepassword.md) для обновления пароля для servicePrincipal.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:----------|
| Авторизация | Bearer {token}. Обязательный.  |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.|
| addIns | [addIn](../resources/addin.md) | Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](/onedrive/developer/file-handlers/) для его функции "FileHandler". Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документов, над которыми работает пользователь.|
|alternativeNames|Коллекция строк| Используется для получения субъектов-служб по подпискам, для идентификации групп ресурсов и полных идентификаторов ресурсов для [управляемых удостоверений](/azure/active-directory/managed-identities-azure-resources/overview).|
|appRoleAssignmentRequired|Boolean|Указывает, требуется ли объект **appRoleAssignment** для пользователя или группы, перед тем как Azure AD выпустит маркер пользователя или доступа для приложения. Значение null не допускается. |
|appRoles|Коллекция [appRole](../resources/approle.md)|Роли приложения, предоставляемые связанным приложением. Дополнительные сведения см. в определении свойства **appRoles** для ресурса [application](../resources/application.md). Значение null не допускается. |
|customSecurityAttributes|[customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|Открытый сложный тип, который содержит значение настраиваемого атрибута безопасности, назначенного объекту каталога.<br/><br/>Чтобы обновить это свойство, вызывающему субъекту должна быть назначена роль администратора назначения атрибутов и должно быть предоставлено разрешение *CustomSecAttributeAssignment.ReadWrite.All*.|
|displayName|String|Отображаемое имя для субъекта-службы.|
|homepage|String|Главная или начальная страница приложения.|
|keyCredentials|Коллекция [keyCredential](../resources/keycredential.md)|Коллекция ключевых учетных данных, связанных с субъектом-службой. Значение null не допускается.            |
|loginUrl|String|Указывает URL-адрес, по которому поставщик услуг перенаправляет пользователя в Azure AD для проверки подлинности. Azure AD использует этот URL-адрес для запуска приложения из Microsoft 365 или из раздела "Мои приложения" в Azure AD. Если оставить пустое значение, Azure AD осуществляет вход на основе IdP для приложений, для которых настроен [единый вход на базе SAML](/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso). Пользователь запускает приложение из Microsoft 365, из раздела "Мои приложения" в Azure AD или по URL-адресу единого входа Azure AD.|
|logoutUrl|String| Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.|
|notificationEmailAddresses|Коллекция строк|Указывает список адресов электронной почты, по которым Azure AD отправляет уведомление, когда приближается срок окончания действия активного сертификата. Используется только для сертификатов, с помощью которых подписан маркер SAML, выпущенный для приложений коллекции Azure AD.|
|publishedPermissionScopes|Коллекция [permissionScope](../resources/permissionScope.md)|Разрешения OAuth 2.0, предоставляемые связанным приложением. Дополнительные сведения см. в определении свойства **oauth2PermissionScopes** для ресурса [application](../resources/application.md). Значение null не допускается.            |
|preferredSingleSignOnMode|Строка|Указывает режим единого входа, настроенный для этого приложения. Azure AD использует предпочитаемый режим единого входа для запуска этого приложения из Microsoft 365 или из раздела "Мои приложения" Azure AD. Поддерживаются значения: password, saml, external, oidc.|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|Указывает дату окончания срока действия keyCredential, использованного для подписи маркера, помеченного с помощью **preferredTokenSigningKeyThumbprint**.|
|preferredTokenSigningKeyThumbprint|String|Зарезервировано только для внутреннего использования. Не записывайте и не используйте иным образом это свойство. Может быть удалено в будущих версиях. |
|publisherName|String|Отображаемое имя клиента, в котором указано связанное приложение.|
|replyUrls|Коллекция String|URL-адреса, по которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, по которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения. Значение NULL не допускается. |
|samlSingleSignOnSettings|[samlSingleSignOnSettings](../resources/samlsinglesignonsettings.md)|Коллекция для параметров, связанных с единым входом SAML.|
|ServicePrincipalNames|Коллекция объектов string|Содержит список объектов **identifiersUris**, скопированных из связанного объекта [application](../resources/application.md). К гибридным приложениям можно добавить дополнительные значения. С помощью этих значений можно идентифицировать разрешения, предоставленные этим приложением в Azure AD. Пример.<ul><li>Клиентские приложения, запрашивающие разрешения на доступ к этому ресурсу, могут использовать эти URI для указания необходимых разрешений в свойстве **requiredResourceAccess** манифеста приложения или в колонке "Разрешения API" в интерфейсе регистрации приложений.</li><li>Клиентские приложения могут указывать URI ресурса, основанный на значениях этого свойства, чтобы получать маркер доступа, который представляет собой URI, возвращенный в запросе "aud".</li></ul><br>Для выражений фильтра для свойств с несколькими значениями требуется оператор any. Значение NULL не допускается.|
|tags|Коллекция String| Значение null не допускается. |
|tokenEncryptionKeyId|String|Задает значение открытого ключа keyId из коллекции keyCredentials. Если это свойство настроено, Azure AD выпускает маркеры для этого приложения в зашифрованном виде; шифрование производится с помощью ключа, указанного эти свойством. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `204 No Content` и обновленный объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-update-properties-of-the-specified-service-principal"></a>Пример 1. Обновление свойств указанного субъекта-службы

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json

{
  "appRoleAssignmentRequired": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-serviceprincipal-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-serviceprincipal-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


### <a name="example-2-assign-a-custom-security-attribute-with-a-string-value-to-a-service-principal"></a>Пример 2. Назначение настраиваемого атрибута безопасности со строковым значением субъекту-службе

В следующем примере показано, как назначить субъекту-службе настраиваемый атрибут безопасности со строковым значением.

+ Набор атрибутов: `Engineering`
+ Атрибут: `ProjectDate`
+ Тип данных атрибута: строка
+ Значение атрибута: `"2022-10-01"`

Чтобы назначить настраиваемые атрибуты безопасности, вызывающему субъекту должна быть присвоена роль администратора назначения атрибутов и должно быть предоставлено разрешение *CustomSecAttributeAssignment.ReadWrite.All*.

Другие аналогичные примеры для пользователей см. в статье [Назначение, обновление или удаление настраиваемых атрибутов безопасности с помощью API Microsoft Graph](/graph/custom-security-attributes-examples).

#### <a name="request"></a>Запрос



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "assign_serviceprincipal_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/assign-serviceprincipal-customsecurityattribute-string-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-serviceprincipal-customsecurityattribute-string-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/assign-serviceprincipal-customsecurityattribute-string-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/assign-serviceprincipal-customsecurityattribute-string-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
