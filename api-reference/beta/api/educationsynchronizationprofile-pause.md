---
title: Приостановка синхронизации в Едукатионсинчронизатионпрофиле
description: Приостановите синхронизацию определенного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 003505dcfc00631f6d7ed9c40dbd9e4c8c3cebd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007205"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="c0a20-103">Приостановка синхронизации в Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="c0a20-103">Pause sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="c0a20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0a20-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0a20-105">Приостановите синхронизацию определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c0a20-105">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0a20-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0a20-106">Permissions</span></span>
<span data-ttu-id="c0a20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0a20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0a20-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0a20-109">Permission type</span></span> | <span data-ttu-id="c0a20-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0a20-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c0a20-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0a20-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0a20-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0a20-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c0a20-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0a20-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c0a20-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0a20-114">Not supported.</span></span>|
|<span data-ttu-id="c0a20-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0a20-115">Application</span></span>|<span data-ttu-id="c0a20-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0a20-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0a20-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0a20-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="c0a20-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0a20-118">Request headers</span></span>
| <span data-ttu-id="c0a20-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c0a20-119">Name</span></span>       | <span data-ttu-id="c0a20-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c0a20-120">Type</span></span> | <span data-ttu-id="c0a20-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c0a20-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0a20-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0a20-122">Authorization</span></span>  | <span data-ttu-id="c0a20-123">string</span><span class="sxs-lookup"><span data-stu-id="c0a20-123">string</span></span>  | <span data-ttu-id="c0a20-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0a20-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0a20-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0a20-126">Request body</span></span>
<span data-ttu-id="c0a20-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0a20-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c0a20-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0a20-128">Response</span></span>
<span data-ttu-id="c0a20-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c0a20-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0a20-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c0a20-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0a20-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0a20-131">Request</span></span>
<span data-ttu-id="c0a20-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0a20-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0a20-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0a20-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="c"></a>[<span data-ttu-id="c0a20-134">C#</span><span class="sxs-lookup"><span data-stu-id="c0a20-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0a20-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0a20-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0a20-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0a20-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c0a20-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0a20-137">Response</span></span>

<span data-ttu-id="c0a20-138">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="c0a20-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```http
HTTP/1.1 200 OK
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


