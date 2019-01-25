---
title: 'synchronizationJob: Приостановка'
description: Временно приостановить синхронизации. Сохраняются все текущие, включая состояние задания и задание продолжит работу с где остановились при вызове Пуск.
localization_priority: Normal
ms.openlocfilehash: 9f8cac05511b5efd17234ccf16b763999418bf2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513923"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="eb9d3-104">synchronizationJob: Приостановка</span><span class="sxs-lookup"><span data-stu-id="eb9d3-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb9d3-105">Временно приостановить синхронизации.</span><span class="sxs-lookup"><span data-stu-id="eb9d3-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="eb9d3-106">Сохраняются все текущие, включая состояние задания и задание продолжит работу с где оно было прервано Если [запустить](../api/synchronization-synchronizationjob-start.md) вызов.</span><span class="sxs-lookup"><span data-stu-id="eb9d3-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb9d3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb9d3-107">Permissions</span></span>
<span data-ttu-id="eb9d3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb9d3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb9d3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb9d3-110">Permission type</span></span>                        | <span data-ttu-id="eb9d3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb9d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb9d3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb9d3-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="eb9d3-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb9d3-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="eb9d3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb9d3-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="eb9d3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb9d3-115">Not supported.</span></span>  |
|<span data-ttu-id="eb9d3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb9d3-116">Application</span></span>                            |<span data-ttu-id="eb9d3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb9d3-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="eb9d3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb9d3-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="eb9d3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb9d3-119">Request headers</span></span>

| <span data-ttu-id="eb9d3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="eb9d3-120">Name</span></span>           | <span data-ttu-id="eb9d3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="eb9d3-121">Type</span></span>    | <span data-ttu-id="eb9d3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eb9d3-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="eb9d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb9d3-123">Authorization</span></span>  | <span data-ttu-id="eb9d3-124">string</span><span class="sxs-lookup"><span data-stu-id="eb9d3-124">string</span></span>  | <span data-ttu-id="eb9d3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb9d3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb9d3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb9d3-127">Request body</span></span>

<span data-ttu-id="eb9d3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb9d3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb9d3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb9d3-129">Response</span></span>

<span data-ttu-id="eb9d3-130">В случае успеха возвращает `204 No Content` ответа.</span><span class="sxs-lookup"><span data-stu-id="eb9d3-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="eb9d3-131">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="eb9d3-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb9d3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="eb9d3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eb9d3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb9d3-133">Request</span></span>
<span data-ttu-id="eb9d3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb9d3-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="eb9d3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb9d3-135">Response</span></span>
<span data-ttu-id="eb9d3-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="eb9d3-136">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-pause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
