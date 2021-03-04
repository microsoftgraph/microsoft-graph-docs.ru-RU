---
title: Список всех identityProviders в b2cIdentityUserFlow
description: Список всех identityProviders в b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: e908159c657016f7b36d1886e3d3b501503b295b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438316"
---
# <a name="list-all-identityproviders-in-a-b2cidentityuserflow"></a><span data-ttu-id="3e825-103">Список всех identityProviders в b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3e825-103">List all identityProviders in a b2cIdentityUserFlow</span></span>

<span data-ttu-id="3e825-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e825-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e825-105">Получите поставщиков удостоверений в [объекте b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="3e825-105">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e825-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e825-106">Permissions</span></span>

<span data-ttu-id="3e825-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e825-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e825-109">Permission type</span></span>      | <span data-ttu-id="3e825-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e825-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e825-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e825-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e825-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e825-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3e825-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e825-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3e825-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e825-114">Not supported.</span></span>|
|<span data-ttu-id="3e825-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3e825-115">Application</span></span>| <span data-ttu-id="3e825-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e825-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3e825-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="3e825-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3e825-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="3e825-118">Global administrator</span></span>
* <span data-ttu-id="3e825-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="3e825-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3e825-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e825-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /b2cUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="3e825-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e825-121">Request headers</span></span>

|<span data-ttu-id="3e825-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3e825-122">Name</span></span>|<span data-ttu-id="3e825-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3e825-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3e825-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e825-124">Authorization</span></span>|<span data-ttu-id="3e825-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e825-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e825-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e825-127">Request body</span></span>

<span data-ttu-id="3e825-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e825-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e825-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e825-129">Response</span></span>

<span data-ttu-id="3e825-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityprovider.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3e825-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e825-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3e825-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e825-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e825-132">Request</span></span>

<span data-ttu-id="3e825-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e825-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3e825-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e825-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="3e825-135">C#</span><span class="sxs-lookup"><span data-stu-id="3e825-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e825-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e825-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e825-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e825-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e825-138">Java</span><span class="sxs-lookup"><span data-stu-id="3e825-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e825-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e825-139">Response</span></span>

<span data-ttu-id="3e825-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3e825-140">The following is an example of the response.</span></span>

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


