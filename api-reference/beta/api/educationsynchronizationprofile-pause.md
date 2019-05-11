---
title: Приостановка синхронизации в Едукатионсинчронизатионпрофиле
description: Приостановите синхронизацию определенного профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 37593589d4ef789021c7ed19f1f98f12407c1621
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938953"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="249e6-103">Приостановка синхронизации в Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="249e6-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="249e6-104">Приостановите синхронизацию определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="249e6-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="249e6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="249e6-105">Permissions</span></span>
<span data-ttu-id="249e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="249e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="249e6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="249e6-108">Permission type</span></span> | <span data-ttu-id="249e6-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="249e6-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="249e6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="249e6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="249e6-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="249e6-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="249e6-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="249e6-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="249e6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="249e6-113">Not supported.</span></span>|
|<span data-ttu-id="249e6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="249e6-114">Application</span></span>|<span data-ttu-id="249e6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="249e6-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="249e6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="249e6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="249e6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="249e6-117">Request headers</span></span>
| <span data-ttu-id="249e6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="249e6-118">Name</span></span>       | <span data-ttu-id="249e6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="249e6-119">Type</span></span> | <span data-ttu-id="249e6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="249e6-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="249e6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="249e6-121">Authorization</span></span>  | <span data-ttu-id="249e6-122">string</span><span class="sxs-lookup"><span data-stu-id="249e6-122">string</span></span>  | <span data-ttu-id="249e6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="249e6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="249e6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="249e6-125">Request body</span></span>
<span data-ttu-id="249e6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="249e6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="249e6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="249e6-127">Response</span></span>
<span data-ttu-id="249e6-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="249e6-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="249e6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="249e6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="249e6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="249e6-130">Request</span></span>
<span data-ttu-id="249e6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="249e6-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="249e6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="249e6-132">Response</span></span>

<span data-ttu-id="249e6-133">Текст отклика отсутствует.</span><span class="sxs-lookup"><span data-stu-id="249e6-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```http
HTTP/1.1 200 OK
```

#### <a name="sdk-sample-code"></a><span data-ttu-id="249e6-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="249e6-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="249e6-135">C#</span><span class="sxs-lookup"><span data-stu-id="249e6-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_synchronizationProfile_pause-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="249e6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="249e6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_synchronizationProfile_pause-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
