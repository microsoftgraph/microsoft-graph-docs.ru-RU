---
title: Удаление identityProvider
description: Удаление существующего объекта identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1917a0d799e170636afb521ffecf4c024e431c9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002715"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="4a9d9-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="4a9d9-103">Delete identityProvider</span></span>

<span data-ttu-id="4a9d9-104">Удаление существующего объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="4a9d9-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a9d9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a9d9-105">Permissions</span></span>

<span data-ttu-id="4a9d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a9d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a9d9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a9d9-108">Permission type</span></span>      | <span data-ttu-id="4a9d9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a9d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a9d9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a9d9-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4a9d9-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a9d9-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="4a9d9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a9d9-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4a9d9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a9d9-113">Not supported.</span></span>|
|<span data-ttu-id="4a9d9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a9d9-114">Application</span></span>|<span data-ttu-id="4a9d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a9d9-115">Not supported.</span></span>|

<span data-ttu-id="4a9d9-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="4a9d9-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="4a9d9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a9d9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a9d9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a9d9-118">Request headers</span></span>

|<span data-ttu-id="4a9d9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4a9d9-119">Name</span></span>|<span data-ttu-id="4a9d9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4a9d9-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4a9d9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a9d9-121">Authorization</span></span>|<span data-ttu-id="4a9d9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a9d9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a9d9-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a9d9-124">Request body</span></span>

<span data-ttu-id="4a9d9-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a9d9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a9d9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a9d9-126">Response</span></span>

<span data-ttu-id="4a9d9-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4a9d9-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4a9d9-128">Пример</span><span class="sxs-lookup"><span data-stu-id="4a9d9-128">Example</span></span>

<span data-ttu-id="4a9d9-129">В приведенном ниже примере удаляется объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="4a9d9-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="4a9d9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a9d9-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4a9d9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a9d9-131">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a9d9-132">C#</span><span class="sxs-lookup"><span data-stu-id="4a9d9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a9d9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a9d9-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a9d9-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a9d9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4a9d9-135">Java</span><span class="sxs-lookup"><span data-stu-id="4a9d9-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4a9d9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a9d9-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
