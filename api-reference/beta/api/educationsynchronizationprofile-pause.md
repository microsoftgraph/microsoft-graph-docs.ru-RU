---
title: Синхронизация паузы на educationSynchronizationProfile
description: Приостановка синхронизации определенного профиля синхронизации школьных данных в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 44477aae7799922008b0a7623fd7e4c91c09e0aa
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574218"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="aa96f-103">Синхронизация паузы на educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="aa96f-103">Pause sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="aa96f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa96f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa96f-105">Приостановка синхронизации определенного профиля синхронизации [школьных данных](../resources/educationsynchronizationprofile.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="aa96f-105">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa96f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa96f-106">Permissions</span></span>
<span data-ttu-id="aa96f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa96f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa96f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa96f-109">Permission type</span></span> | <span data-ttu-id="aa96f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa96f-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="aa96f-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa96f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aa96f-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa96f-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="aa96f-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa96f-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="aa96f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa96f-114">Not supported.</span></span>|
|<span data-ttu-id="aa96f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa96f-115">Application</span></span>|<span data-ttu-id="aa96f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa96f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa96f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa96f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="aa96f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa96f-118">Request headers</span></span>
| <span data-ttu-id="aa96f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="aa96f-119">Name</span></span>       | <span data-ttu-id="aa96f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="aa96f-120">Type</span></span> | <span data-ttu-id="aa96f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="aa96f-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa96f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa96f-122">Authorization</span></span>  | <span data-ttu-id="aa96f-123">string</span><span class="sxs-lookup"><span data-stu-id="aa96f-123">string</span></span>  | <span data-ttu-id="aa96f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa96f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa96f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa96f-126">Request body</span></span>
<span data-ttu-id="aa96f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa96f-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="aa96f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa96f-128">Response</span></span>
<span data-ttu-id="aa96f-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="aa96f-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aa96f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="aa96f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa96f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa96f-131">Request</span></span>
<span data-ttu-id="aa96f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa96f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa96f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa96f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="c"></a>[<span data-ttu-id="aa96f-134">C#</span><span class="sxs-lookup"><span data-stu-id="aa96f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa96f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa96f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa96f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa96f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa96f-137">Java</span><span class="sxs-lookup"><span data-stu-id="aa96f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-synchronizationprofile-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aa96f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa96f-138">Response</span></span>

<span data-ttu-id="aa96f-139">Тело ответа не существует.</span><span class="sxs-lookup"><span data-stu-id="aa96f-139">There is no response body.</span></span>

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


