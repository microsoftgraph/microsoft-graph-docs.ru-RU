---
title: Удаление Едукатионсинчронизатионпрофиле
description: Удалите профиль School Data Synchronization в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 89dd57e3188a63e87ed88f796b3f7259e7996661
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424535"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="4dc62-103">Удаление Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="4dc62-103">Delete a educationSynchronizationProfile</span></span>

<span data-ttu-id="4dc62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dc62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dc62-105">Удалите профиль School Data [Synchronization](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="4dc62-105">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="4dc62-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4dc62-106">Permissions</span></span>
<span data-ttu-id="4dc62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dc62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4dc62-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dc62-109">Permission type</span></span> | <span data-ttu-id="4dc62-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4dc62-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4dc62-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dc62-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4dc62-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dc62-112">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dc62-113">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dc62-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4dc62-114">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dc62-114">Request headers</span></span>
| <span data-ttu-id="4dc62-115">Имя</span><span class="sxs-lookup"><span data-stu-id="4dc62-115">Name</span></span>       | <span data-ttu-id="4dc62-116">Тип</span><span class="sxs-lookup"><span data-stu-id="4dc62-116">Type</span></span> | <span data-ttu-id="4dc62-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4dc62-117">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4dc62-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dc62-118">Authorization</span></span>  | <span data-ttu-id="4dc62-119">string</span><span class="sxs-lookup"><span data-stu-id="4dc62-119">string</span></span>  | <span data-ttu-id="4dc62-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dc62-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="4dc62-122">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dc62-122">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4dc62-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dc62-123">Not supported.</span></span>|
|<span data-ttu-id="4dc62-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dc62-124">Application</span></span>|<span data-ttu-id="4dc62-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dc62-125">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dc62-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4dc62-126">Request body</span></span>
<span data-ttu-id="4dc62-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4dc62-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4dc62-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dc62-128">Response</span></span>
<span data-ttu-id="4dc62-129">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="4dc62-129">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dc62-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4dc62-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4dc62-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dc62-131">Request</span></span>
<span data-ttu-id="4dc62-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dc62-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4dc62-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4dc62-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="4dc62-134">C#</span><span class="sxs-lookup"><span data-stu-id="4dc62-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4dc62-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4dc62-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4dc62-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4dc62-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4dc62-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc62-137">Response</span></span>
<span data-ttu-id="4dc62-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4dc62-138">Here is an example of the response.</span></span>
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
