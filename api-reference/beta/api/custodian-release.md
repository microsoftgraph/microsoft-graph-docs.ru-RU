---
title: 'custodian: release'
description: Освобождение хранителя из дела.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 3b3fc0633672785e6a1f8aacc350fd9a8d34d4d7
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872501"
---
# <a name="custodian-release"></a><span data-ttu-id="e949a-103">custodian: release</span><span class="sxs-lookup"><span data-stu-id="e949a-103">custodian: release</span></span>

<span data-ttu-id="e949a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e949a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e949a-105">Освобождение хранителя из дела.</span><span class="sxs-lookup"><span data-stu-id="e949a-105">Release a custodian from a case.</span></span> <span data-ttu-id="e949a-106">For details, see [Release a custodian from a case](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span><span class="sxs-lookup"><span data-stu-id="e949a-106">For details, see [Release a custodian from a case](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="e949a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e949a-107">Permissions</span></span>

<span data-ttu-id="e949a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e949a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e949a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e949a-110">Permission type</span></span>|<span data-ttu-id="e949a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e949a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e949a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e949a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e949a-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="e949a-113">User.Read</span></span>|
|<span data-ttu-id="e949a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e949a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e949a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e949a-115">Not supported.</span></span>|
|<span data-ttu-id="e949a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e949a-116">Application</span></span>|<span data-ttu-id="e949a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e949a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e949a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e949a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/release
```

## <a name="request-headers"></a><span data-ttu-id="e949a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e949a-119">Request headers</span></span>

|<span data-ttu-id="e949a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e949a-120">Name</span></span>|<span data-ttu-id="e949a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e949a-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e949a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e949a-122">Authorization</span></span>|<span data-ttu-id="e949a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e949a-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e949a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e949a-125">Content-Type</span></span>|<span data-ttu-id="e949a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e949a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e949a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e949a-128">Request body</span></span>

<span data-ttu-id="e949a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e949a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e949a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e949a-130">Response</span></span>

<span data-ttu-id="e949a-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e949a-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e949a-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="e949a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e949a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e949a-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e949a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e949a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "custodian_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/release
```
# <a name="c"></a>[<span data-ttu-id="e949a-135">C#</span><span class="sxs-lookup"><span data-stu-id="e949a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/custodian-release-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e949a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e949a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/custodian-release-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e949a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e949a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/custodian-release-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e949a-138">Java</span><span class="sxs-lookup"><span data-stu-id="e949a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/custodian-release-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e949a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e949a-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
