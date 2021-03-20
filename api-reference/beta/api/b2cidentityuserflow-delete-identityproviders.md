---
title: Удаление identityProvider из b2cIdentityUserFlow
description: Удаление identityProvider из b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 290a2e7597f0211bf4aefbda70273efb5003aa69
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944893"
---
# <a name="delete-an-identityprovider-from-a-b2cidentityuserflow"></a><span data-ttu-id="1f540-103">Удаление identityProvider из b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="1f540-103">Delete an identityProvider from a b2cIdentityUserFlow</span></span>

<span data-ttu-id="1f540-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f540-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f540-105">Удаление поставщика удостоверений из [объекта b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="1f540-105">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="1f540-106">Дополнительные сведения о поставщиках удостоверений, доступных для потоков пользователей, см. в справке об API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="1f540-106">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f540-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f540-107">Permissions</span></span>

<span data-ttu-id="1f540-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f540-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f540-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f540-110">Permission type</span></span>      | <span data-ttu-id="1f540-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f540-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f540-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f540-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f540-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f540-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1f540-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f540-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1f540-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f540-115">Not supported.</span></span>|
|<span data-ttu-id="1f540-116">Application</span><span class="sxs-lookup"><span data-stu-id="1f540-116">Application</span></span>| <span data-ttu-id="1f540-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f540-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="1f540-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="1f540-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1f540-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1f540-119">Global administrator</span></span>
* <span data-ttu-id="1f540-120">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="1f540-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1f540-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f540-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1f540-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f540-122">Request headers</span></span>

|<span data-ttu-id="1f540-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1f540-123">Name</span></span>|<span data-ttu-id="1f540-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1f540-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1f540-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f540-125">Authorization</span></span>|<span data-ttu-id="1f540-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f540-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f540-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f540-128">Request body</span></span>

<span data-ttu-id="1f540-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f540-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f540-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f540-130">Response</span></span>

<span data-ttu-id="1f540-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1f540-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="1f540-132">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="1f540-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="1f540-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1f540-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f540-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f540-134">Request</span></span>

<span data-ttu-id="1f540-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f540-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1f540-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f540-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_1"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="1f540-137">C#</span><span class="sxs-lookup"><span data-stu-id="1f540-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f540-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f540-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f540-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f540-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f540-140">Java</span><span class="sxs-lookup"><span data-stu-id="1f540-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-identityproviders-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f540-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f540-141">Response</span></span>

<span data-ttu-id="1f540-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1f540-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


