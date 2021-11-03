---
title: Обновление federatedIdentityCredential
description: Обновление свойств объекта federatedIdentityCredential.
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: d6be2a72ae63db2800d822274725d7b51a80143e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694777"
---
# <a name="update-federatedidentitycredential"></a>Обновление federatedIdentityCredential
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [federatedIdentityCredential.](../resources/federatedidentitycredential.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) |  Application.ReadWrite.All |
|Приложение | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |


## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /applications/{applicationsId}/federatedIdentityCredentials/{federatedIdentityCredentialId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

Укажите в тексте запроса *только* значения обновляемых свойств. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.

В следующей таблице указаны свойства, которые можно обновить.

|Свойство|Тип|Описание|
|:---|:---|:---|
|аудитории|Коллекция строк|Список аудиторий, которые могут отображаться в выданных маркерах. Рекомендуемое значение `api://AzureADTokenExchange` . |
|description|String|Предоставленное пользователем описание того, для чего используется federatedIdentityCredential. |
|эмитент|String|URL-адрес входящих доверенных эмитентов (Secure Token Service). Соответствует утверждению эмитента о маркере доступа. Например, в сценарии "Управляемые ключи клиента" Azure AD является эмитентом и допустимым значением будет `https://login.microsoftonline.com/{tenantid}/v2.0` . Сочетание значений эмитента **и** субъекта должно **быть** уникальным в приложении. |
|subject|String|<li>Для эмитента Azure AD службаPrincipal (может представлять управляемый идентификатор), которая может `objectId` олицетворять приложение. Объект, связанный с этим GUID, должен существовать в клиенте.</li><li>Для всех остальных эмитентов строка без дополнительной проверки</ul><br><br>Сочетание значений эмитента **и** субъекта должно **быть** уникальным в приложении.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_federatedidentitycredential"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/bcd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/15be77d1-1940-43fe-8aae-94a78e078da0
Content-Type: application/json

{
    "name": "testing02",
    "issuer": "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
    "subject": "a7d388c3-5e3f-4959-ac7d-786b3383006a",
    "description": "Updated description",
    "audiences": [
        "api://AzureADTokenExchange"
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-federatedidentitycredential-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-federatedidentitycredential-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-federatedidentitycredential-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-federatedidentitycredential-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content

```

