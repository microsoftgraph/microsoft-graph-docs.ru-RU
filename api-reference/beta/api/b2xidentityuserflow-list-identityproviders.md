---
title: Список всех identityProviders в b2xIdentityUserFlow
description: Список всех identityProviders в b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: d1589c5ec3267bcfe51de38540bb9ef83efeee78
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438108"
---
# <a name="list-all-identityproviders-in-a-b2xidentityuserflow"></a><span data-ttu-id="f2873-103">Список всех identityProviders в b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="f2873-103">List all identityProviders in a b2xIdentityUserFlow</span></span>

<span data-ttu-id="f2873-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2873-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2873-105">Получите поставщиков удостоверений в [объекте b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="f2873-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2873-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2873-106">Permissions</span></span>

<span data-ttu-id="f2873-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2873-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2873-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2873-109">Permission type</span></span>      | <span data-ttu-id="f2873-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2873-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2873-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2873-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2873-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2873-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f2873-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2873-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f2873-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2873-114">Not supported.</span></span>|
|<span data-ttu-id="f2873-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f2873-115">Application</span></span>| <span data-ttu-id="f2873-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2873-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f2873-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="f2873-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f2873-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f2873-118">Global administrator</span></span>
* <span data-ttu-id="f2873-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="f2873-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f2873-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2873-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="f2873-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2873-121">Request headers</span></span>

|<span data-ttu-id="f2873-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f2873-122">Name</span></span>|<span data-ttu-id="f2873-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f2873-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f2873-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2873-124">Authorization</span></span>|<span data-ttu-id="f2873-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2873-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2873-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2873-127">Request body</span></span>

<span data-ttu-id="f2873-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2873-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2873-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2873-129">Response</span></span>

<span data-ttu-id="f2873-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityprovider.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f2873-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2873-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f2873-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2873-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2873-132">Request</span></span>

<span data-ttu-id="f2873-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2873-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2873-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2873-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="f2873-135">C#</span><span class="sxs-lookup"><span data-stu-id="f2873-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2873-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2873-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2873-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2873-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2873-138">Java</span><span class="sxs-lookup"><span data-stu-id="f2873-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2873-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2873-139">Response</span></span>

<span data-ttu-id="f2873-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f2873-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "*****"
        },
        {
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}
```


