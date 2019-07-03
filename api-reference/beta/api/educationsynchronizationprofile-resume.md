---
title: Возобновление синхронизации в Едукатионсинчронизатионпрофиле
description: Возобновление синхронизации конкретного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: fc442cda70e2ed1e6adac6bc1764ba8afc9b3fb5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441291"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="f9f8d-103">Возобновление синхронизации в Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="f9f8d-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9f8d-104">Возобновление синхронизации конкретного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9f8d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9f8d-105">Permissions</span></span>
<span data-ttu-id="f9f8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9f8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9f8d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9f8d-108">Permission type</span></span> | <span data-ttu-id="f9f8d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9f8d-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f9f8d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f9f8d-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9f8d-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f9f8d-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9f8d-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f9f8d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-113">Not supported.</span></span>|
|<span data-ttu-id="f9f8d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9f8d-114">Application</span></span>|<span data-ttu-id="f9f8d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9f8d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9f8d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="f9f8d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9f8d-117">Request headers</span></span>
| <span data-ttu-id="f9f8d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f9f8d-118">Name</span></span>       | <span data-ttu-id="f9f8d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f9f8d-119">Type</span></span> | <span data-ttu-id="f9f8d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f9f8d-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f9f8d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9f8d-121">Authorization</span></span>  | <span data-ttu-id="f9f8d-122">string</span><span class="sxs-lookup"><span data-stu-id="f9f8d-122">string</span></span>  | <span data-ttu-id="f9f8d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9f8d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9f8d-125">Request body</span></span>
<span data-ttu-id="f9f8d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f9f8d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9f8d-127">Response</span></span>
<span data-ttu-id="f9f8d-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9f8d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f9f8d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9f8d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9f8d-130">Request</span></span>
<span data-ttu-id="f9f8d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f9f8d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9f8d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9f8d-133">C#</span><span class="sxs-lookup"><span data-stu-id="f9f8d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-resume-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9f8d-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="f9f8d-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-resume-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9f8d-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f9f8d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-resume-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f9f8d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9f8d-136">Response</span></span>

<span data-ttu-id="f9f8d-137">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="f9f8d-137">There is no response body.</span></span>

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
