---
title: Перечисление объектов identityProvider
description: Получение всех объектов identityProvider в каталоге.
localization_priority: Normal
ms.openlocfilehash: 8af8806c2d932bbaa488252dbf5a665640ac4c6a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442239"
---
# <a name="list-identityproviders"></a><span data-ttu-id="52df8-103">Перечисление объектов identityProvider</span><span class="sxs-lookup"><span data-stu-id="52df8-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52df8-104">Получение всех объектов [identityProvider](../resources/identityprovider.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="52df8-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="52df8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52df8-105">Permissions</span></span>

<span data-ttu-id="52df8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52df8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52df8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52df8-108">Permission type</span></span>      | <span data-ttu-id="52df8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52df8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52df8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52df8-110">Delegated (work or school account)</span></span>|<span data-ttu-id="52df8-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52df8-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="52df8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52df8-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="52df8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52df8-113">Not supported.</span></span>|
|<span data-ttu-id="52df8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52df8-114">Application</span></span>|<span data-ttu-id="52df8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52df8-115">Not supported.</span></span>|

<span data-ttu-id="52df8-116">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="52df8-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="52df8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52df8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="52df8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52df8-118">Request headers</span></span>

|<span data-ttu-id="52df8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="52df8-119">Name</span></span>|<span data-ttu-id="52df8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="52df8-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="52df8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52df8-121">Authorization</span></span>|<span data-ttu-id="52df8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52df8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52df8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52df8-124">Request body</span></span>

<span data-ttu-id="52df8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52df8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52df8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="52df8-126">Response</span></span>

<span data-ttu-id="52df8-127">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [identityProvider](../resources/identityprovider.md) в формате JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52df8-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52df8-128">Пример</span><span class="sxs-lookup"><span data-stu-id="52df8-128">Example</span></span>

<span data-ttu-id="52df8-129">В приведенном ниже примере возвращаются все объекты **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="52df8-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="52df8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="52df8-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="52df8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="52df8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="52df8-132">C#</span><span class="sxs-lookup"><span data-stu-id="52df8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52df8-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="52df8-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52df8-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="52df8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="52df8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="52df8-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
