---
title: 'ediscoveryCase: reopen'
description: Повторное открытие дела eDiscovery, которое было закрыто.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f8eb4265fb87668023038ddaa50967cad22c2a91
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872298"
---
# <a name="ediscoverycase-reopen"></a><span data-ttu-id="70cb8-103">ediscoveryCase: reopen</span><span class="sxs-lookup"><span data-stu-id="70cb8-103">ediscoveryCase: reopen</span></span>

<span data-ttu-id="70cb8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70cb8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70cb8-105">Повторное открытие дела eDiscovery, которое было закрыто.</span><span class="sxs-lookup"><span data-stu-id="70cb8-105">Reopen an eDiscovery case that was closed.</span></span> <span data-ttu-id="70cb8-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span><span class="sxs-lookup"><span data-stu-id="70cb8-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="70cb8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70cb8-107">Permissions</span></span>
<span data-ttu-id="70cb8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70cb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70cb8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70cb8-110">Permission type</span></span>|<span data-ttu-id="70cb8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70cb8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70cb8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70cb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70cb8-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="70cb8-113">User.Read</span></span>|
|<span data-ttu-id="70cb8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70cb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70cb8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70cb8-115">Not supported.</span></span>|
|<span data-ttu-id="70cb8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70cb8-116">Application</span></span>|<span data-ttu-id="70cb8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70cb8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70cb8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70cb8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/reopen
```

## <a name="request-headers"></a><span data-ttu-id="70cb8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70cb8-119">Request headers</span></span>

|<span data-ttu-id="70cb8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="70cb8-120">Name</span></span>|<span data-ttu-id="70cb8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="70cb8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="70cb8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70cb8-122">Authorization</span></span>|<span data-ttu-id="70cb8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70cb8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70cb8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70cb8-125">Request body</span></span>

<span data-ttu-id="70cb8-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70cb8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70cb8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="70cb8-127">Response</span></span>

<span data-ttu-id="70cb8-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="70cb8-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="70cb8-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="70cb8-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70cb8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="70cb8-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="70cb8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="70cb8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoverycase_reopen"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen
```
# <a name="c"></a>[<span data-ttu-id="70cb8-132">C#</span><span class="sxs-lookup"><span data-stu-id="70cb8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-reopen-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70cb8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70cb8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-reopen-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70cb8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70cb8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-reopen-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70cb8-135">Java</span><span class="sxs-lookup"><span data-stu-id="70cb8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-reopen-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="70cb8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="70cb8-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
