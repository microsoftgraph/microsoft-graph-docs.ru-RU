---
title: Возобновление синхронизации в Едукатионсинчронизатионпрофиле
description: Возобновление синхронизации конкретного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e6cc5739ff0c1ec270c6bf19bb30731cddd4de53
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965838"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="6313e-103">Возобновление синхронизации в Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="6313e-103">Resume sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="6313e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6313e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6313e-105">Возобновление синхронизации конкретного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6313e-105">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="6313e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6313e-106">Permissions</span></span>
<span data-ttu-id="6313e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6313e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6313e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6313e-109">Permission type</span></span> | <span data-ttu-id="6313e-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6313e-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="6313e-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6313e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6313e-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6313e-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="6313e-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6313e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6313e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6313e-114">Not supported.</span></span>|
|<span data-ttu-id="6313e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6313e-115">Application</span></span>|<span data-ttu-id="6313e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6313e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6313e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6313e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="6313e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6313e-118">Request headers</span></span>
| <span data-ttu-id="6313e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6313e-119">Name</span></span>       | <span data-ttu-id="6313e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="6313e-120">Type</span></span> | <span data-ttu-id="6313e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6313e-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6313e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6313e-122">Authorization</span></span>  | <span data-ttu-id="6313e-123">string</span><span class="sxs-lookup"><span data-stu-id="6313e-123">string</span></span>  | <span data-ttu-id="6313e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6313e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6313e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6313e-126">Request body</span></span>
<span data-ttu-id="6313e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6313e-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6313e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6313e-128">Response</span></span>
<span data-ttu-id="6313e-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="6313e-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6313e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6313e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6313e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6313e-131">Request</span></span>
<span data-ttu-id="6313e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6313e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6313e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6313e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```
# <a name="c"></a>[<span data-ttu-id="6313e-134">C#</span><span class="sxs-lookup"><span data-stu-id="6313e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-resume-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6313e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6313e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-resume-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6313e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6313e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-resume-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6313e-137">Java</span><span class="sxs-lookup"><span data-stu-id="6313e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-resume-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6313e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6313e-138">Response</span></span>

<span data-ttu-id="6313e-139">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="6313e-139">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
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


