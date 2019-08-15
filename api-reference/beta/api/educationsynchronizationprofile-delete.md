---
title: Удаление Едукатионсинчронизатионпрофиле
description: Удалите профиль School Data Synchronization в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a2230d8bc88bfdba6f014c9b78cbdc7f519f075d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416018"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="4c063-103">Удаление Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="4c063-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c063-104">Удалите профиль School Data [Synchronization](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="4c063-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c063-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c063-105">Permissions</span></span>
<span data-ttu-id="4c063-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c063-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c063-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c063-108">Permission type</span></span> | <span data-ttu-id="4c063-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c063-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4c063-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c063-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c063-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c063-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c063-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c063-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c063-113">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c063-113">Request headers</span></span>
| <span data-ttu-id="4c063-114">Имя</span><span class="sxs-lookup"><span data-stu-id="4c063-114">Name</span></span>       | <span data-ttu-id="4c063-115">Тип</span><span class="sxs-lookup"><span data-stu-id="4c063-115">Type</span></span> | <span data-ttu-id="4c063-116">Описание</span><span class="sxs-lookup"><span data-stu-id="4c063-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4c063-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c063-117">Authorization</span></span>  | <span data-ttu-id="4c063-118">string</span><span class="sxs-lookup"><span data-stu-id="4c063-118">string</span></span>  | <span data-ttu-id="4c063-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c063-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="4c063-121">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c063-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4c063-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c063-122">Not supported.</span></span>|
|<span data-ttu-id="4c063-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c063-123">Application</span></span>|<span data-ttu-id="4c063-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c063-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c063-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c063-125">Request body</span></span>
<span data-ttu-id="4c063-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c063-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4c063-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c063-127">Response</span></span>
<span data-ttu-id="4c063-128">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="4c063-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c063-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4c063-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c063-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c063-130">Request</span></span>
<span data-ttu-id="4c063-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c063-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4c063-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c063-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c063-133">C#</span><span class="sxs-lookup"><span data-stu-id="4c063-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c063-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c063-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c063-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4c063-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4c063-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c063-136">Response</span></span>
<span data-ttu-id="4c063-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c063-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
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
