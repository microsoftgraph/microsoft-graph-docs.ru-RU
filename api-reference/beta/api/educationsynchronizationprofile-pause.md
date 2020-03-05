---
title: Приостановка синхронизации в Едукатионсинчронизатионпрофиле
description: Приостановите синхронизацию определенного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 71012e82fdb3e695d1ccf4e61dc9433c7fa2ebc1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424458"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="5243a-103">Приостановка синхронизации в Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="5243a-103">Pause sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="5243a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5243a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5243a-105">Приостановите синхронизацию определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5243a-105">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5243a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5243a-106">Permissions</span></span>
<span data-ttu-id="5243a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5243a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5243a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5243a-109">Permission type</span></span> | <span data-ttu-id="5243a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5243a-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="5243a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5243a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5243a-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5243a-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="5243a-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5243a-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5243a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5243a-114">Not supported.</span></span>|
|<span data-ttu-id="5243a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5243a-115">Application</span></span>|<span data-ttu-id="5243a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5243a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5243a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5243a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="5243a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5243a-118">Request headers</span></span>
| <span data-ttu-id="5243a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5243a-119">Name</span></span>       | <span data-ttu-id="5243a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="5243a-120">Type</span></span> | <span data-ttu-id="5243a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5243a-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5243a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5243a-122">Authorization</span></span>  | <span data-ttu-id="5243a-123">string</span><span class="sxs-lookup"><span data-stu-id="5243a-123">string</span></span>  | <span data-ttu-id="5243a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5243a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5243a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5243a-126">Request body</span></span>
<span data-ttu-id="5243a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5243a-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5243a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5243a-128">Response</span></span>
<span data-ttu-id="5243a-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="5243a-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5243a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5243a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5243a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5243a-131">Request</span></span>
<span data-ttu-id="5243a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5243a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5243a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5243a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="c"></a>[<span data-ttu-id="5243a-134">C#</span><span class="sxs-lookup"><span data-stu-id="5243a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5243a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5243a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5243a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5243a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5243a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5243a-137">Response</span></span>

<span data-ttu-id="5243a-138">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="5243a-138">There is no response body.</span></span>

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
