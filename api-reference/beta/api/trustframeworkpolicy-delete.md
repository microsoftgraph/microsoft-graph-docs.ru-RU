---
title: Удаление trustFrameworkPolicy
description: Эта операция удаляет существующий объект trustFrameworkPolicy из клиента Azure AD B2C.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0ebca87f50af1d4db6c4b6053bcabcaf9aa672d3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444954"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="6825e-103">Удаление trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="6825e-103">Delete trustFrameworkPolicy</span></span>

<span data-ttu-id="6825e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6825e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6825e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6825e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6825e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6825e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6825e-107">Удаление существующего [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6825e-107">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6825e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6825e-108">Permissions</span></span>

<span data-ttu-id="6825e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6825e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="6825e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6825e-111">Permission type</span></span>      | <span data-ttu-id="6825e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6825e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6825e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6825e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6825e-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="6825e-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="6825e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6825e-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6825e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6825e-116">Not supported.</span></span>|
|<span data-ttu-id="6825e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6825e-117">Application</span></span>|<span data-ttu-id="6825e-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="6825e-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="6825e-119">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="6825e-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="6825e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6825e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6825e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6825e-121">Request headers</span></span>

|<span data-ttu-id="6825e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6825e-122">Name</span></span>|<span data-ttu-id="6825e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6825e-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6825e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6825e-124">Authorization</span></span>|<span data-ttu-id="6825e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6825e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6825e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6825e-127">Request body</span></span>

<span data-ttu-id="6825e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6825e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6825e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6825e-129">Response</span></span>

<span data-ttu-id="6825e-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6825e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6825e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6825e-131">Example</span></span>

<span data-ttu-id="6825e-132">В следующем примере **удаляется trustFrameworkPolicy**.</span><span class="sxs-lookup"><span data-stu-id="6825e-132">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="6825e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6825e-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6825e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6825e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```
# <a name="c"></a>[<span data-ttu-id="6825e-135">C#</span><span class="sxs-lookup"><span data-stu-id="6825e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6825e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6825e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6825e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6825e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6825e-138">Java</span><span class="sxs-lookup"><span data-stu-id="6825e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-trustframeworkpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6825e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6825e-139">Response</span></span>

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
  "description": "Delete trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


