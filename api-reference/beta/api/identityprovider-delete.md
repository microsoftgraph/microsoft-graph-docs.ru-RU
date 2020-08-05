---
title: Удаление identityProvider
description: Удаление identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f138dd61b8674151fd3ac2ec7ddd1f340570e994
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566825"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="b6c20-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="b6c20-103">Delete identityProvider</span></span>

<span data-ttu-id="b6c20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6c20-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6c20-105">Удаление [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="b6c20-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6c20-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6c20-106">Permissions</span></span>

<span data-ttu-id="b6c20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6c20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6c20-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6c20-109">Permission type</span></span>      | <span data-ttu-id="b6c20-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6c20-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6c20-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6c20-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6c20-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c20-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b6c20-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6c20-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b6c20-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6c20-114">Not supported.</span></span>|
|<span data-ttu-id="b6c20-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6c20-115">Application</span></span>|<span data-ttu-id="b6c20-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c20-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="b6c20-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="b6c20-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="b6c20-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b6c20-118">Global administrator</span></span>
* <span data-ttu-id="b6c20-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="b6c20-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b6c20-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6c20-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b6c20-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6c20-121">Request headers</span></span>

|<span data-ttu-id="b6c20-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b6c20-122">Name</span></span>|<span data-ttu-id="b6c20-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b6c20-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b6c20-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6c20-124">Authorization</span></span>|<span data-ttu-id="b6c20-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6c20-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6c20-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6c20-127">Request body</span></span>

<span data-ttu-id="b6c20-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6c20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6c20-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6c20-129">Response</span></span>

<span data-ttu-id="b6c20-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6c20-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6c20-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b6c20-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6c20-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6c20-132">Request</span></span>

<span data-ttu-id="b6c20-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6c20-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b6c20-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6c20-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="b6c20-135">C#</span><span class="sxs-lookup"><span data-stu-id="b6c20-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6c20-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6c20-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6c20-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6c20-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b6c20-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6c20-138">Response</span></span>

<span data-ttu-id="b6c20-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b6c20-139">The following is an example of the response.</span></span>

<span data-ttu-id="b6c20-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b6c20-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
