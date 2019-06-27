---
title: Удаление Едукатионсинчронизатионпрофиле
description: Удалите профиль School Data Synchronization в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 79f84dceed52fd4d9fde269be577b826d371255a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259487"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="9607b-103">Удаление Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="9607b-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9607b-104">Удалите профиль School Data [Synchronization](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="9607b-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="9607b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9607b-105">Permissions</span></span>
<span data-ttu-id="9607b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9607b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9607b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9607b-108">Permission type</span></span> | <span data-ttu-id="9607b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9607b-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9607b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9607b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9607b-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9607b-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9607b-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9607b-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9607b-113">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9607b-113">Request headers</span></span>
| <span data-ttu-id="9607b-114">Имя</span><span class="sxs-lookup"><span data-stu-id="9607b-114">Name</span></span>       | <span data-ttu-id="9607b-115">Тип</span><span class="sxs-lookup"><span data-stu-id="9607b-115">Type</span></span> | <span data-ttu-id="9607b-116">Описание</span><span class="sxs-lookup"><span data-stu-id="9607b-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9607b-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="9607b-117">Authorization</span></span>  | <span data-ttu-id="9607b-118">string</span><span class="sxs-lookup"><span data-stu-id="9607b-118">string</span></span>  | <span data-ttu-id="9607b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9607b-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="9607b-121">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9607b-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9607b-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9607b-122">Not supported.</span></span>|
|<span data-ttu-id="9607b-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9607b-123">Application</span></span>|<span data-ttu-id="9607b-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9607b-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9607b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9607b-125">Request body</span></span>
<span data-ttu-id="9607b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9607b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9607b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9607b-127">Response</span></span>
<span data-ttu-id="9607b-128">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="9607b-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="9607b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9607b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9607b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9607b-130">Request</span></span>
<span data-ttu-id="9607b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9607b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="9607b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9607b-132">Response</span></span>
<span data-ttu-id="9607b-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9607b-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9607b-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="9607b-134">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9607b-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="9607b-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationProfile-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="9607b-136">C#</span><span class="sxs-lookup"><span data-stu-id="9607b-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationProfile-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9607b-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9607b-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_synchronizationProfile-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
