---
title: 'случай: повторное открытие'
description: Повторное открытие закрытого дела об обнаружении электронной почты.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5eaa03b81502273e6aae914fa699311457df9cd9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447104"
---
# <a name="case-reopen"></a><span data-ttu-id="b3d0b-103">случай: повторное открытие</span><span class="sxs-lookup"><span data-stu-id="b3d0b-103">case: reopen</span></span>

<span data-ttu-id="b3d0b-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b3d0b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3d0b-105">Повторное открытие закрытого дела об обнаружении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b3d0b-105">Reopen an eDiscovery case that was closed.</span></span> <span data-ttu-id="b3d0b-106">Подробные сведения см. [в материале Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span><span class="sxs-lookup"><span data-stu-id="b3d0b-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3d0b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3d0b-107">Permissions</span></span>

<span data-ttu-id="b3d0b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3d0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3d0b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3d0b-110">Permission type</span></span>|<span data-ttu-id="b3d0b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3d0b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3d0b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3d0b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3d0b-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d0b-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="b3d0b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3d0b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3d0b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d0b-115">Not supported.</span></span>|
|<span data-ttu-id="b3d0b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3d0b-116">Application</span></span>|<span data-ttu-id="b3d0b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d0b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3d0b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3d0b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reopen
```

## <a name="request-headers"></a><span data-ttu-id="b3d0b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3d0b-119">Request headers</span></span>

|<span data-ttu-id="b3d0b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b3d0b-120">Name</span></span>|<span data-ttu-id="b3d0b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b3d0b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b3d0b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3d0b-122">Authorization</span></span>|<span data-ttu-id="b3d0b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3d0b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3d0b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b3d0b-125">Request body</span></span>

<span data-ttu-id="b3d0b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3d0b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3d0b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3d0b-127">Response</span></span>

<span data-ttu-id="b3d0b-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b3d0b-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b3d0b-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3d0b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3d0b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3d0b-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b3d0b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3d0b-131">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "case_reopen"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen
```
# <a name="c"></a>[<span data-ttu-id="b3d0b-132">C#</span><span class="sxs-lookup"><span data-stu-id="b3d0b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-reopen-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3d0b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3d0b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-reopen-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3d0b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3d0b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-reopen-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3d0b-135">Java</span><span class="sxs-lookup"><span data-stu-id="b3d0b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-reopen-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b3d0b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3d0b-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
