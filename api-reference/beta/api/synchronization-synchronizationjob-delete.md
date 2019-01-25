---
title: Удаление synchronizationJob
description: Остановить задание синхронизации и окончательно удалить все состояния, связанные с ним. Синхронизированные учетные записи остаются-является.
localization_priority: Normal
ms.openlocfilehash: 29083413c5b24a5ed07b671adfa048f58d437f0d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521686"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="4bb6d-104">Удаление synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="4bb6d-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bb6d-105">Остановить задание синхронизации и окончательно удалить все состояния, связанные с ним.</span><span class="sxs-lookup"><span data-stu-id="4bb6d-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="4bb6d-106">Синхронизированные учетные записи остаются-является.</span><span class="sxs-lookup"><span data-stu-id="4bb6d-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bb6d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bb6d-107">Permissions</span></span>
<span data-ttu-id="4bb6d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bb6d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bb6d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bb6d-110">Permission type</span></span>                        | <span data-ttu-id="4bb6d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bb6d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bb6d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bb6d-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="4bb6d-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bb6d-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4bb6d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bb6d-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4bb6d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb6d-115">Not supported.</span></span>  |
|<span data-ttu-id="4bb6d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bb6d-116">Application</span></span>                            |<span data-ttu-id="4bb6d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb6d-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4bb6d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bb6d-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="4bb6d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bb6d-119">Request headers</span></span>

| <span data-ttu-id="4bb6d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4bb6d-120">Name</span></span>           | <span data-ttu-id="4bb6d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4bb6d-121">Type</span></span>    | <span data-ttu-id="4bb6d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb6d-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4bb6d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bb6d-123">Authorization</span></span>  | <span data-ttu-id="4bb6d-124">string</span><span class="sxs-lookup"><span data-stu-id="4bb6d-124">string</span></span>  | <span data-ttu-id="4bb6d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bb6d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bb6d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bb6d-127">Request body</span></span>

<span data-ttu-id="4bb6d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4bb6d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bb6d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bb6d-129">Response</span></span>

<span data-ttu-id="4bb6d-130">В случае успеха возвращает `204 No Content` ответа.</span><span class="sxs-lookup"><span data-stu-id="4bb6d-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="4bb6d-131">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4bb6d-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bb6d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4bb6d-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4bb6d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bb6d-133">Request</span></span>
<span data-ttu-id="4bb6d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bb6d-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="4bb6d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bb6d-135">Response</span></span>
<span data-ttu-id="4bb6d-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4bb6d-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
