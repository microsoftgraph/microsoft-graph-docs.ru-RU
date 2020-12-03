---
title: Удаление Клаудпкпровисионингполици
description: Удаление объекта Клаудпкпровисионингполици.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 18b98a3d7afab82e554b35a5dd018608407689a2
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563445"
---
# <a name="delete-cloudpcprovisioningpolicy"></a><span data-ttu-id="dc891-103">Удаление Клаудпкпровисионингполици</span><span class="sxs-lookup"><span data-stu-id="dc891-103">Delete cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="dc891-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc891-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc891-105">Удаление объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="dc891-105">Delete a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span> <span data-ttu-id="dc891-106">Вы не можете удалить используемую политику.</span><span class="sxs-lookup"><span data-stu-id="dc891-106">You can’t delete a policy that’s in use.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="dc891-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc891-107">Permissions</span></span>

<span data-ttu-id="dc891-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc891-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc891-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc891-110">Permission type</span></span>|<span data-ttu-id="dc891-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc891-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc891-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc891-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc891-113">Клаудпк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dc891-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="dc891-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc891-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc891-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc891-115">Not supported.</span></span>|
|<span data-ttu-id="dc891-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc891-116">Application</span></span>|<span data-ttu-id="dc891-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc891-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc891-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc891-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dc891-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc891-119">Request headers</span></span>

|<span data-ttu-id="dc891-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dc891-120">Name</span></span>|<span data-ttu-id="dc891-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dc891-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc891-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc891-122">Authorization</span></span>|<span data-ttu-id="dc891-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc891-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc891-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc891-125">Request body</span></span>

<span data-ttu-id="dc891-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc891-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc891-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc891-127">Response</span></span>

<span data-ttu-id="dc891-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc891-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dc891-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="dc891-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc891-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc891-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dc891-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc891-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_provisioningpolicies_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="dc891-132">C#</span><span class="sxs-lookup"><span data-stu-id="dc891-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-provisioningpolicies-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc891-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc891-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-provisioningpolicies-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc891-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc891-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-provisioningpolicies-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc891-135">Java</span><span class="sxs-lookup"><span data-stu-id="dc891-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-provisioningpolicies-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dc891-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc891-136">Response</span></span>

<span data-ttu-id="dc891-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dc891-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
