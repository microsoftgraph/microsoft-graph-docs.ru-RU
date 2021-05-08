---
title: Удаление развертывания
description: Удаление объекта развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 3baf7f9d163c7f1f4beb8967ca8cb94b53fb95f5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241383"
---
# <a name="delete-deployment"></a><span data-ttu-id="16936-103">Удаление развертывания</span><span class="sxs-lookup"><span data-stu-id="16936-103">Delete deployment</span></span>
<span data-ttu-id="16936-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="16936-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16936-105">Удаление [объекта развертывания.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="16936-105">Delete a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="16936-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16936-106">Permissions</span></span>
<span data-ttu-id="16936-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16936-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16936-109">Permission type</span></span>|<span data-ttu-id="16936-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16936-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16936-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16936-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16936-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16936-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="16936-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16936-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16936-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16936-114">Not supported.</span></span>|
|<span data-ttu-id="16936-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16936-115">Application</span></span>|<span data-ttu-id="16936-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16936-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16936-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16936-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/deployments/{deploymentId}
```

## <a name="request-headers"></a><span data-ttu-id="16936-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16936-118">Request headers</span></span>
|<span data-ttu-id="16936-119">Имя</span><span class="sxs-lookup"><span data-stu-id="16936-119">Name</span></span>|<span data-ttu-id="16936-120">Описание</span><span class="sxs-lookup"><span data-stu-id="16936-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="16936-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16936-121">Authorization</span></span>|<span data-ttu-id="16936-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16936-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16936-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16936-124">Request body</span></span>
<span data-ttu-id="16936-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16936-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16936-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="16936-126">Response</span></span>

<span data-ttu-id="16936-p103">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16936-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16936-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="16936-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16936-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="16936-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="16936-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="16936-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_deployment"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}
```
# <a name="c"></a>[<span data-ttu-id="16936-132">C#</span><span class="sxs-lookup"><span data-stu-id="16936-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-deployment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16936-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16936-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-deployment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16936-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16936-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-deployment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16936-135">Java</span><span class="sxs-lookup"><span data-stu-id="16936-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-deployment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="16936-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="16936-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

