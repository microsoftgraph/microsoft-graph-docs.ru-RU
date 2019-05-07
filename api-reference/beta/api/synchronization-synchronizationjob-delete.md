---
title: Удаление Синчронизатионжоб
description: Остановите задание синхронизации и окончательно удалите все связанные с ним состояния. Синхронизированные учетные записи остаются недоступными.
localization_priority: Normal
ms.openlocfilehash: 5b4d49f9a9a64f4063b11ee8cc14434282b80b02
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638062"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="904f2-104">Удаление Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="904f2-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="904f2-105">Остановите задание синхронизации и окончательно удалите все связанные с ним состояния.</span><span class="sxs-lookup"><span data-stu-id="904f2-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="904f2-106">Синхронизированные учетные записи остаются недоступными.</span><span class="sxs-lookup"><span data-stu-id="904f2-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="904f2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="904f2-107">Permissions</span></span>
<span data-ttu-id="904f2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="904f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="904f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="904f2-110">Permission type</span></span>                        | <span data-ttu-id="904f2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="904f2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="904f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="904f2-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="904f2-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="904f2-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="904f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="904f2-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="904f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="904f2-115">Not supported.</span></span>  |
|<span data-ttu-id="904f2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="904f2-116">Application</span></span>                            |<span data-ttu-id="904f2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="904f2-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="904f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="904f2-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="904f2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="904f2-119">Request headers</span></span>

| <span data-ttu-id="904f2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="904f2-120">Name</span></span>           | <span data-ttu-id="904f2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="904f2-121">Type</span></span>    | <span data-ttu-id="904f2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="904f2-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="904f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="904f2-123">Authorization</span></span>  | <span data-ttu-id="904f2-124">string</span><span class="sxs-lookup"><span data-stu-id="904f2-124">string</span></span>  | <span data-ttu-id="904f2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="904f2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="904f2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="904f2-127">Request body</span></span>

<span data-ttu-id="904f2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="904f2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="904f2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="904f2-129">Response</span></span>

<span data-ttu-id="904f2-130">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="904f2-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="904f2-131">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="904f2-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="904f2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="904f2-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="904f2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="904f2-133">Request</span></span>
<span data-ttu-id="904f2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="904f2-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="904f2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="904f2-135">Response</span></span>
<span data-ttu-id="904f2-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="904f2-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="904f2-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="904f2-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="904f2-138">Языках</span><span class="sxs-lookup"><span data-stu-id="904f2-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_synchronizationjob-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="904f2-139">Язык</span><span class="sxs-lookup"><span data-stu-id="904f2-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_synchronizationjob-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
