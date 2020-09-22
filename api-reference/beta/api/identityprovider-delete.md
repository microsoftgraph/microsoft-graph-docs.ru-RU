---
title: Удаление identityProvider
description: Удаление identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 08e6208cbd58a3101d995d77e7d90b47918fbce5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001689"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="8ff6a-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="8ff6a-103">Delete identityProvider</span></span>

<span data-ttu-id="8ff6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ff6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff6a-105">Удаление [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="8ff6a-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ff6a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ff6a-106">Permissions</span></span>

<span data-ttu-id="8ff6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ff6a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ff6a-109">Permission type</span></span>      | <span data-ttu-id="8ff6a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ff6a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ff6a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ff6a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8ff6a-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff6a-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="8ff6a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ff6a-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8ff6a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ff6a-114">Not supported.</span></span>|
|<span data-ttu-id="8ff6a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ff6a-115">Application</span></span>|<span data-ttu-id="8ff6a-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff6a-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="8ff6a-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="8ff6a-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="8ff6a-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8ff6a-118">Global administrator</span></span>
* <span data-ttu-id="8ff6a-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="8ff6a-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8ff6a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ff6a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ff6a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ff6a-121">Request headers</span></span>

|<span data-ttu-id="8ff6a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8ff6a-122">Name</span></span>|<span data-ttu-id="8ff6a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8ff6a-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8ff6a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ff6a-124">Authorization</span></span>|<span data-ttu-id="8ff6a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ff6a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ff6a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ff6a-127">Request body</span></span>

<span data-ttu-id="8ff6a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ff6a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ff6a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ff6a-129">Response</span></span>

<span data-ttu-id="8ff6a-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8ff6a-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8ff6a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8ff6a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ff6a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ff6a-132">Request</span></span>

<span data-ttu-id="8ff6a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ff6a-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8ff6a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ff6a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="8ff6a-135">C#</span><span class="sxs-lookup"><span data-stu-id="8ff6a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ff6a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ff6a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ff6a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ff6a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8ff6a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ff6a-138">Response</span></span>

<span data-ttu-id="8ff6a-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8ff6a-139">The following is an example of the response.</span></span>

<span data-ttu-id="8ff6a-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8ff6a-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


