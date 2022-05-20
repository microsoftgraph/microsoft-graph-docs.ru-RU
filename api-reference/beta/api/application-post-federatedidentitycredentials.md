---
title: Создание federatedIdentityCredential
description: Создайте объект federatedIdentityCredential для приложения.
author: shahzad-khalid
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: b110f00734c7d7ad2044f289917713ad5d19887a
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602702"
---
# <a name="create-federatedidentitycredential"></a>Создание federatedIdentityCredential
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [federatedIdentityCredential](../resources/federatedidentitycredential.md) для приложения. Настроив отношение доверия между регистрацией приложения Azure AD и поставщиком удостоверений для вычислительной платформы, вы можете использовать маркеры, выданные этой платформой, для проверки подлинности с помощью платформа удостоверений Майкрософт и вызова API в экосистеме Майкрософт.[](/azure/active-directory/develop/workload-identity-federation-create-trust) В приложение можно добавить не более 20 объектов.

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
POST /applications/{applicationsId}/federatedIdentityCredentials
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [federatedIdentityCredential](../resources/federatedidentitycredential.md) в формате JSON.

В следующей таблице показаны свойства, необходимые при создании [federatedIdentityCredential](../resources/federatedidentitycredential.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|Аудитории|Коллекция строк|Список аудиторий, которые могут отображаться во внешнем маркере. Это поле является обязательным и по умолчанию имеет значение "api://AzureADTokenExchange". В нем указано, платформа удостоверений Майкрософт должны приниматься в утверждении `aud` во входящем токене. Это значение Azure AD во внешнем поставщике удостоверений и не имеет фиксированного значения для поставщиков удостоверений. Возможно, потребуется создать регистрацию приложения в поставщике удостоверений, чтобы выступать в качестве аудитории этого маркера. Обязательный аргумент.|
|Эмитента|Строка|TThe URL-адрес внешнего поставщика удостоверений и должен соответствовать утверждению издателя внешнего маркера для обмена. Сочетание значений издателя и субъекта **должно быть уникальным** в приложении. Обязательный аргумент.|
|name|String|Уникальный идентификатор для учетных данных федеративного удостоверения, который имеет ограничение в 120 символов и должен быть понятным по URL-адресу. После создания она неизменяема|
|subject|String|Обязательный. Идентификатор рабочей нагрузки внешнего программного обеспечения во внешнем поставщике удостоверений. Как и значение аудитории, он не имеет фиксированного формата, так как каждый поставщик удостоверений использует собственный идентификатор GUID, иногда идентификатор с разделителями двоеточия, иногда произвольные строки. Здесь значение должно совпадать с вложенным утверждением в токене, представленном Azure AD. Сочетание **издателя и субъекта** **должно** быть уникальным в приложении.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [federatedIdentityCredential](../resources/federatedidentitycredential.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_federatedidentitycredential_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/bcd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/
Content-Type: application/json

{
    "name": "testing02",
    "issuer": "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
    "subject": "a7d388c3-5e3f-4959-ac7d-786b3383006a",
    "audiences": [
        "api://AzureADTokenExchange"
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-federatedidentitycredential-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-federatedidentitycredential-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-federatedidentitycredential-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-federatedidentitycredential-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-federatedidentitycredential-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-federatedidentitycredential-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.federatedIdentityCredential"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications('bcd7c908-1c4d-4d48-93ee-ff38349a75c8')/federatedIdentityCredentials/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/directoryObjects/$/Microsoft.DirectoryServices.Application('bcd7c908-1c4d-4d48-93ee-ff38349a75c8')/federatedIdentityCredentials/d9b7bf1e-429e-4678-8132-9b00c9846cc4",
    "id": "d9b7bf1e-429e-4678-8132-9b00c9846cc4",
    "name": "testing02",
    "issuer": "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
    "subject": "a7d388c3-5e3f-4959-ac7d-786b3383006a",
    "description": null,
    "audiences": [
        "api://AzureADTokenExchange"
    ]
}
```

