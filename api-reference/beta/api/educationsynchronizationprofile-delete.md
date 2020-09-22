---
title: Удаление Едукатионсинчронизатионпрофиле
description: Удалите профиль School Data Synchronization в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 39bc4909e63e6e7ff908481873f32324703bf549
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991259"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="9d97a-103">Удаление Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="9d97a-103">Delete a educationSynchronizationProfile</span></span>

<span data-ttu-id="9d97a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d97a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d97a-105">Удалите профиль School Data [Synchronization](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="9d97a-105">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d97a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d97a-106">Permissions</span></span>
<span data-ttu-id="9d97a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d97a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d97a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d97a-109">Permission type</span></span> | <span data-ttu-id="9d97a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d97a-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9d97a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d97a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9d97a-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d97a-112">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d97a-113">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d97a-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9d97a-114">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d97a-114">Request headers</span></span>
| <span data-ttu-id="9d97a-115">Имя</span><span class="sxs-lookup"><span data-stu-id="9d97a-115">Name</span></span>       | <span data-ttu-id="9d97a-116">Тип</span><span class="sxs-lookup"><span data-stu-id="9d97a-116">Type</span></span> | <span data-ttu-id="9d97a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="9d97a-117">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9d97a-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d97a-118">Authorization</span></span>  | <span data-ttu-id="9d97a-119">string</span><span class="sxs-lookup"><span data-stu-id="9d97a-119">string</span></span>  | <span data-ttu-id="9d97a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d97a-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="9d97a-122">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d97a-122">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9d97a-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d97a-123">Not supported.</span></span>|
|<span data-ttu-id="9d97a-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d97a-124">Application</span></span>|<span data-ttu-id="9d97a-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d97a-125">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d97a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d97a-126">Request body</span></span>
<span data-ttu-id="9d97a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d97a-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9d97a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d97a-128">Response</span></span>
<span data-ttu-id="9d97a-129">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="9d97a-129">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d97a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9d97a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d97a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d97a-131">Request</span></span>
<span data-ttu-id="9d97a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d97a-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d97a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d97a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="9d97a-134">C#</span><span class="sxs-lookup"><span data-stu-id="9d97a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d97a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d97a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d97a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d97a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9d97a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d97a-137">Response</span></span>
<span data-ttu-id="9d97a-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9d97a-138">Here is an example of the response.</span></span>
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


