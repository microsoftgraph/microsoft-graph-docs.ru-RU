---
title: Обновление приложения
description: Обновление свойств объекта приложения.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 027735c3bbffe4baf16e5a0f2fb94f2bfb192343
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787830"
---
# <a name="update-application"></a>Обновление приложения

Пространство имен: microsoft.graph

Обновление свойств объекта [приложения.](../resources/application.md)

> [!IMPORTANT]
> Использование метода PATCH для настройки [**passwordCredential**](../resources/passwordcredential.md) не поддерживается. Чтобы обновить пароль для приложения, используйте методы [addPassword](./application-addpassword.md) и [removePassword.](./application-removepassword.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Application.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Application.ReadWrite.All |
|Для приложений | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:----------|
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство                | Тип                                                                        | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|:------------------------|:----------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| api                     | [apiApplication](../resources/apiapplication.md)                            | Задает параметры приложения, реализующего веб-API.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| appRoles                | Коллекция [appRole](../resources/approle.md)                               | Коллекция ролей приложения, которые могут быть объявлены приложением. Эти роли могут назначаться пользователям, группам или субъектам-службам. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                |
| displayName             | String                                                                      | Отображаемое имя приложения.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| groupMembershipClaims   | String                                                                      | Настраивает **требования групп,** выдаваемые пользователем или маркером доступа OAuth 2.0, который ожидает приложение. Чтобы задать этот атрибут, используйте одно из следующих допустимых строковых значений.<ul><li>`None`</li><li>`SecurityGroup`: Для групп безопасности и ролей Azure Active Directory (Azure AD)</li><li>`All` — предоставит все группы безопасности, группы рассылки и роли каталога Azure AD, членом которых является выполнивший вход пользователь</li></ul>                                                                                                                       |
| identifierUris          | Коллекция String                                                           | URI, идентифицирующие приложение в клиенте Azure AD или в проверенном личном домене, если приложение является мультитенантным. Дополнительные сведения см. в разделе [Объекты приложения и субъекта-службы](/azure/active-directory/develop/app-objects-and-service-principals). Для выражений фильтра в случае многозначных свойств требуется оператор *any*. Значение null не допускается.                                                                                                                                                 |
| info                    | [informationalUrl](../resources/informationalurl.md)                        | Основные сведения о профиле приложения, такие как маркетинг приложения, поддержка, условия службы и URL-адреса заявлений о конфиденциальности. Условия обслуживания и заявление о конфиденциальности отображаются в окне запроса согласия пользователя. Дополнительные сведения см. в [сообщении Add Terms of service and privacy statement for registered Azure AD apps.](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement)                                                                                                                       |
| isFallbackPublicClient  | Boolean                                                                     | Указывает резервный тип приложения как общедоступный клиент, например установленное приложение, запущенное на мобильном устройстве. Значение по умолчанию означает, что тип приложения-отката — это `false` конфиденциальный клиент, например веб-приложение. Существуют определенные сценарии, в которых Azure AD не может определить тип клиентского приложения (например, поток [ROPC,](https://tools.ietf.org/html/rfc6749#section-4.3) где он настроен без указания URI перенаправления). В этих случаях Azure AD будет интерпретировать тип приложения в зависимости от значения этого свойства. |
| keyCredentials          | Коллекция [keyCredential](../resources/keycredential.md)                   | Коллекция ключевых учетных данных, связанных с приложением. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| logo                    | Stream                                                                      | Основной логотип для приложения. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| optionalClaims          | optionalClaims                                                              | Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт). Дополнительные [сведения см. в дополнительных](/azure/active-directory/develop/active-directory-optional-claims) утверждениях.                                                                                                                                                                                                                                     |
| parentalControlSettings | [parentalControlSettings](../resources/parentalcontrolsettings.md)          | Указывает параметры родительского контроля для приложения.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| publicClient            | [publicClientApplication](../resources/publicclientapplication.md)          | Указывает параметры для установленных клиентов, например классических или мобильных устройств.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| requiredResourceAccess  | Коллекция [requiredResourceAccess](../resources/requiredresourceaccess.md) | Указывает ресурсы, к которым приложению требуется доступ, и устанавливает области разрешений OAuth и роли приложения, требующиеся приложению для каждого из этих ресурсов. Эта предварительная настройка доступа к необходимым ресурсам определяет интерфейс предоставления согласия. Значение null не допускается.                                                                                                                                                                                                                                                                                                 |
| signInAudience          | String                                                                      | Указывает, какие учетные записи Майкрософт поддерживаются для текущего приложения. Поддерживаемые значения:<ul><li>`AzureADMyOrg` — пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD моей организации (т. е. один клиент)</li><li>`AzureADMultipleOrgs` — пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD любой организации (т. е. несколько клиентов)</li> <li>`AzureADandPersonalMicrosoftAccount` — пользователи с личной учетной записью Майкрософт, рабочей или учебной учетной записью в клиенте Azure AD любой организации</li></ul>                           |
| tags                    | Коллекция String                                                           | Настраиваемые строки, которые можно использовать для классификации и определения приложения. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| tokenEncryptionKeyId    | String                                                                      | Задает значение открытого ключа keyId из коллекции keyCredentials. При настройке Azure AD шифрует все созданные маркеры с помощью ключа, на который указывает это свойство. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.                                                                                                                                                                                                                               |
| web                     | [webApplication](../resources/webapplication.md)                            | Указывает параметры для веб-приложения.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и ничего не возвращает `204 No Content` в тексте ответа.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/applications/{id}
Content-type: application/json
Content-length: 72

{
  "displayName": "New display name"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

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
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
