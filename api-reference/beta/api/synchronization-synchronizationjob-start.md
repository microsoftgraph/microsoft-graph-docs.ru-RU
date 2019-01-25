---
title: Запустите synchronizationJob
description: Запустите существующее задание синхронизации. Если задание находится в приостановленном состоянии, он будет предоставляться обработки изменений из точки, где он был приостановлен. Если задание находится в карантине, будут очищены состояние карантина.
localization_priority: Normal
ms.openlocfilehash: 4648d9d3d889adf2cd7ec06e4fcf79b761c77132
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515372"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="3150d-105">Запустите synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3150d-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3150d-106">Запустите существующее задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="3150d-106">Start an existing synchronization job.</span></span> <span data-ttu-id="3150d-107">Если задание находится в приостановленном состоянии, он будет предоставляться обработки изменений из точки, где он был приостановлен.</span><span class="sxs-lookup"><span data-stu-id="3150d-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="3150d-108">Если задание находится в карантине, будут очищены состояние карантина.</span><span class="sxs-lookup"><span data-stu-id="3150d-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="3150d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3150d-109">Permissions</span></span>
<span data-ttu-id="3150d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3150d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3150d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3150d-112">Permission type</span></span>                        | <span data-ttu-id="3150d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3150d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3150d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3150d-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="3150d-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3150d-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3150d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3150d-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3150d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3150d-117">Not supported.</span></span> |
|<span data-ttu-id="3150d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3150d-118">Application</span></span>                            |<span data-ttu-id="3150d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3150d-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3150d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3150d-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="3150d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3150d-121">Request headers</span></span>

| <span data-ttu-id="3150d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3150d-122">Name</span></span>           | <span data-ttu-id="3150d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3150d-123">Type</span></span>    | <span data-ttu-id="3150d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3150d-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3150d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3150d-125">Authorization</span></span>  | <span data-ttu-id="3150d-126">string</span><span class="sxs-lookup"><span data-stu-id="3150d-126">string</span></span>  | <span data-ttu-id="3150d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3150d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3150d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3150d-129">Request body</span></span>

<span data-ttu-id="3150d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3150d-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="3150d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="3150d-131">Response</span></span>

<span data-ttu-id="3150d-132">В случае успеха возвращает `204 No Content` ответа.</span><span class="sxs-lookup"><span data-stu-id="3150d-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="3150d-133">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3150d-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3150d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="3150d-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3150d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3150d-135">Request</span></span>
<span data-ttu-id="3150d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3150d-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="3150d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="3150d-137">Response</span></span>
<span data-ttu-id="3150d-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3150d-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-start.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
