---
title: Создание federatedIdentityCredential
description: Создайте новый объект federatedIdentityCredential для приложения.
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 09c06d30a39755b7b0d04fba29352d4f4a94da64
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097280"
---
# <a name="create-federatedidentitycredential"></a>Создание federatedIdentityCredential
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект federatedIdentityCredential](../resources/federatedidentitycredential.md) для приложения. Настроив доверительные отношения между регистрацией приложений Azure AD и поставщиком удостоверений для компьютерной платформы, вы можете использовать маркеры, выданные этой платформой, для проверки подлинности с помощью платформа удостоверений Майкрософт и вызова API в экосистеме Майкрософт. [](/azure/active-directory/develop/workload-identity-federation-create-trust) В приложение можно добавить не более 20 объектов.

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
POST /applications/{applicationsId}/federatedIdentityCredentials
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [federatedIdentityCredential.](../resources/federatedidentitycredential.md)

В следующей таблице показаны свойства, необходимые при создании [federatedIdentityCredential.](../resources/federatedidentitycredential.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|аудитории|Коллекция строк|Списки аудиторий, которые могут отображаться во внешнем маркере. Это поле является обязательным и по умолчанию "api://AzureADTokenExchange". В нем платформа удостоверений Майкрософт, что следует принять в `aud` утверждении в входящих маркерах. Это значение представляет Azure AD во внешнем поставщике удостоверений и не имеет фиксированного значения для поставщиков удостоверений , возможно, потребуется создать новую регистрацию приложений в поставщике удостоверений, чтобы служить аудиторией этого маркера. Обязательный.|
|эмитент|String|TThe URL-адрес внешнего поставщика удостоверений и должен соответствовать утверждению эмитента об обмене внешнего маркера. Сочетание значений эмитента **и** субъекта должно **быть** уникальным в приложении. Обязательный.|
|name|String|Уникальный идентификатор для учетных данных федерательных удостоверений, который имеет ограничение символов в 120 символов и должен быть удобным URL-адресом. Это неуменяемо после создания|
|subject|String|Обязательный. Идентификатор рабочей нагрузки внешнего программного обеспечения во внешнем поставщике удостоверений. Как и значение аудитории, он не имеет фиксированного формата, так как каждый поставщик удостоверений использует свои собственные — иногда GUID, иногда идентификатор двоеточия, иногда произвольные строки. Значение здесь должно соответствовать утверждению sub в маркере, представленном Azure AD. Сочетание **эмитента и** **субъекта должно** быть уникальным в приложении.|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект federatedIdentityCredential](../resources/federatedidentitycredential.md) в тексте ответа.

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

