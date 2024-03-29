---
title: Обновление federatedIdentityCredential
description: Обновление свойств объекта federatedIdentityCredential.
author: shahzad-khalid
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 11ee8eb14f13398dcf322b1f2553f076e3db9038
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602758"
---
# <a name="update-federatedidentitycredential"></a>Обновление federatedIdentityCredential
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [federatedIdentityCredential](../resources/federatedidentitycredential.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) |  Application.ReadWrite.All |
|Для приложений | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |


## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /applications/{applicationId}/federatedIdentityCredentials/{federatedIdentityCredentialId}

PATCH /applications/{applicationId}/federatedIdentityCredentials/{federatedIdentityCredentialName}
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
|Аудитории|Коллекция строк|Список аудиторий, которые могут отображаться в выданных маркерах. Рекомендуемое значение — `api://AzureADTokenExchange`. |
|description|Строка|Предоставленное пользователем описание того, для чего используется federatedIdentityCredential. |
|Эмитента|Строка|URL-адрес входящего доверенного издателя (служба маркеров безопасности). Соответствует утверждению издателя маркера доступа. Например, в сценарии с управляемыми клиентом ключами Azure AD издателем и допустимым значением `https://login.microsoftonline.com/{tenantid}/v2.0`будет . Сочетание значений издателя и субъекта **должно быть уникальным** в приложении. |
|subject|String|<li>Для Azure AD издателя servicePrincipal `objectId` (может представлять управляемое удостоверение), которое может олицетворять приложение. Объект, связанный с этим GUID, должен существовать в клиенте.</li><li>Для всех остальных издателей строка без дополнительной проверки</ul><br><br>Сочетание значений издателя и субъекта **должно быть уникальным** в приложении.|



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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-federatedidentitycredential-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-federatedidentitycredential-powershell-snippets.md)]
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

