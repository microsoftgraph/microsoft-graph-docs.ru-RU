---
title: 'cloudPC: reprovision'
description: Повторное создание определенного облачного КОМПЬЮТЕРА.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7a887ced74a6b0eb53e1516f314cc2be5ff96428
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872879"
---
# <a name="cloudpc-reprovision"></a><span data-ttu-id="e5b30-103">cloudPC: reprovision</span><span class="sxs-lookup"><span data-stu-id="e5b30-103">cloudPC: reprovision</span></span>

<span data-ttu-id="e5b30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5b30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5b30-105">Повторное создание определенного облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="e5b30-105">Reprovision a specific cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="e5b30-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5b30-106">Permissions</span></span>

<span data-ttu-id="e5b30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5b30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5b30-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5b30-109">Permission type</span></span>|<span data-ttu-id="e5b30-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5b30-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5b30-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5b30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e5b30-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5b30-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="e5b30-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5b30-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5b30-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5b30-114">Not supported.</span></span>|
|<span data-ttu-id="e5b30-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5b30-115">Application</span></span>|<span data-ttu-id="e5b30-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5b30-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5b30-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5b30-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```

## <a name="request-headers"></a><span data-ttu-id="e5b30-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5b30-118">Request headers</span></span>

|<span data-ttu-id="e5b30-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e5b30-119">Name</span></span>|<span data-ttu-id="e5b30-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e5b30-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e5b30-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5b30-121">Authorization</span></span>|<span data-ttu-id="e5b30-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5b30-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5b30-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5b30-124">Request body</span></span>

<span data-ttu-id="e5b30-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5b30-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5b30-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5b30-126">Response</span></span>

<span data-ttu-id="e5b30-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e5b30-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e5b30-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e5b30-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5b30-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5b30-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e5b30-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5b30-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```
# <a name="c"></a>[<span data-ttu-id="e5b30-131">C#</span><span class="sxs-lookup"><span data-stu-id="e5b30-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5b30-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5b30-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5b30-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5b30-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5b30-134">Java</span><span class="sxs-lookup"><span data-stu-id="e5b30-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5b30-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5b30-135">Response</span></span>

<span data-ttu-id="e5b30-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e5b30-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
