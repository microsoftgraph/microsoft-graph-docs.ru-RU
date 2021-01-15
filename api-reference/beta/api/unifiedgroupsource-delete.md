---
title: Удаление unifiedGroupSource
description: Удаление объекта unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 1e5145d3e067c92ce5faf8f9ddd6b7012bd19220
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872459"
---
# <a name="delete-unifiedgroupsource"></a><span data-ttu-id="cb414-103">Удаление unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="cb414-103">Delete unifiedGroupSource</span></span>

<span data-ttu-id="cb414-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb414-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb414-105">Удаление объекта [unifiedGroupSource.](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="cb414-105">Delete a [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb414-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb414-106">Permissions</span></span>

<span data-ttu-id="cb414-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb414-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb414-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb414-109">Permission type</span></span>|<span data-ttu-id="cb414-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb414-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb414-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb414-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb414-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="cb414-112">User.Read</span></span>|
|<span data-ttu-id="cb414-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb414-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb414-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb414-114">Not supported.</span></span>|
|<span data-ttu-id="cb414-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb414-115">Application</span></span>|<span data-ttu-id="cb414-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb414-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb414-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb414-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633
```

## <a name="request-headers"></a><span data-ttu-id="cb414-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb414-118">Request headers</span></span>

|<span data-ttu-id="cb414-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cb414-119">Name</span></span>|<span data-ttu-id="cb414-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cb414-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb414-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb414-121">Authorization</span></span>|<span data-ttu-id="cb414-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb414-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb414-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb414-124">Request body</span></span>

<span data-ttu-id="cb414-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb414-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb414-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb414-126">Response</span></span>

<span data-ttu-id="cb414-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cb414-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cb414-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb414-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb414-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb414-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cb414-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb414-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedgroupsource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}
```
# <a name="c"></a>[<span data-ttu-id="cb414-131">C#</span><span class="sxs-lookup"><span data-stu-id="cb414-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedgroupsource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb414-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb414-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedgroupsource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb414-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb414-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedgroupsource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb414-134">Java</span><span class="sxs-lookup"><span data-stu-id="cb414-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedgroupsource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cb414-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb414-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
