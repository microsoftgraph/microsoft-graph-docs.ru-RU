---
title: Запуск Синчронизатионжоб
description: Запуск существующего задания синхронизации. Если задание приостановлено, оно продолжит обработку изменений с того места, где оно было приостановлено. Если задание находится в карантине, состояние карантина будет очищено.
localization_priority: Normal
ms.openlocfilehash: 4648d9d3d889adf2cd7ec06e4fcf79b761c77132
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545301"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="75944-105">Запуск Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="75944-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75944-106">Запуск существующего задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="75944-106">Start an existing synchronization job.</span></span> <span data-ttu-id="75944-107">Если задание приостановлено, оно продолжит обработку изменений с того места, где оно было приостановлено.</span><span class="sxs-lookup"><span data-stu-id="75944-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="75944-108">Если задание находится в карантине, состояние карантина будет очищено.</span><span class="sxs-lookup"><span data-stu-id="75944-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="75944-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75944-109">Permissions</span></span>
<span data-ttu-id="75944-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75944-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75944-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75944-112">Permission type</span></span>                        | <span data-ttu-id="75944-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75944-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="75944-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75944-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="75944-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75944-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="75944-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75944-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="75944-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75944-117">Not supported.</span></span> |
|<span data-ttu-id="75944-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75944-118">Application</span></span>                            |<span data-ttu-id="75944-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75944-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="75944-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75944-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="75944-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75944-121">Request headers</span></span>

| <span data-ttu-id="75944-122">Имя</span><span class="sxs-lookup"><span data-stu-id="75944-122">Name</span></span>           | <span data-ttu-id="75944-123">Тип</span><span class="sxs-lookup"><span data-stu-id="75944-123">Type</span></span>    | <span data-ttu-id="75944-124">Описание</span><span class="sxs-lookup"><span data-stu-id="75944-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="75944-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="75944-125">Authorization</span></span>  | <span data-ttu-id="75944-126">string</span><span class="sxs-lookup"><span data-stu-id="75944-126">string</span></span>  | <span data-ttu-id="75944-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75944-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75944-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75944-129">Request body</span></span>

<span data-ttu-id="75944-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75944-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="75944-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="75944-131">Response</span></span>

<span data-ttu-id="75944-132">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="75944-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="75944-133">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="75944-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75944-134">Пример</span><span class="sxs-lookup"><span data-stu-id="75944-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="75944-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="75944-135">Request</span></span>
<span data-ttu-id="75944-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75944-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="75944-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="75944-137">Response</span></span>
<span data-ttu-id="75944-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="75944-138">The following is an example of a response.</span></span>
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
