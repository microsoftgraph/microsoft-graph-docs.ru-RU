---
title: Возобновление синхронизации в Едукатионсинчронизатионпрофиле
description: Возобновление синхронизации конкретного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 83007ef7a38189f6b50d286940af7e6c287700f8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259509"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="036b1-103">Возобновление синхронизации в Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="036b1-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="036b1-104">Возобновление синхронизации конкретного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="036b1-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="036b1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="036b1-105">Permissions</span></span>
<span data-ttu-id="036b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="036b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="036b1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="036b1-108">Permission type</span></span> | <span data-ttu-id="036b1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="036b1-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="036b1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="036b1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="036b1-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="036b1-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="036b1-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="036b1-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="036b1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="036b1-113">Not supported.</span></span>|
|<span data-ttu-id="036b1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="036b1-114">Application</span></span>|<span data-ttu-id="036b1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="036b1-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="036b1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="036b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="036b1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="036b1-117">Request headers</span></span>
| <span data-ttu-id="036b1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="036b1-118">Name</span></span>       | <span data-ttu-id="036b1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="036b1-119">Type</span></span> | <span data-ttu-id="036b1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="036b1-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="036b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="036b1-121">Authorization</span></span>  | <span data-ttu-id="036b1-122">string</span><span class="sxs-lookup"><span data-stu-id="036b1-122">string</span></span>  | <span data-ttu-id="036b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="036b1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="036b1-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="036b1-125">Request body</span></span>
<span data-ttu-id="036b1-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="036b1-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="036b1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="036b1-127">Response</span></span>
<span data-ttu-id="036b1-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="036b1-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="036b1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="036b1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="036b1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="036b1-130">Request</span></span>
<span data-ttu-id="036b1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="036b1-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="036b1-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="036b1-132">Response</span></span>

<span data-ttu-id="036b1-133">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="036b1-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="036b1-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="036b1-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="036b1-135">C#</span><span class="sxs-lookup"><span data-stu-id="036b1-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_resume-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="036b1-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="036b1-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_resume-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="036b1-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="036b1-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_resume-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
