---
title: Получение identityProvider
description: Получение свойств существующего identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 670c745966f3fecfbbe837e0d8c176d67a436a45
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199617"
---
# <a name="get-identityprovider"></a><span data-ttu-id="e8fd1-103">Получение identityProvider</span><span class="sxs-lookup"><span data-stu-id="e8fd1-103">Get identityProvider</span></span>

<span data-ttu-id="e8fd1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8fd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8fd1-105">Получение свойств существующего объекта [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="e8fd1-105">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8fd1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8fd1-106">Permissions</span></span>

<span data-ttu-id="e8fd1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8fd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8fd1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8fd1-109">Permission type</span></span>      | <span data-ttu-id="e8fd1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8fd1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8fd1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8fd1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8fd1-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8fd1-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e8fd1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8fd1-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e8fd1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8fd1-114">Not supported.</span></span>|
|<span data-ttu-id="e8fd1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8fd1-115">Application</span></span>|<span data-ttu-id="e8fd1-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8fd1-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="e8fd1-117">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="e8fd1-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e8fd1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8fd1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8fd1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8fd1-119">Request headers</span></span>

|<span data-ttu-id="e8fd1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e8fd1-120">Name</span></span>|<span data-ttu-id="e8fd1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e8fd1-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e8fd1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8fd1-122">Authorization</span></span>|<span data-ttu-id="e8fd1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8fd1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8fd1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8fd1-125">Request body</span></span>

<span data-ttu-id="e8fd1-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8fd1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8fd1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8fd1-127">Response</span></span>

<span data-ttu-id="e8fd1-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и представление объекта [identityProvider](../resources/identityprovider.md) в формате JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8fd1-128">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8fd1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e8fd1-129">Example</span></span>

<span data-ttu-id="e8fd1-130">В приведенном ниже примере возвращается определенный объект **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="e8fd1-130">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e8fd1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8fd1-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e8fd1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8fd1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```
# <a name="c"></a>[<span data-ttu-id="e8fd1-133">C#</span><span class="sxs-lookup"><span data-stu-id="e8fd1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8fd1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8fd1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8fd1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8fd1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e8fd1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8fd1-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
