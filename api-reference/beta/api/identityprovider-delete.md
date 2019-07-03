---
title: Удаление identityProvider
description: Удаление существующего объекта identityProvider.
localization_priority: Normal
ms.openlocfilehash: 74acf6b790ca9039944bc2d9bc687b74fced1d1b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442582"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="3a5b1-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="3a5b1-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a5b1-104">Удаление существующего объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="3a5b1-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3a5b1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a5b1-105">Permissions</span></span>

<span data-ttu-id="3a5b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a5b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a5b1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a5b1-108">Permission type</span></span>      | <span data-ttu-id="3a5b1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a5b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a5b1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a5b1-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3a5b1-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a5b1-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="3a5b1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a5b1-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3a5b1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a5b1-113">Not supported.</span></span>|
|<span data-ttu-id="3a5b1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a5b1-114">Application</span></span>|<span data-ttu-id="3a5b1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a5b1-115">Not supported.</span></span>|

<span data-ttu-id="3a5b1-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="3a5b1-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="3a5b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a5b1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3a5b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a5b1-118">Request headers</span></span>

|<span data-ttu-id="3a5b1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3a5b1-119">Name</span></span>|<span data-ttu-id="3a5b1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3a5b1-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3a5b1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a5b1-121">Authorization</span></span>|<span data-ttu-id="3a5b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a5b1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a5b1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a5b1-124">Request body</span></span>

<span data-ttu-id="3a5b1-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a5b1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a5b1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a5b1-126">Response</span></span>

<span data-ttu-id="3a5b1-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a5b1-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3a5b1-128">Пример</span><span class="sxs-lookup"><span data-stu-id="3a5b1-128">Example</span></span>

<span data-ttu-id="3a5b1-129">В приведенном ниже примере удаляется объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="3a5b1-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="3a5b1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a5b1-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3a5b1-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a5b1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3a5b1-132">C#</span><span class="sxs-lookup"><span data-stu-id="3a5b1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a5b1-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="3a5b1-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3a5b1-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3a5b1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3a5b1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a5b1-135">Response</span></span>

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
