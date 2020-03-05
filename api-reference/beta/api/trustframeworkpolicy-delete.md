---
title: Удаление Трустфрамеворкполици
description: Эта операция удаляет существующий объект Трустфрамеворкполици из клиента Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 08f96b0321b8b50973254b7c6cdf1a024e6ccd42
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452108"
---
# <a name="delete-trustframeworkpolicy"></a><span data-ttu-id="dd14f-103">Удаление Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="dd14f-103">Delete trustFrameworkPolicy</span></span>

<span data-ttu-id="dd14f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd14f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd14f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dd14f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd14f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd14f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd14f-107">Удаление существующего [трустфрамеворкполици](../resources/trustframeworkpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd14f-107">Delete an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd14f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd14f-108">Permissions</span></span>

<span data-ttu-id="dd14f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dd14f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="dd14f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd14f-111">Permission type</span></span>      | <span data-ttu-id="dd14f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd14f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd14f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd14f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd14f-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="dd14f-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="dd14f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd14f-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="dd14f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd14f-116">Not supported.</span></span>|
|<span data-ttu-id="dd14f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd14f-117">Application</span></span>|<span data-ttu-id="dd14f-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="dd14f-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="dd14f-119">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="dd14f-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="dd14f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd14f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /trustFramework/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dd14f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd14f-121">Request headers</span></span>

|<span data-ttu-id="dd14f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="dd14f-122">Name</span></span>|<span data-ttu-id="dd14f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dd14f-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="dd14f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd14f-124">Authorization</span></span>|<span data-ttu-id="dd14f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd14f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd14f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd14f-127">Request body</span></span>

<span data-ttu-id="dd14f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd14f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd14f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd14f-129">Response</span></span>

<span data-ttu-id="dd14f-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dd14f-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dd14f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dd14f-131">Example</span></span>

<span data-ttu-id="dd14f-132">В следующем примере удаляется объект **трустфрамеворкполици**.</span><span class="sxs-lookup"><span data-stu-id="dd14f-132">The following example deletes a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="dd14f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd14f-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dd14f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd14f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustFrameworkPolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base
```
# <a name="c"></a>[<span data-ttu-id="dd14f-135">C#</span><span class="sxs-lookup"><span data-stu-id="dd14f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd14f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd14f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd14f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd14f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd14f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd14f-138">Response</span></span>

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
