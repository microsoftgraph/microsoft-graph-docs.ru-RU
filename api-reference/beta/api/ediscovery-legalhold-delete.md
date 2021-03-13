---
title: Удаление legalHold
description: Удаление объекта legalHold.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 84d94cf4ce0d340d36cb0cf5f2b478c70581f374
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773132"
---
# <a name="delete-legalhold"></a><span data-ttu-id="a67cb-103">Удаление legalHold</span><span class="sxs-lookup"><span data-stu-id="a67cb-103">Delete legalHold</span></span>

<span data-ttu-id="a67cb-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a67cb-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a67cb-105">Удаление [объекта legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="a67cb-105">Delete a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a67cb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a67cb-106">Permissions</span></span>

<span data-ttu-id="a67cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a67cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a67cb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a67cb-109">Permission type</span></span>|<span data-ttu-id="a67cb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a67cb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a67cb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a67cb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a67cb-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a67cb-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a67cb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a67cb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a67cb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a67cb-114">Not supported.</span></span>|
|<span data-ttu-id="a67cb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a67cb-115">Application</span></span>|<span data-ttu-id="a67cb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a67cb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a67cb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a67cb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/legalHolds/{legalHoldId}
```

## <a name="request-headers"></a><span data-ttu-id="a67cb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a67cb-118">Request headers</span></span>

|<span data-ttu-id="a67cb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a67cb-119">Name</span></span>|<span data-ttu-id="a67cb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a67cb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a67cb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a67cb-121">Authorization</span></span>|<span data-ttu-id="a67cb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a67cb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a67cb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a67cb-124">Request body</span></span>

<span data-ttu-id="a67cb-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a67cb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a67cb-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a67cb-126">Response</span></span>

<span data-ttu-id="a67cb-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a67cb-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a67cb-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a67cb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a67cb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a67cb-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a67cb-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a67cb-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_legalhold"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```
# <a name="c"></a>[<span data-ttu-id="a67cb-131">C#</span><span class="sxs-lookup"><span data-stu-id="a67cb-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-legalhold-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a67cb-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a67cb-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-legalhold-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a67cb-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a67cb-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-legalhold-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a67cb-134">Java</span><span class="sxs-lookup"><span data-stu-id="a67cb-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-legalhold-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a67cb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a67cb-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
