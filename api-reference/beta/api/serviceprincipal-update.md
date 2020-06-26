---
title: Обновление serviceprincipal
description: Обновление свойств объекта serviceprincipal.
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4a80b28cb42a3c23902fed139f7ccc7ec92ea794
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896135"
---
# <a name="update-serviceprincipal"></a>Обновление servicePrincipal

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [servicePrincipal](../resources/serviceprincipal.md) .

> [!IMPORTANT]
> Использование PATCH для установки [**пассвордкредентиал**](../resources/passwordcredential.md) не поддерживается. Используйте методы [аддпассворд](./serviceprincipal-addpassword.md) и [ремовепассворд](./serviceprincipal-removepassword.md) , чтобы обновить пароль для servicePrincipal.

## <a name="permissions"></a>Разрешения
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:----------|
| Авторизация | Bearer {token}. Required.  |
| Content-Type | application/json. Required. |

## <a name="request-body"></a>Текст запроса
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Логический| Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.|
| addIns | [addIn](../resources/addin.md) | Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) для его функции "FileHandler". Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документа, над которым работает пользователь.|
|алтернативенамес|Коллекция String| Используется для получения субъектов служб по подписке, идентификации группы ресурсов и полных идентификаторов ресурсов для [управляемых удостоверений](https://aka.ms/azuremanagedidentity).|
|appRoleAssignmentRequired|Boolean|Указывает, требуется ли объект **appRoleAssignment** для пользователя или группы, перед тем как Azure AD выпустит маркер пользователя или доступа для приложения. Значение null не допускается. |
|appRoles|Коллекция [appRole](../resources/approle.md)|Роли приложения, предоставляемые связанным приложением. Дополнительные сведения см. в описании свойства **appRoles** ресурса [Application](../resources/application.md) . Значение null не допускается. |
|displayName|Строка|Отображаемое имя для субъекта-службы.|
|homepage|String|Домашняя или целевая страница приложения.|
|keyCredentials|Коллекция [keyCredential](../resources/keycredential.md)|Коллекция ключевых учетных данных, связанных с субъектом-службой. Значение null не допускается.            |
|логинурл|String|Указывает URL-адрес, по которому поставщик услуг перенаправляет пользователя в Azure AD для проверки подлинности. Azure AD использует URL-адрес для запуска приложения из Microsoft 365 или Azure AD мои приложения. Если это поле не заполнено, Azure AD выполняет IdP вход для приложений, настроенных с [единым входом на основе SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-single-sign-on#saml-sso). Пользователь запускает приложение из Microsoft 365, "Мои приложения Azure AD" или URL-адрес единого входа Azure AD.|
|logoutUrl|String| Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.|
|notificationEmailAddresses|Коллекция String|Указывает список адресов электронной почты, на которые служба Azure AD отправляет уведомление, если срок действия активного сертификата приближается к дате окончания срока действия. Это относится только к сертификатам, которые используются для подписи маркера SAML, выпущенного для приложений коллекции Azure AD.|
|публишедпермиссионскопес|Коллекция [permissionScope](../resources/permissionScope.md)|Разрешения OAuth 2.0, предоставляемые связанным приложением. Дополнительные сведения см. в описании свойства **oauth2PermissionScopes** ресурса [Application](../resources/application.md) . Значение null не допускается.            |
|преферредсинглесигнонмоде|string|Задает режим единого входа, настроенный для этого приложения. Azure AD использует предпочтительный режим единого входа для запуска приложения из Microsoft 365 или Azure AD мои приложения. Поддерживаемые значения: Password, SAML, External и оидк.|
|преферредтокенсигнингкэйенддатетиме|DateTimeOffset|Задает дату истечения срока действия Кэйкредентиал, которая используется для подписи маркеров, помеченной **преферредтокенсигнингкэйсумбпринт**.|
|preferredTokenSigningKeyThumbprint|String|Зарезервировано только для внутреннего использования. Не записывайте и не используйте иным образом это свойство. Может быть удалено в будущих версиях. |
|publisherName|String|Отображаемое имя клиента, в котором указано связанное приложение.|
|replyUrls|Коллекция String|URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения. Значение null не допускается. |
|самлсинглесигнонсеттингс|[самлсинглесигнонсеттингс](../resources/samlsinglesignonsettings.md)|Коллекция параметров, связанных с единым входом SAML.|
|ServicePrincipalNames|Коллекция String|Содержит список **идентифиерсурис**, скопированных из связанного [приложения](../resources/application.md). В гибридные приложения можно добавлять дополнительные значения. Эти значения можно использовать для определения разрешений, предоставляемых приложением в Azure AD. For example,<ul><li>Клиентские приложения, запрашивающие разрешения для этого ресурса, могут использовать эти URI для указания необходимых разрешений в свойстве **рекуиредресаурцеакцесс** манифеста приложения или в колонке "разрешения API" в функции регистрации приложений.</li><li>Клиентские приложения могут указывать URI ресурса, основанный на значениях этого свойства для получения маркера доступа, который представляет собой URI, возвращенный в утверждении "ауд".</li></ul><br>Для выражений фильтра в случае многозначных свойств требуется оператор any. Значение null не допускается.|
|tags|Коллекция String| Значение null не допускается. |
|tokenEncryptionKeyId|String|Задает значение открытого ключа keyId из коллекции keyCredentials. При настройке в Azure AD маркеры проблем для этого приложения шифруются с помощью ключа, указанного этим свойством. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и обновленный объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.
## <a name="examples"></a>Примеры
### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

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

---


### <a name="response"></a>Отклик
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
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
