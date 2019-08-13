---
title: Удаление Едукатионсинчронизатионпрофиле
description: Удалите профиль School Data Synchronization в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2c766abb5b4336e1b3f7c7f581ce945a4af76455
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323908"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="ca8a9-103">Удаление Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="ca8a9-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca8a9-104">Удалите профиль School Data [Synchronization](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="ca8a9-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca8a9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca8a9-105">Permissions</span></span>
<span data-ttu-id="ca8a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca8a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca8a9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca8a9-108">Permission type</span></span> | <span data-ttu-id="ca8a9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca8a9-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ca8a9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca8a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ca8a9-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca8a9-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca8a9-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca8a9-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ca8a9-113">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca8a9-113">Request headers</span></span>
| <span data-ttu-id="ca8a9-114">Имя</span><span class="sxs-lookup"><span data-stu-id="ca8a9-114">Name</span></span>       | <span data-ttu-id="ca8a9-115">Тип</span><span class="sxs-lookup"><span data-stu-id="ca8a9-115">Type</span></span> | <span data-ttu-id="ca8a9-116">Описание</span><span class="sxs-lookup"><span data-stu-id="ca8a9-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ca8a9-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca8a9-117">Authorization</span></span>  | <span data-ttu-id="ca8a9-118">string</span><span class="sxs-lookup"><span data-stu-id="ca8a9-118">string</span></span>  | <span data-ttu-id="ca8a9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca8a9-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="ca8a9-121">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca8a9-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ca8a9-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca8a9-122">Not supported.</span></span>|
|<span data-ttu-id="ca8a9-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca8a9-123">Application</span></span>|<span data-ttu-id="ca8a9-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca8a9-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca8a9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca8a9-125">Request body</span></span>
<span data-ttu-id="ca8a9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca8a9-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ca8a9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca8a9-127">Response</span></span>
<span data-ttu-id="ca8a9-128">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="ca8a9-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca8a9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ca8a9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca8a9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca8a9-130">Request</span></span>
<span data-ttu-id="ca8a9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca8a9-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ca8a9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca8a9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ca8a9-133">C#</span><span class="sxs-lookup"><span data-stu-id="ca8a9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ca8a9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca8a9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ca8a9-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ca8a9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ca8a9-136">Java</span><span class="sxs-lookup"><span data-stu-id="ca8a9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ca8a9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca8a9-137">Response</span></span>
<span data-ttu-id="ca8a9-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca8a9-138">Here is an example of the response.</span></span>
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
