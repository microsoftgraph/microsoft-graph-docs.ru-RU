---
title: Обновление serviceprincipal
description: Обновление свойств объекта serviceprincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 852ea0467779ba0dab80eb0c571f39b1cf60ed9b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410134"
---
# <a name="update-serviceprincipal"></a>Обновление serviceprincipal

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта serviceprincipal.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Boolean|                Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.            |
|appDisplayName|String|Отображаемое имя, предоставляемое связанным приложением.|
|appId|String|Уникальный идентификатор для связанного приложения (его свойство **appId**).|
|appRoleAssignmentRequired|Boolean|Указывает, требуется ли объект **appRoleAssignment** для пользователя или группы, перед тем как Azure AD выпустит маркер пользователя или доступа для приложения.                            **Примечания**: требуется версия 1,5 или более новая, не допускающая значение null.            |
|appRoles|аппроле|Роли приложения, предоставляемые связанным приложением. Дополнительные сведения см. в описании свойства **appRoles** для объекта Application **Notes**: требуется версия 1,5 или более новая, не допускающая значение null.            |
|displayName|Строка|Отображаемое имя для субъекта-службы.|
|errorUrl|String|            |
|homepage|String|URL-адрес домашней страницы связанного приложения.|
|keyCredentials|кэйкредентиал|Коллекция ключевых учетных данных, связанных с субъектом-службой.                            **Примечание.** Значение null не допускается.            |
|logoutUrl|String| Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML. |
|oauth2Permissions|oAuth2Permission|Разрешения OAuth 2.0, предоставляемые связанным приложением. Дополнительные сведения см. в определении свойства **oauth2Permissions** для объекта application.                            **Примечания**: требуется версия 1,5 или более новая, не допускающая значение null.            |
|passwordCredentials|пассвордкредентиал|Коллекция учетных данных паролей, связанных с субъектом-службой.                            **Примечание.** Значение null не допускается.            |
|preferredTokenSigningKeyThumbprint|String|Зарезервировано только для внутреннего использования. Не записывайте и не используйте иным образом это свойство. Может быть удалено в будущих версиях.                            **Примечания**: требуется версия 1,5 или более поздняя.            |
|publisherName|String|Отображаемое имя клиента, в котором указано связанное приложение.|
|replyUrls|String|URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения.                            **Примечание.** Значение null не допускается.            |
|samlMetadataUrl|String|            |
|ServicePrincipalNames|String|URI, определяющие связанное приложение. Дополнительные сведения см. в статье [Объекты приложения и субъекта-службы](https://msdn.microsoft.com/library/azure/dn132633.aspx).                            **Notes**: not Nullable, оператор **ANY** необходим для выражений фильтров в многозначных свойствах; Дополнительные сведения см в разделе [Поддерживаемые запросы, фильтры и параметры разбиения по страницам](https://msdn.microsoft.com/library/azure/dn727074.aspx).            |
|tags|String|                                        **Примечание.** Значение null не допускается.            |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
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
