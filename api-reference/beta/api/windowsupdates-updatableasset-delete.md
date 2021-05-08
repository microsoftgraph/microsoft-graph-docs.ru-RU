---
title: Удаление updatableAsset
description: Удаление объекта updatableAsset.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 7e266a24fd23858f60326e14b956cdf5ef731315
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240731"
---
# <a name="delete-updatableasset"></a><span data-ttu-id="ac507-103">Удаление updatableAsset</span><span class="sxs-lookup"><span data-stu-id="ac507-103">Delete updatableAsset</span></span>
<span data-ttu-id="ac507-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ac507-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac507-105">Удаление [объекта updatableAsset.](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="ac507-105">Delete an [updatableAsset](../resources/windowsupdates-updatableasset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac507-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac507-106">Permissions</span></span>
<span data-ttu-id="ac507-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac507-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac507-109">Permission type</span></span>|<span data-ttu-id="ac507-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac507-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac507-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac507-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ac507-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac507-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="ac507-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac507-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac507-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac507-114">Not supported.</span></span>|
|<span data-ttu-id="ac507-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac507-115">Application</span></span>|<span data-ttu-id="ac507-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac507-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac507-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac507-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{updatableAssetId}
```

## <a name="request-headers"></a><span data-ttu-id="ac507-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac507-118">Request headers</span></span>
|<span data-ttu-id="ac507-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ac507-119">Name</span></span>|<span data-ttu-id="ac507-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ac507-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ac507-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac507-121">Authorization</span></span>|<span data-ttu-id="ac507-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac507-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac507-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac507-124">Request body</span></span>
<span data-ttu-id="ac507-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac507-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac507-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac507-126">Response</span></span>

<span data-ttu-id="ac507-p103">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ac507-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac507-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="ac507-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac507-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac507-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ac507-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac507-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_updatableasset"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetId}
```
# <a name="c"></a>[<span data-ttu-id="ac507-132">C#</span><span class="sxs-lookup"><span data-stu-id="ac507-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac507-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac507-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac507-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac507-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac507-135">Java</span><span class="sxs-lookup"><span data-stu-id="ac507-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac507-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac507-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

