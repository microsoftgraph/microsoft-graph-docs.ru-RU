---
title: Возобновление синхронизации на educationSynchronizationProfile
description: Возобновим синхронизацию определенного профиля синхронизации школьных данных в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d88c4a2e9bf6aa719e4cde333764fe32a29bf285
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574170"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="99927-103">Возобновление синхронизации на educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="99927-103">Resume sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="99927-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99927-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99927-105">Возобновим синхронизацию определенного профиля синхронизации [школьных](../resources/educationsynchronizationprofile.md) данных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="99927-105">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="99927-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99927-106">Permissions</span></span>
<span data-ttu-id="99927-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99927-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99927-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99927-109">Permission type</span></span> | <span data-ttu-id="99927-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99927-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="99927-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99927-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99927-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99927-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="99927-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99927-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="99927-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99927-114">Not supported.</span></span>|
|<span data-ttu-id="99927-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99927-115">Application</span></span>|<span data-ttu-id="99927-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99927-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99927-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99927-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="99927-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99927-118">Request headers</span></span>
| <span data-ttu-id="99927-119">Имя</span><span class="sxs-lookup"><span data-stu-id="99927-119">Name</span></span>       | <span data-ttu-id="99927-120">Тип</span><span class="sxs-lookup"><span data-stu-id="99927-120">Type</span></span> | <span data-ttu-id="99927-121">Описание</span><span class="sxs-lookup"><span data-stu-id="99927-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="99927-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99927-122">Authorization</span></span>  | <span data-ttu-id="99927-123">string</span><span class="sxs-lookup"><span data-stu-id="99927-123">string</span></span>  | <span data-ttu-id="99927-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99927-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99927-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99927-126">Request body</span></span>
<span data-ttu-id="99927-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99927-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="99927-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="99927-128">Response</span></span>
<span data-ttu-id="99927-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="99927-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="99927-130">Пример</span><span class="sxs-lookup"><span data-stu-id="99927-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99927-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="99927-131">Request</span></span>
<span data-ttu-id="99927-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99927-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99927-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="99927-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```
# <a name="c"></a>[<span data-ttu-id="99927-134">C#</span><span class="sxs-lookup"><span data-stu-id="99927-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-resume-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99927-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99927-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-resume-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99927-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99927-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-resume-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99927-137">Java</span><span class="sxs-lookup"><span data-stu-id="99927-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-resume-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="99927-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="99927-138">Response</span></span>

<span data-ttu-id="99927-139">Тело ответа не существует.</span><span class="sxs-lookup"><span data-stu-id="99927-139">There is no response body.</span></span>

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


