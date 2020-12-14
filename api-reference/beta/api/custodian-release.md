---
title: 'custodian: release'
description: Освобождение хранителя из дела.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: ca5e2198280aae067f6da92ae03eb755a3bfa4f8
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658969"
---
# <a name="custodian-release"></a><span data-ttu-id="4d2da-103">custodian: release</span><span class="sxs-lookup"><span data-stu-id="4d2da-103">custodian: release</span></span>

<span data-ttu-id="4d2da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d2da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d2da-105">Освобождение хранителя из дела.</span><span class="sxs-lookup"><span data-stu-id="4d2da-105">Release a custodian from a case.</span></span> <span data-ttu-id="4d2da-106">For details, see [Release a custodian from a case](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span><span class="sxs-lookup"><span data-stu-id="4d2da-106">For details, see [Release a custodian from a case](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d2da-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d2da-107">Permissions</span></span>

<span data-ttu-id="4d2da-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d2da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d2da-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d2da-110">Permission type</span></span>|<span data-ttu-id="4d2da-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d2da-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d2da-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d2da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d2da-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="4d2da-113">User.Read</span></span>|
|<span data-ttu-id="4d2da-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d2da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d2da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d2da-115">Not supported.</span></span>|
|<span data-ttu-id="4d2da-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d2da-116">Application</span></span>|<span data-ttu-id="4d2da-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d2da-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d2da-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d2da-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/release
```

## <a name="request-headers"></a><span data-ttu-id="4d2da-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d2da-119">Request headers</span></span>

|<span data-ttu-id="4d2da-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4d2da-120">Name</span></span>|<span data-ttu-id="4d2da-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4d2da-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4d2da-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d2da-122">Authorization</span></span>|<span data-ttu-id="4d2da-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d2da-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4d2da-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d2da-125">Content-Type</span></span>|<span data-ttu-id="4d2da-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d2da-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d2da-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d2da-128">Request body</span></span>

<span data-ttu-id="4d2da-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d2da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d2da-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d2da-130">Response</span></span>

<span data-ttu-id="4d2da-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4d2da-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4d2da-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="4d2da-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d2da-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d2da-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4d2da-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d2da-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "custodian_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/release
```
# <a name="c"></a>[<span data-ttu-id="4d2da-135">C#</span><span class="sxs-lookup"><span data-stu-id="4d2da-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/custodian-release-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d2da-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d2da-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/custodian-release-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d2da-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d2da-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/custodian-release-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d2da-138">Java</span><span class="sxs-lookup"><span data-stu-id="4d2da-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/custodian-release-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d2da-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d2da-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
