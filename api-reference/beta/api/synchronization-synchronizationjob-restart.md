---
title: Перезапустите synchronizationJob
description: Перезапустите задание синхронизации, заставить его повторно обработать все объекты в каталоге. При необходимости удаляет существующие состояние синхронизации и предыдущих ошибок.
localization_priority: Normal
ms.openlocfilehash: 169f95c3662fd774207584b54fcf27fb2548c795
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526727"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="091b4-104">Перезапустите synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="091b4-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="091b4-105">Перезапустите задание синхронизации, заставить его повторно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="091b4-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="091b4-106">При необходимости удаляет существующие состояние синхронизации и предыдущих ошибок.</span><span class="sxs-lookup"><span data-stu-id="091b4-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="091b4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="091b4-107">Permissions</span></span>
<span data-ttu-id="091b4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="091b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="091b4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="091b4-110">Permission type</span></span>                        | <span data-ttu-id="091b4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="091b4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="091b4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="091b4-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="091b4-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="091b4-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="091b4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="091b4-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="091b4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="091b4-115">Not supported.</span></span> |
|<span data-ttu-id="091b4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="091b4-116">Application</span></span>                            |<span data-ttu-id="091b4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="091b4-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="091b4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="091b4-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="091b4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="091b4-119">Request headers</span></span>

| <span data-ttu-id="091b4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="091b4-120">Name</span></span>           | <span data-ttu-id="091b4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="091b4-121">Type</span></span>    | <span data-ttu-id="091b4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="091b4-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="091b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="091b4-123">Authorization</span></span>  | <span data-ttu-id="091b4-124">string</span><span class="sxs-lookup"><span data-stu-id="091b4-124">string</span></span>  | <span data-ttu-id="091b4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="091b4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="091b4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="091b4-127">Request body</span></span>

<span data-ttu-id="091b4-128">Предоставить объект JSON в тексте запроса следующий параметр.</span><span class="sxs-lookup"><span data-stu-id="091b4-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="091b4-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="091b4-129">Parameter</span></span>     | <span data-ttu-id="091b4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="091b4-130">Type</span></span>      | <span data-ttu-id="091b4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="091b4-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="091b4-132">criteria</span><span class="sxs-lookup"><span data-stu-id="091b4-132">criteria</span></span>       |[<span data-ttu-id="091b4-133">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="091b4-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="091b4-134">Перезапустите критериев</span><span class="sxs-lookup"><span data-stu-id="091b4-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="091b4-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="091b4-135">Response</span></span>

<span data-ttu-id="091b4-136">В случае успеха возвращает `204 No Content` ответа.</span><span class="sxs-lookup"><span data-stu-id="091b4-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="091b4-137">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="091b4-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="091b4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="091b4-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="091b4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="091b4-139">Request</span></span>
<span data-ttu-id="091b4-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="091b4-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_restart"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
Authorization: Bearer <token>
Content-type: application/json

{
   "criteria": {
       "resetScope": "ConnectorDataStore, Escrows, QuarantineState"
   }
}
```

##### <a name="response"></a><span data-ttu-id="091b4-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="091b4-141">Response</span></span>
<span data-ttu-id="091b4-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="091b4-142">The following is an example of a response.</span></span>

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
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
