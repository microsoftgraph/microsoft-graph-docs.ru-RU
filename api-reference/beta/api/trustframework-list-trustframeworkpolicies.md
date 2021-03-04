---
title: Список trustFrameworkPolicies
description: В этой операции перечислены все объекты trustFrameworkPolicy в клиенте Azure AD B2C.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 872c26dd3b129fd47bb779ee3c10faf1419670af
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443316"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="e6a16-103">Список trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="e6a16-103">List trustFrameworkPolicies</span></span>

<span data-ttu-id="e6a16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6a16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6a16-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6a16-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6a16-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a16-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6a16-107">Извлечение списка [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) в клиенте или каталоге.</span><span class="sxs-lookup"><span data-stu-id="e6a16-107">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6a16-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6a16-108">Permissions</span></span>

<span data-ttu-id="e6a16-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6a16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6a16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6a16-111">Permission type</span></span>      | <span data-ttu-id="e6a16-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6a16-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6a16-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6a16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6a16-114">Policy.Read.All, Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="e6a16-114">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="e6a16-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6a16-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e6a16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a16-116">Not supported.</span></span>|
|<span data-ttu-id="e6a16-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e6a16-117">Application</span></span>|<span data-ttu-id="e6a16-118">Policy.Read.All, Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="e6a16-118">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="e6a16-119">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="e6a16-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e6a16-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6a16-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6a16-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6a16-121">Optional query parameters</span></span>

<span data-ttu-id="e6a16-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e6a16-122">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6a16-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6a16-123">Request headers</span></span>

|<span data-ttu-id="e6a16-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e6a16-124">Name</span></span>|<span data-ttu-id="e6a16-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e6a16-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e6a16-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6a16-126">Authorization</span></span>|<span data-ttu-id="e6a16-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6a16-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6a16-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6a16-129">Request body</span></span>

<span data-ttu-id="e6a16-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6a16-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6a16-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6a16-131">Response</span></span>

<span data-ttu-id="e6a16-132">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) в представлении JSON в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e6a16-132">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6a16-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e6a16-133">Example</span></span>

<span data-ttu-id="e6a16-134">В следующем примере извлекаем **все trustFrameworkPolicies.**</span><span class="sxs-lookup"><span data-stu-id="e6a16-134">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="e6a16-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6a16-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e6a16-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6a16-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/policies
```
# <a name="c"></a>[<span data-ttu-id="e6a16-137">C#</span><span class="sxs-lookup"><span data-stu-id="e6a16-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6a16-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6a16-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6a16-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6a16-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6a16-140">Java</span><span class="sxs-lookup"><span data-stu-id="e6a16-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-trustframeworks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e6a16-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6a16-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "B2C_1A_CustomPolicy2"
        },
        {
            "id": "B2C_1A_CustomPolicy3"
        },
        {
            "id": "B2C_1A_SocialAndLocalAccounts_Base"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


