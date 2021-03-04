---
title: Удаление identityProvider
description: Удаление identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: f09503674cf3f340ef6b7ebe7a918c7c061368c9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435492"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="fe96f-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="fe96f-103">Delete identityProvider</span></span>

<span data-ttu-id="fe96f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe96f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe96f-105">Удаление [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="fe96f-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe96f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe96f-106">Permissions</span></span>

<span data-ttu-id="fe96f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe96f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe96f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe96f-109">Permission type</span></span>      | <span data-ttu-id="fe96f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe96f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe96f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe96f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe96f-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe96f-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="fe96f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe96f-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fe96f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe96f-114">Not supported.</span></span>|
|<span data-ttu-id="fe96f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="fe96f-115">Application</span></span>|<span data-ttu-id="fe96f-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe96f-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="fe96f-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="fe96f-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="fe96f-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="fe96f-118">Global administrator</span></span>
* <span data-ttu-id="fe96f-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="fe96f-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fe96f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe96f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fe96f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe96f-121">Request headers</span></span>

|<span data-ttu-id="fe96f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fe96f-122">Name</span></span>|<span data-ttu-id="fe96f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fe96f-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fe96f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe96f-124">Authorization</span></span>|<span data-ttu-id="fe96f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe96f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe96f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe96f-127">Request body</span></span>

<span data-ttu-id="fe96f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe96f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe96f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe96f-129">Response</span></span>

<span data-ttu-id="fe96f-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fe96f-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fe96f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fe96f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe96f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe96f-132">Request</span></span>

<span data-ttu-id="fe96f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe96f-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fe96f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe96f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="fe96f-135">C#</span><span class="sxs-lookup"><span data-stu-id="fe96f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe96f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe96f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe96f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe96f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe96f-138">Java</span><span class="sxs-lookup"><span data-stu-id="fe96f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fe96f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe96f-139">Response</span></span>

<span data-ttu-id="fe96f-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fe96f-140">The following is an example of the response.</span></span>

<span data-ttu-id="fe96f-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fe96f-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


