---
title: Удаление siteSource
description: Удаление объекта siteSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 5d929949aa18a1fb2b47347828b2e4d7d20a9cec
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874440"
---
# <a name="delete-sitesource"></a><span data-ttu-id="12217-103">Удаление siteSource</span><span class="sxs-lookup"><span data-stu-id="12217-103">Delete siteSource</span></span>

<span data-ttu-id="12217-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12217-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12217-105">Удаление объекта [siteSource.](../resources/sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="12217-105">Delete a [siteSource](../resources/sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="12217-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12217-106">Permissions</span></span>

<span data-ttu-id="12217-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12217-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12217-109">Permission type</span></span>|<span data-ttu-id="12217-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12217-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12217-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12217-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12217-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="12217-112">User.Read</span></span>|
|<span data-ttu-id="12217-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12217-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12217-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12217-114">Not supported.</span></span>|
|<span data-ttu-id="12217-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12217-115">Application</span></span>|<span data-ttu-id="12217-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12217-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12217-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12217-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources/{siteSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="12217-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12217-118">Request headers</span></span>

|<span data-ttu-id="12217-119">Имя</span><span class="sxs-lookup"><span data-stu-id="12217-119">Name</span></span>|<span data-ttu-id="12217-120">Описание</span><span class="sxs-lookup"><span data-stu-id="12217-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="12217-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12217-121">Authorization</span></span>|<span data-ttu-id="12217-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12217-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12217-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12217-124">Request body</span></span>

<span data-ttu-id="12217-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12217-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12217-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="12217-126">Response</span></span>

<span data-ttu-id="12217-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="12217-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="12217-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="12217-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12217-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="12217-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="12217-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="12217-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sitesource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources/38304445-3741-3333-4233-344238454333
```
# <a name="c"></a>[<span data-ttu-id="12217-131">C#</span><span class="sxs-lookup"><span data-stu-id="12217-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sitesource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12217-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12217-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sitesource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12217-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12217-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sitesource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12217-134">Java</span><span class="sxs-lookup"><span data-stu-id="12217-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-sitesource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="12217-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="12217-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
