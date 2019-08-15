---
title: Удаление Трустфрамеворкполици
description: Эта операция удаляет существующий объект Трустфрамеворкполици из клиента Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e71048b1ffc461228670521fd971e6df293cd5e4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409200"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="f63f0-103">Удаление Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="f63f0-103">Delete trustFrameworkPolicy</span></span>

> <span data-ttu-id="f63f0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f63f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f63f0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f63f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f63f0-106">Удаление существующего [трустфрамеворкполици](../resources/trustframeworkpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f63f0-106">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f63f0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f63f0-107">Permissions</span></span>

<span data-ttu-id="f63f0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f63f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f63f0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f63f0-110">Permission type</span></span>      | <span data-ttu-id="f63f0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f63f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f63f0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f63f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f63f0-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="f63f0-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="f63f0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f63f0-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f63f0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f63f0-115">Not supported.</span></span>|
|<span data-ttu-id="f63f0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f63f0-116">Application</span></span>|<span data-ttu-id="f63f0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f63f0-117">Not supported.</span></span>|

<span data-ttu-id="f63f0-118">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="f63f0-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f63f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f63f0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f63f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f63f0-120">Request headers</span></span>

|<span data-ttu-id="f63f0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f63f0-121">Name</span></span>|<span data-ttu-id="f63f0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f63f0-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f63f0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f63f0-123">Authorization</span></span>|<span data-ttu-id="f63f0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f63f0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f63f0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f63f0-126">Request body</span></span>

<span data-ttu-id="f63f0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f63f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f63f0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f63f0-128">Response</span></span>

<span data-ttu-id="f63f0-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f63f0-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f63f0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f63f0-130">Example</span></span>

<span data-ttu-id="f63f0-131">В следующем примере удаляется объект **трустфрамеворкполици**.</span><span class="sxs-lookup"><span data-stu-id="f63f0-131">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="f63f0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f63f0-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f63f0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f63f0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f63f0-134">C#</span><span class="sxs-lookup"><span data-stu-id="f63f0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f63f0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f63f0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f63f0-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f63f0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f63f0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f63f0-137">Response</span></span>

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
