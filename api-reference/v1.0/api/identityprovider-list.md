---
title: Перечисление объектов identityProvider
description: Получение всех объектов identityProvider
localization_priority: Priority
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fdc7e4323fa096d40d757426fd064179921c1ebc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441846"
---
# <a name="list-identityproviders"></a><span data-ttu-id="eab01-103">Перечисление объектов identityProvider</span><span class="sxs-lookup"><span data-stu-id="eab01-103">List identityProviders</span></span>

<span data-ttu-id="eab01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eab01-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eab01-105">Получение всех объектов [identityProvider](../resources/identityprovider.md) в каталоге.</span><span class="sxs-lookup"><span data-stu-id="eab01-105">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="eab01-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eab01-106">Permissions</span></span>

<span data-ttu-id="eab01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eab01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eab01-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eab01-109">Permission type</span></span>      | <span data-ttu-id="eab01-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eab01-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eab01-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eab01-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eab01-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eab01-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="eab01-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eab01-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="eab01-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eab01-114">Not supported.</span></span>|
|<span data-ttu-id="eab01-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eab01-115">Application</span></span>|<span data-ttu-id="eab01-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eab01-116">Not supported.</span></span>|

<span data-ttu-id="eab01-117">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="eab01-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="eab01-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eab01-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="eab01-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eab01-119">Request headers</span></span>

|<span data-ttu-id="eab01-120">Имя</span><span class="sxs-lookup"><span data-stu-id="eab01-120">Name</span></span>|<span data-ttu-id="eab01-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eab01-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="eab01-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eab01-122">Authorization</span></span>|<span data-ttu-id="eab01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eab01-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eab01-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eab01-125">Request body</span></span>

<span data-ttu-id="eab01-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eab01-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eab01-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="eab01-127">Response</span></span>

<span data-ttu-id="eab01-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [identityProvider](../resources/identityprovider.md) в формате JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eab01-128">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eab01-129">Пример</span><span class="sxs-lookup"><span data-stu-id="eab01-129">Example</span></span>

<span data-ttu-id="eab01-130">В приведенном ниже примере возвращаются все объекты **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="eab01-130">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="eab01-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eab01-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eab01-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="eab01-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list-identityproviders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="eab01-133">C#</span><span class="sxs-lookup"><span data-stu-id="eab01-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eab01-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eab01-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eab01-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eab01-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eab01-136">Java</span><span class="sxs-lookup"><span data-stu-id="eab01-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eab01-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="eab01-137">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

