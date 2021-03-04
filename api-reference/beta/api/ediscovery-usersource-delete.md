---
title: Удаление userSource
description: Удаляет объект userSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 86792f5fe7375d3abc644d718f0bf22c96e1f147
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446804"
---
# <a name="delete-usersource"></a><span data-ttu-id="55e52-103">Удаление userSource</span><span class="sxs-lookup"><span data-stu-id="55e52-103">Delete userSource</span></span>

<span data-ttu-id="55e52-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="55e52-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55e52-105">Удаление [объекта userSource.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="55e52-105">Delete a [userSource](../resources/ediscovery-usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55e52-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55e52-106">Permissions</span></span>

<span data-ttu-id="55e52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55e52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55e52-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55e52-109">Permission type</span></span>|<span data-ttu-id="55e52-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55e52-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55e52-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55e52-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55e52-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55e52-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="55e52-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55e52-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55e52-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55e52-114">Not supported.</span></span>|
|<span data-ttu-id="55e52-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55e52-115">Application</span></span>|<span data-ttu-id="55e52-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55e52-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55e52-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55e52-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="55e52-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55e52-118">Request headers</span></span>

|<span data-ttu-id="55e52-119">Имя</span><span class="sxs-lookup"><span data-stu-id="55e52-119">Name</span></span>|<span data-ttu-id="55e52-120">Описание</span><span class="sxs-lookup"><span data-stu-id="55e52-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="55e52-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55e52-121">Authorization</span></span>|<span data-ttu-id="55e52-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55e52-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55e52-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55e52-124">Request body</span></span>

<span data-ttu-id="55e52-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55e52-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55e52-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="55e52-126">Response</span></span>

<span data-ttu-id="55e52-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="55e52-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="55e52-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="55e52-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="55e52-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="55e52-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="55e52-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="55e52-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_usersource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```
# <a name="c"></a>[<span data-ttu-id="55e52-131">C#</span><span class="sxs-lookup"><span data-stu-id="55e52-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55e52-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55e52-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55e52-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55e52-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55e52-134">Java</span><span class="sxs-lookup"><span data-stu-id="55e52-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="55e52-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="55e52-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
