---
title: Удаление Едукатионсинчронизатионпрофиле
description: Удалите профиль School Data Synchronization в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5f786bf9c36b09aae4a26d3de317d09d1376fb35
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587042"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="b2a5a-103">Удаление Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="b2a5a-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2a5a-104">Удалите профиль School Data [Synchronization](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="b2a5a-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2a5a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2a5a-105">Permissions</span></span>
<span data-ttu-id="b2a5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2a5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2a5a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2a5a-108">Permission type</span></span> | <span data-ttu-id="b2a5a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2a5a-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="b2a5a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2a5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b2a5a-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2a5a-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2a5a-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2a5a-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b2a5a-113">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2a5a-113">Request headers</span></span>
| <span data-ttu-id="b2a5a-114">Имя</span><span class="sxs-lookup"><span data-stu-id="b2a5a-114">Name</span></span>       | <span data-ttu-id="b2a5a-115">Тип</span><span class="sxs-lookup"><span data-stu-id="b2a5a-115">Type</span></span> | <span data-ttu-id="b2a5a-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b2a5a-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b2a5a-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2a5a-117">Authorization</span></span>  | <span data-ttu-id="b2a5a-118">string</span><span class="sxs-lookup"><span data-stu-id="b2a5a-118">string</span></span>  | <span data-ttu-id="b2a5a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2a5a-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="b2a5a-121">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2a5a-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b2a5a-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2a5a-122">Not supported.</span></span>|
|<span data-ttu-id="b2a5a-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2a5a-123">Application</span></span>|<span data-ttu-id="b2a5a-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2a5a-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2a5a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2a5a-125">Request body</span></span>
<span data-ttu-id="b2a5a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2a5a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b2a5a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2a5a-127">Response</span></span>
<span data-ttu-id="b2a5a-128">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="b2a5a-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2a5a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b2a5a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2a5a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2a5a-130">Request</span></span>
<span data-ttu-id="b2a5a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2a5a-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="b2a5a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2a5a-132">Response</span></span>
<span data-ttu-id="b2a5a-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b2a5a-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b2a5a-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="b2a5a-134">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="b2a5a-135">Языках</span><span class="sxs-lookup"><span data-stu-id="b2a5a-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationProfile-Cs-snippets.md)]

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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
