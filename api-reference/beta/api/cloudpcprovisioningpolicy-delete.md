---
title: Удаление cloudPcProvisioningPolicy
description: Удаление объекта cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b90a8005f7d2f4e48e07cce07ba3ba525c6fd0f2
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872739"
---
# <a name="delete-cloudpcprovisioningpolicy"></a><span data-ttu-id="35ff7-103">Удаление cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="35ff7-103">Delete cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="35ff7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35ff7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35ff7-105">Удаление объекта [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35ff7-105">Delete a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span> <span data-ttu-id="35ff7-106">Вы не можете удалить используемую политику.</span><span class="sxs-lookup"><span data-stu-id="35ff7-106">You can’t delete a policy that’s in use.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="35ff7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35ff7-107">Permissions</span></span>

<span data-ttu-id="35ff7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35ff7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35ff7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35ff7-110">Permission type</span></span>|<span data-ttu-id="35ff7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35ff7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35ff7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35ff7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35ff7-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35ff7-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="35ff7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35ff7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35ff7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35ff7-115">Not supported.</span></span>|
|<span data-ttu-id="35ff7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35ff7-116">Application</span></span>|<span data-ttu-id="35ff7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35ff7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35ff7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35ff7-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="35ff7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35ff7-119">Request headers</span></span>

|<span data-ttu-id="35ff7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="35ff7-120">Name</span></span>|<span data-ttu-id="35ff7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="35ff7-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="35ff7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35ff7-122">Authorization</span></span>|<span data-ttu-id="35ff7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35ff7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="35ff7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35ff7-125">Request body</span></span>

<span data-ttu-id="35ff7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35ff7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35ff7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="35ff7-127">Response</span></span>

<span data-ttu-id="35ff7-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="35ff7-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="35ff7-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="35ff7-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35ff7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="35ff7-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="35ff7-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="35ff7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_provisioningpolicies_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="35ff7-132">C#</span><span class="sxs-lookup"><span data-stu-id="35ff7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-provisioningpolicies-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35ff7-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35ff7-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-provisioningpolicies-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35ff7-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35ff7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-provisioningpolicies-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35ff7-135">Java</span><span class="sxs-lookup"><span data-stu-id="35ff7-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-provisioningpolicies-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35ff7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="35ff7-136">Response</span></span>

<span data-ttu-id="35ff7-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="35ff7-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
