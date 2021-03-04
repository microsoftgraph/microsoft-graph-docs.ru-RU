---
title: 'случай: закрыть'
description: Закрой дело об обнаружении электронной почты.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d5fd2bcf997660dac803a9e417ee93d41f95882a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447188"
---
# <a name="case-close"></a><span data-ttu-id="c3e14-103">случай: закрыть</span><span class="sxs-lookup"><span data-stu-id="c3e14-103">case: close</span></span>

<span data-ttu-id="c3e14-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="c3e14-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3e14-105">Закрой дело об обнаружении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c3e14-105">Close an eDiscovery case.</span></span> <span data-ttu-id="c3e14-106">Подробные сведения [см. в материале Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span><span class="sxs-lookup"><span data-stu-id="c3e14-106">For details, see [Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3e14-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3e14-107">Permissions</span></span>

<span data-ttu-id="c3e14-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3e14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3e14-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3e14-110">Permission type</span></span>|<span data-ttu-id="c3e14-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3e14-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3e14-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3e14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3e14-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3e14-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="c3e14-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3e14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3e14-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e14-115">Not supported.</span></span>|
|<span data-ttu-id="c3e14-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3e14-116">Application</span></span>|<span data-ttu-id="c3e14-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e14-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3e14-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3e14-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{CaseId}/close
```

## <a name="request-headers"></a><span data-ttu-id="c3e14-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3e14-119">Request headers</span></span>

|<span data-ttu-id="c3e14-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c3e14-120">Name</span></span>|<span data-ttu-id="c3e14-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c3e14-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3e14-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3e14-122">Authorization</span></span>|<span data-ttu-id="c3e14-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3e14-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3e14-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3e14-125">Request body</span></span>

<span data-ttu-id="c3e14-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3e14-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3e14-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3e14-127">Response</span></span>

<span data-ttu-id="c3e14-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c3e14-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c3e14-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c3e14-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3e14-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3e14-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c3e14-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3e14-131">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "case_close"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/close
```

# <a name="c"></a>[<span data-ttu-id="c3e14-132">C#</span><span class="sxs-lookup"><span data-stu-id="c3e14-132">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-close-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3e14-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3e14-133">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-close-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3e14-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3e14-134">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-close-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3e14-135">Java</span><span class="sxs-lookup"><span data-stu-id="c3e14-135">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-close-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c3e14-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3e14-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
