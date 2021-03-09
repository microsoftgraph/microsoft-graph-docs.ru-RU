---
title: Удаление educationSynchronizationProfile
description: Удаление профиля синхронизации школьных данных в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2cc7d03b406888022fc8bab935af2b5118357c0c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574288"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="04495-103">Удаление educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="04495-103">Delete a educationSynchronizationProfile</span></span>

<span data-ttu-id="04495-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04495-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04495-105">Удаление профиля [синхронизации школьных данных](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="04495-105">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="04495-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04495-106">Permissions</span></span>
<span data-ttu-id="04495-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04495-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04495-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04495-109">Permission type</span></span> | <span data-ttu-id="04495-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04495-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="04495-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04495-111">Delegated (work or school account)</span></span> | <span data-ttu-id="04495-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04495-112">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="04495-113">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04495-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="04495-114">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04495-114">Request headers</span></span>
| <span data-ttu-id="04495-115">Имя</span><span class="sxs-lookup"><span data-stu-id="04495-115">Name</span></span>       | <span data-ttu-id="04495-116">Тип</span><span class="sxs-lookup"><span data-stu-id="04495-116">Type</span></span> | <span data-ttu-id="04495-117">Описание</span><span class="sxs-lookup"><span data-stu-id="04495-117">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="04495-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="04495-118">Authorization</span></span>  | <span data-ttu-id="04495-119">string</span><span class="sxs-lookup"><span data-stu-id="04495-119">string</span></span>  | <span data-ttu-id="04495-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04495-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="04495-122">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04495-122">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="04495-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04495-123">Not supported.</span></span>|
|<span data-ttu-id="04495-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04495-124">Application</span></span>|<span data-ttu-id="04495-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04495-125">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04495-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04495-126">Request body</span></span>
<span data-ttu-id="04495-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04495-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="04495-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="04495-128">Response</span></span>
<span data-ttu-id="04495-129">В случае успешной работы этот метод возвращает код `202 Accepted` ответа и не возвращает текст ответа.</span><span class="sxs-lookup"><span data-stu-id="04495-129">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="04495-130">Пример</span><span class="sxs-lookup"><span data-stu-id="04495-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04495-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="04495-131">Request</span></span>
<span data-ttu-id="04495-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04495-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04495-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="04495-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="04495-134">C#</span><span class="sxs-lookup"><span data-stu-id="04495-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04495-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04495-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04495-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04495-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04495-137">Java</span><span class="sxs-lookup"><span data-stu-id="04495-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04495-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="04495-138">Response</span></span>
<span data-ttu-id="04495-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04495-139">Here is an example of the response.</span></span>
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


