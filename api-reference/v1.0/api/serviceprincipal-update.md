---
title: Обновление serviceprincipal
description: Обновление свойств объекта serviceprincipal.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 7810b008e94ec37fb8f683dfc3f551616adb93fc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024156"
---
# <a name="update-serviceprincipal"></a>Обновление servicePrincipal

Пространство имен: microsoft.graph

Обновление свойств объекта [servicePrincipal](../resources/serviceprincipal.md).

> [!IMPORTANT]
> Использование метода PATCH для настройки [**passwordCredential**](../resources/passwordcredential.md) не поддерживается. Используйте методы [addPassword](./serviceprincipal-addpassword.md) и [removePassword](./serviceprincipal-removepassword.md) для обновления пароля для servicePrincipal.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

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
|addIns| [addIn](../resources/addin.md) | Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) для его функции "FileHandler". Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документов, над которыми работает пользователь.|
|alternativeNames|Коллекция строк| Используется для получения субъектов-служб по подпискам, для идентификации групп ресурсов и полных идентификаторов ресурсов для [управляемых удостоверений](https://aka.ms/azuremanagedidentity).|
|appRoleAssignmentRequired|Boolean|Указывает, требуется ли объект **appRoleAssignment** для пользователя или группы, перед тем как Azure AD выпустит маркер пользователя или доступа для приложения. Значение null не допускается. |
|appRoles|Коллекция [appRole](../resources/approle.md)|Роли приложения, предоставляемые связанным приложением. Дополнительные сведения см. в определении свойства **appRoles** для ресурса [application](../resources/application.md). Значение null не допускается. |
|displayName|String|Отображаемое имя для субъекта-службы.|
|homepage|String|Главная или начальная страница приложения.|
|keyCredentials|Коллекция [keyCredential](../resources/keycredential.md)|Коллекция ключевых учетных данных, связанных с субъектом-службой. Значение null не допускается.            |
|logoutUrl|String| Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.|
|oauth2PermissionScopes|Коллекция [permissionScope](../resources/permissionScope.md)|Области разрешений OAuth 2.0, предоставляемые связанным приложением. Дополнительные сведения см. в определении свойства **oauth2PermissionScopes** для ресурса [application](../resources/application.md). Значение null не допускается.|
|preferredSingleSignOnMode|Строка|Указывает режим единого входа, настроенный для этого приложения. Azure AD использует предпочитаемый режим единого входа для запуска этого приложения из Microsoft 365 или из раздела "Мои приложения" Azure AD. Поддерживаемые значения: `password`, `saml`, `external` и `oidc`.|
|replyUrls|Коллекция String|URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения. Значение null не допускается. |
|ServicePrincipalNames|Коллекция объектов string|Содержит список объектов **identifiersUris**, скопированных из связанного объекта [application](../resources/application.md). К гибридным приложениям можно добавить дополнительные значения. С помощью этих значений можно идентифицировать разрешения, предоставленные этим приложением в Azure AD. Пример.<ul><li>Клиентские приложения, запрашивающие разрешения на доступ к этому ресурсу, могут использовать эти URI для указания необходимых разрешений в свойстве **requiredResourceAccess** манифеста приложения или в колонке "Разрешения API" в интерфейсе регистрации приложений.</li><li>Клиентские приложения могут указывать URI ресурса, основанный на значениях этого свойства, чтобы получать маркер доступа, который представляет собой URI, возвращенный в запросе "aud".</li></ul><br>Для выражений фильтра для свойств с несколькими значениями требуется оператор any. Значение NULL не допускается.|
|tags|Коллекция String| Настраиваемые строки, которые можно использовать для классификации и определения приложения. Значение null не допускается. |
| tokenEncryptionKeyId |String|Задает значение открытого ключа keyId из коллекции keyCredentials. Если это свойство настроено, Azure AD выпускает маркеры для этого приложения в зашифрованном виде; шифрование производится с помощью ключа, указанного эти свойством. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `204 No Content` и обновленный объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/{id}
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

---


### <a name="response"></a>Отклик
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

