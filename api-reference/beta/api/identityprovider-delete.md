---
title: Удаление identityProvider
description: Удаление существующего объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d63e828ac78ce376c78a484402f44e7584bc331
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446508"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="3e4f8-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="3e4f8-103">Delete identityProvider</span></span>

<span data-ttu-id="3e4f8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3e4f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e4f8-105">Удаление существующего объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="3e4f8-105">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e4f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e4f8-106">Permissions</span></span>

<span data-ttu-id="3e4f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e4f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e4f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e4f8-109">Permission type</span></span>      | <span data-ttu-id="3e4f8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e4f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e4f8-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e4f8-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="3e4f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e4f8-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3e4f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-114">Not supported.</span></span>|
|<span data-ttu-id="3e4f8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e4f8-115">Application</span></span>|<span data-ttu-id="3e4f8-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e4f8-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="3e4f8-117">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="3e4f8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e4f8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3e4f8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e4f8-119">Request headers</span></span>

|<span data-ttu-id="3e4f8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3e4f8-120">Name</span></span>|<span data-ttu-id="3e4f8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3e4f8-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3e4f8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e4f8-122">Authorization</span></span>|<span data-ttu-id="3e4f8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e4f8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e4f8-125">Request body</span></span>

<span data-ttu-id="3e4f8-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e4f8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e4f8-127">Response</span></span>

<span data-ttu-id="3e4f8-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3e4f8-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3e4f8-129">Example</span></span>

<span data-ttu-id="3e4f8-130">В приведенном ниже примере удаляется объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="3e4f8-130">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="3e4f8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e4f8-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3e4f8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e4f8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="c"></a>[<span data-ttu-id="3e4f8-133">C#</span><span class="sxs-lookup"><span data-stu-id="3e4f8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e4f8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e4f8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e4f8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e4f8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3e4f8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e4f8-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
