---
title: Удаление identityProvider
description: Удаление существующего объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 0a7bdf4083ca02dfd8a2a92e2318884a2ae132e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953229"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="f1531-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="f1531-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1531-104">Удаление существующего объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="f1531-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1531-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1531-105">Permissions</span></span>

<span data-ttu-id="f1531-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1531-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1531-108">Permission type</span></span>      | <span data-ttu-id="f1531-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1531-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1531-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1531-110">Delegated (work or school account)</span></span>|<span data-ttu-id="f1531-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1531-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="f1531-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1531-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f1531-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1531-113">Not supported.</span></span>|
|<span data-ttu-id="f1531-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1531-114">Application</span></span>|<span data-ttu-id="f1531-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1531-115">Not supported.</span></span>|

<span data-ttu-id="f1531-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="f1531-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f1531-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1531-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f1531-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1531-118">Request headers</span></span>

|<span data-ttu-id="f1531-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f1531-119">Name</span></span>|<span data-ttu-id="f1531-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f1531-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f1531-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1531-121">Authorization</span></span>|<span data-ttu-id="f1531-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1531-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1531-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1531-124">Request body</span></span>

<span data-ttu-id="f1531-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1531-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1531-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1531-126">Response</span></span>

<span data-ttu-id="f1531-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1531-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1531-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f1531-128">Example</span></span>

<span data-ttu-id="f1531-129">В приведенном ниже примере удаляется объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="f1531-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="f1531-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1531-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f1531-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1531-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f1531-132">C#</span><span class="sxs-lookup"><span data-stu-id="f1531-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1531-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="f1531-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f1531-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f1531-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f1531-135">Java</span><span class="sxs-lookup"><span data-stu-id="f1531-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f1531-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1531-136">Response</span></span>

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
