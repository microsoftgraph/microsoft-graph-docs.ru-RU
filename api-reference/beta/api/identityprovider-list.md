---
title: Перечисление объектов identityProvider
description: Получение всех объектов identityProvider в каталоге.
localization_priority: Normal
doc_type: apiPageType
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a2c6279a6d5c3511d6b6786f3d561d0632933e66
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199552"
---
# <a name="list-identityproviders"></a><span data-ttu-id="b3292-103">Перечисление объектов identityProvider</span><span class="sxs-lookup"><span data-stu-id="b3292-103">List identityProviders</span></span>

<span data-ttu-id="b3292-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3292-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3292-105">Получение всех объектов [identityProvider](../resources/identityprovider.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="b3292-105">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3292-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3292-106">Permissions</span></span>

<span data-ttu-id="b3292-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3292-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3292-109">Permission type</span></span>      | <span data-ttu-id="b3292-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3292-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3292-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3292-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3292-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3292-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b3292-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3292-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b3292-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3292-114">Not supported.</span></span>|
|<span data-ttu-id="b3292-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3292-115">Application</span></span>|<span data-ttu-id="b3292-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3292-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="b3292-117">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="b3292-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="b3292-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3292-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="b3292-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3292-119">Request headers</span></span>

|<span data-ttu-id="b3292-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b3292-120">Name</span></span>|<span data-ttu-id="b3292-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b3292-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b3292-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3292-122">Authorization</span></span>|<span data-ttu-id="b3292-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3292-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3292-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3292-125">Request body</span></span>

<span data-ttu-id="b3292-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3292-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3292-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3292-127">Response</span></span>

<span data-ttu-id="b3292-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [identityProvider](../resources/identityprovider.md) в формате JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3292-128">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3292-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b3292-129">Example</span></span>

<span data-ttu-id="b3292-130">В приведенном ниже примере возвращаются все объекты **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="b3292-130">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="b3292-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3292-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b3292-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3292-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="b3292-133">C#</span><span class="sxs-lookup"><span data-stu-id="b3292-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3292-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3292-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3292-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3292-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b3292-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3292-136">Response</span></span>

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
