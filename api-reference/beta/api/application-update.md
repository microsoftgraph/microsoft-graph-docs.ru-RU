---
title: Обновление приложения
description: Обновление свойств объекта приложения.
author: sureshja
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 9c5f3d6cb9be4d8b5456e5d348e9cc89d874c007
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555543"
---
# <a name="update-application"></a>Обновление приложения

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств [объекта приложения.](../resources/application.md)

> [!IMPORTANT]
> Использование метода PATCH для настройки [**passwordCredential**](../resources/passwordcredential.md) не поддерживается. Используйте методы [addPassword](./application-addpassword.md) и [removePassword](./application-removepassword.md) для обновления пароля или секрета приложения.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Application.ReadWrite.All, Directory.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Application.ReadWrite.All    |
|Приложение | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
Замените `{id}` **идентификатор объекта** приложения, который также называется идентификатором **объекта в портал Azure**.
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
| groupMembershipClaims   | String                                                                      | Настраивает утверждение **группы,** выданное пользователем или маркером доступа OAuth 2.0, который ожидает приложение. Чтобы задать этот атрибут, используйте одно из следующих допустимых строковых значений.<ul><li>`None`</li><li>`SecurityGroup`: для групп безопасности и ролей Azure Active Directory (Azure AD)</li><li>`All` — предоставит все группы безопасности, группы рассылки и роли каталога Azure AD, членом которых является выполнивший вход пользователь</li></ul>                                                                                                                       |
| identifierUris          | Коллекция String                                                           | URI, идентифицирующие приложение в клиенте Azure AD или в проверенном личном домене, если приложение является мультитенантным. Дополнительные сведения см. в разделе [Объекты приложения и субъекта-службы](/azure/active-directory/develop/app-objects-and-service-principals). Для выражений фильтра в случае многозначных свойств требуется оператор *any*. Значение null не допускается.                                                                                                                                                                           |
| info                    | [informationalUrl](../resources/informationalurl.md)                        | Основные сведения о профиле приложения, такие как маркетинг приложения, поддержка, условия обслуживания и URL-адреса заявлений о конфиденциальности. Условия обслуживания и заявление о конфиденциальности отображаются в окне запроса согласия пользователя. Дополнительные сведения см. в разделе "Добавление условий обслуживания и заявление о конфиденциальности для зарегистрированных Azure AD [приложений"](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement).                                                                                                                                                 |
| isFallbackPublicClient  | Boolean                                                                     | Указывает резервный тип приложения как общедоступный клиент, например установленное приложение, запущенное на мобильном устройстве. Значение по умолчанию — это `false`означает, что резервным типом приложения является конфиденциальный клиент, например веб-приложение. Существуют некоторые сценарии, в которых Azure AD не может определить тип клиентского приложения (например, поток [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3), в котором он настроен без указания URI перенаправления). В таких случаях Azure AD будет интерпретировать тип приложения на основе значения этого свойства. |
| keyCredentials          | Коллекция [keyCredential](../resources/keycredential.md)                   | Коллекция ключевых учетных данных, связанных с приложением. Значение NULL не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| logo                    | Stream                                                                      | Основной логотип для приложения. Значение NULL не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| onPremisesPublishing    | [onPremisesPublishing](../resources/onpremisespublishing.md)                | Представляет набор свойств для настройки [Azure AD Application Proxy для](/azure/active-directory/app-proxy/what-is-application-proxy) локального приложения. Это свойство можно задать только после создания приложения и не может быть обновлено в том же запросе, что и другие свойства приложения.                                                                                                                                                                                                                                                                                                                                                       |
| optionalClaims          | optionalClaims                                                              | Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт). [Дополнительные сведения см. в дополнительных](/azure/active-directory/develop/active-directory-optional-claims) утверждениях.                                                                                                                                                                                                                                                               |
| parentalControlSettings | [parentalControlSettings](../resources/parentalcontrolsettings.md)          | Указывает параметры родительского контроля для приложения.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| publicClient            | [publicClientApplication](../resources/publicclientapplication.md)          | Указывает параметры для установленных клиентов, например классических или мобильных устройств.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| requiredResourceAccess  | Коллекция [requiredResourceAccess](../resources/requiredresourceaccess.md) | Указывает ресурсы, к которым приложению необходимо получить доступ. В этом свойстве также указывается набор делегированных разрешений и ролей приложения, необходимых для каждого из этих ресурсов. Эта настройка доступа к необходимым ресурсам определяет порядок предоставления согласия. Можно настроить не более 50 служб ресурсов (API). С середины октября 2021 г. общее количество необходимых разрешений не должно превышать 400. Значение null не допускается.                                                                                                                 |
| signInAudience          | String                                                                      | Указывает, какие учетные записи Майкрософт поддерживаются для текущего приложения. Поддерживаемые значения:<ul><li>`AzureADMyOrg` — пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD моей организации (т. е. один клиент)</li><li>`AzureADMultipleOrgs` — пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD любой организации (т. е. несколько клиентов)</li> <li>`AzureADandPersonalMicrosoftAccount` — пользователи с личной учетной записью Майкрософт, рабочей или учебной учетной записью в клиенте Azure AD любой организации</li></ul>                           |
| spa                     | [spaApplication](../resources/spaapplication.md)                            | Указывает параметры для одностраничного приложения, в том числе URL-адреса выхода и URI перенаправления для кодов авторизации и маркеров доступа. |
| tags                    | Коллекция String                                                           | Настраиваемые строки, которые можно использовать для классификации и определения приложения. Значение null не допускается.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| tokenEncryptionKeyId    | String                                                                      | Задает значение открытого ключа keyId из коллекции keyCredentials. При настройке Azure AD шифрует все созданные маркеры с помощью ключа, на который указывает это свойство. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.                                                                                                                                                                                                                               |
| uniqueName | Строка | Уникальный идентификатор, который можно назначить приложению в качестве альтернативного идентификатора. Неизменяемый. Только для чтения.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| web                     | [webApplication](../resources/webapplication.md)                            | Указывает параметры для веб-приложения.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| spa                     | [spaApplication](../resources/spaapplication.md)                            | Указывает параметры для одностраничного приложения, в том числе URL-адреса выхода и URI перенаправления для кодов авторизации и маркеров доступа. |
| windows                     | [windowsApplication](../resources/windowsapplication.md)                            | Указывает параметры приложений для устройств под управлением Microsoft Windows, опубликованных в Microsoft Store или магазине игр Xbox. Включает идентификатор безопасности пакета и URI перенаправления для кодов авторизации и маркеров доступа. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `204 No Content` отклика и ничего не возвращает в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json

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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-application-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-application-powershell-snippets.md)]
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
