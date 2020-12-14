---
title: 'ediscoveryCase: reopen'
description: Повторное открытие дела eDiscovery, которое было закрыто.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 256dba8a09e2be3be20aadd4e2c8e9927f2b20df
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657113"
---
# <a name="ediscoverycase-reopen"></a><span data-ttu-id="4672d-103">ediscoveryCase: reopen</span><span class="sxs-lookup"><span data-stu-id="4672d-103">ediscoveryCase: reopen</span></span>

<span data-ttu-id="4672d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4672d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4672d-105">Повторное открытие дела eDiscovery, которое было закрыто.</span><span class="sxs-lookup"><span data-stu-id="4672d-105">Reopen an eDiscovery case that was closed.</span></span> <span data-ttu-id="4672d-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span><span class="sxs-lookup"><span data-stu-id="4672d-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="4672d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4672d-107">Permissions</span></span>
<span data-ttu-id="4672d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4672d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4672d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4672d-110">Permission type</span></span>|<span data-ttu-id="4672d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4672d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4672d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4672d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4672d-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="4672d-113">User.Read</span></span>|
|<span data-ttu-id="4672d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4672d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4672d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4672d-115">Not supported.</span></span>|
|<span data-ttu-id="4672d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4672d-116">Application</span></span>|<span data-ttu-id="4672d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4672d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4672d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4672d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/reopen
```

## <a name="request-headers"></a><span data-ttu-id="4672d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4672d-119">Request headers</span></span>

|<span data-ttu-id="4672d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4672d-120">Name</span></span>|<span data-ttu-id="4672d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4672d-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4672d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4672d-122">Authorization</span></span>|<span data-ttu-id="4672d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4672d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4672d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4672d-125">Request body</span></span>

<span data-ttu-id="4672d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4672d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4672d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4672d-127">Response</span></span>

<span data-ttu-id="4672d-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4672d-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4672d-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="4672d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4672d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4672d-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4672d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4672d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoverycase_reopen"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen
```
# <a name="c"></a>[<span data-ttu-id="4672d-132">C#</span><span class="sxs-lookup"><span data-stu-id="4672d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-reopen-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4672d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4672d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-reopen-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4672d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4672d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-reopen-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4672d-135">Java</span><span class="sxs-lookup"><span data-stu-id="4672d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-reopen-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4672d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4672d-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
