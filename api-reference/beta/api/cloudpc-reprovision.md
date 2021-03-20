---
title: 'cloudPC: reprovision'
description: Перепроизводить определенный облачный КОМПЬЮТЕР.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 90ab69337fc0cd1d7f7f73df5ee84afe13b98021
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947647"
---
# <a name="cloudpc-reprovision"></a><span data-ttu-id="8c9ce-103">cloudPC: reprovision</span><span class="sxs-lookup"><span data-stu-id="8c9ce-103">cloudPC: reprovision</span></span>

<span data-ttu-id="8c9ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c9ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c9ce-105">Перепроизводить определенный облачный КОМПЬЮТЕР.</span><span class="sxs-lookup"><span data-stu-id="8c9ce-105">Reprovision a specific cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="8c9ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c9ce-106">Permissions</span></span>

<span data-ttu-id="8c9ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c9ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c9ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c9ce-109">Permission type</span></span>|<span data-ttu-id="8c9ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c9ce-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c9ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c9ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c9ce-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c9ce-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="8c9ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c9ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c9ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c9ce-114">Not supported.</span></span>|
|<span data-ttu-id="8c9ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c9ce-115">Application</span></span>|<span data-ttu-id="8c9ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c9ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c9ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c9ce-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```

## <a name="request-headers"></a><span data-ttu-id="8c9ce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c9ce-118">Request headers</span></span>

|<span data-ttu-id="8c9ce-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8c9ce-119">Name</span></span>|<span data-ttu-id="8c9ce-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8c9ce-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8c9ce-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c9ce-121">Authorization</span></span>|<span data-ttu-id="8c9ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c9ce-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c9ce-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c9ce-124">Request body</span></span>

<span data-ttu-id="8c9ce-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c9ce-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c9ce-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c9ce-126">Response</span></span>

<span data-ttu-id="8c9ce-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8c9ce-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8c9ce-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c9ce-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c9ce-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c9ce-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8c9ce-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c9ce-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck_1"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```
# <a name="c"></a>[<span data-ttu-id="8c9ce-131">C#</span><span class="sxs-lookup"><span data-stu-id="8c9ce-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c9ce-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c9ce-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c9ce-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c9ce-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c9ce-134">Java</span><span class="sxs-lookup"><span data-stu-id="8c9ce-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c9ce-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c9ce-135">Response</span></span>

<span data-ttu-id="8c9ce-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c9ce-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
