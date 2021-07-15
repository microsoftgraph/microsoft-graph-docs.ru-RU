---
title: Список всех identityProviders в b2xIdentityUserFlow (обесценив)
description: Список всех identityProviders в b2xIdentityUserFlow (обесценив).
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 7b92da67e8969ffb54fe6a65469f6bd428d6e240
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439632"
---
# <a name="list-all-identityproviders-in-a-b2xidentityuserflow-deprecated"></a><span data-ttu-id="a4ee7-103">Список всех identityProviders в b2xIdentityUserFlow (обесценив)</span><span class="sxs-lookup"><span data-stu-id="a4ee7-103">List all identityProviders in a b2xIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="a4ee7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4ee7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="a4ee7-105">Получите поставщиков удостоверений в [объекте b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="a4ee7-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4ee7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4ee7-106">Permissions</span></span>

<span data-ttu-id="a4ee7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4ee7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4ee7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4ee7-109">Permission type</span></span>      | <span data-ttu-id="a4ee7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4ee7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4ee7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4ee7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4ee7-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4ee7-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a4ee7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4ee7-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a4ee7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4ee7-114">Not supported.</span></span>|
|<span data-ttu-id="a4ee7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4ee7-115">Application</span></span>| <span data-ttu-id="a4ee7-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4ee7-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="a4ee7-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="a4ee7-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a4ee7-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a4ee7-118">Global administrator</span></span>
* <span data-ttu-id="a4ee7-119">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="a4ee7-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a4ee7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4ee7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="a4ee7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4ee7-121">Request headers</span></span>

|<span data-ttu-id="a4ee7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a4ee7-122">Name</span></span>|<span data-ttu-id="a4ee7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ee7-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a4ee7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4ee7-124">Authorization</span></span>|<span data-ttu-id="a4ee7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4ee7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4ee7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4ee7-127">Request body</span></span>

<span data-ttu-id="a4ee7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4ee7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4ee7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4ee7-129">Response</span></span>

<span data-ttu-id="a4ee7-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` представление JSON [идентификаторовProviders](../resources/identityprovider.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a4ee7-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4ee7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a4ee7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4ee7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4ee7-132">Request</span></span>

<span data-ttu-id="a4ee7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4ee7-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a4ee7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4ee7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="a4ee7-135">C#</span><span class="sxs-lookup"><span data-stu-id="a4ee7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflow-list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4ee7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4ee7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflow-list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4ee7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4ee7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflow-list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4ee7-138">Java</span><span class="sxs-lookup"><span data-stu-id="a4ee7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflow-list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a4ee7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4ee7-139">Response</span></span>

<span data-ttu-id="a4ee7-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a4ee7-140">The following is an example of the response.</span></span>

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
