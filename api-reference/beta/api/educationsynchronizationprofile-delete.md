---
title: Удаление Едукатионсинчронизатионпрофиле
description: Удалите профиль School Data Synchronization в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cc5b5230265bfaee468735fb06380652520afdd3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441333"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="9cb27-103">Удаление Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="9cb27-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cb27-104">Удалите профиль School Data [Synchronization](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="9cb27-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cb27-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9cb27-105">Permissions</span></span>
<span data-ttu-id="9cb27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cb27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cb27-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cb27-108">Permission type</span></span> | <span data-ttu-id="9cb27-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9cb27-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9cb27-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cb27-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9cb27-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cb27-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cb27-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cb27-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9cb27-113">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cb27-113">Request headers</span></span>
| <span data-ttu-id="9cb27-114">Имя</span><span class="sxs-lookup"><span data-stu-id="9cb27-114">Name</span></span>       | <span data-ttu-id="9cb27-115">Тип</span><span class="sxs-lookup"><span data-stu-id="9cb27-115">Type</span></span> | <span data-ttu-id="9cb27-116">Описание</span><span class="sxs-lookup"><span data-stu-id="9cb27-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9cb27-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cb27-117">Authorization</span></span>  | <span data-ttu-id="9cb27-118">string</span><span class="sxs-lookup"><span data-stu-id="9cb27-118">string</span></span>  | <span data-ttu-id="9cb27-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cb27-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="9cb27-121">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cb27-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9cb27-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cb27-122">Not supported.</span></span>|
|<span data-ttu-id="9cb27-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cb27-123">Application</span></span>|<span data-ttu-id="9cb27-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cb27-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cb27-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9cb27-125">Request body</span></span>
<span data-ttu-id="9cb27-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9cb27-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9cb27-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cb27-127">Response</span></span>
<span data-ttu-id="9cb27-128">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="9cb27-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cb27-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9cb27-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cb27-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cb27-130">Request</span></span>
<span data-ttu-id="9cb27-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cb27-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9cb27-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cb27-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cb27-133">C#</span><span class="sxs-lookup"><span data-stu-id="9cb27-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cb27-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="9cb27-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cb27-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9cb27-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9cb27-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cb27-136">Response</span></span>
<span data-ttu-id="9cb27-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9cb27-137">Here is an example of the response.</span></span>
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
