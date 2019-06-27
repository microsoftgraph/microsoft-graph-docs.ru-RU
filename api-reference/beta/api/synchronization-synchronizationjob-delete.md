---
title: Удаление Синчронизатионжоб
description: Остановите задание синхронизации и окончательно удалите все связанные с ним состояния. Синхронизированные учетные записи остаются недоступными.
localization_priority: Normal
ms.openlocfilehash: 0a37be6a9a31c5844071d7c5e1013cd4ce693878
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271416"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="457e3-104">Удаление Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="457e3-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="457e3-105">Остановите задание синхронизации и окончательно удалите все связанные с ним состояния.</span><span class="sxs-lookup"><span data-stu-id="457e3-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="457e3-106">Синхронизированные учетные записи остаются недоступными.</span><span class="sxs-lookup"><span data-stu-id="457e3-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="457e3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="457e3-107">Permissions</span></span>
<span data-ttu-id="457e3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="457e3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="457e3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="457e3-110">Permission type</span></span>                        | <span data-ttu-id="457e3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="457e3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="457e3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="457e3-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="457e3-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457e3-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="457e3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="457e3-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="457e3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="457e3-115">Not supported.</span></span>  |
|<span data-ttu-id="457e3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="457e3-116">Application</span></span>                            |<span data-ttu-id="457e3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="457e3-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="457e3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="457e3-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="457e3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="457e3-119">Request headers</span></span>

| <span data-ttu-id="457e3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="457e3-120">Name</span></span>           | <span data-ttu-id="457e3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="457e3-121">Type</span></span>    | <span data-ttu-id="457e3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="457e3-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="457e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="457e3-123">Authorization</span></span>  | <span data-ttu-id="457e3-124">string</span><span class="sxs-lookup"><span data-stu-id="457e3-124">string</span></span>  | <span data-ttu-id="457e3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="457e3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="457e3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="457e3-127">Request body</span></span>

<span data-ttu-id="457e3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="457e3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="457e3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="457e3-129">Response</span></span>

<span data-ttu-id="457e3-130">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="457e3-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="457e3-131">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="457e3-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="457e3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="457e3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="457e3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="457e3-133">Request</span></span>
<span data-ttu-id="457e3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="457e3-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="457e3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="457e3-135">Response</span></span>
<span data-ttu-id="457e3-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="457e3-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="457e3-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="457e3-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="457e3-138">C#</span><span class="sxs-lookup"><span data-stu-id="457e3-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_synchronizationjob-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="457e3-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="457e3-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_synchronizationjob-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="457e3-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="457e3-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_synchronizationjob-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
