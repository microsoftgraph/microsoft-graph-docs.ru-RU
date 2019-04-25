---
title: Удаление Синчронизатионжоб
description: Остановите задание синхронизации и окончательно удалите все связанные с ним состояния. Синхронизированные учетные записи остаются недоступными.
localization_priority: Normal
ms.openlocfilehash: 29083413c5b24a5ed07b671adfa048f58d437f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545230"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="536bc-104">Удаление Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="536bc-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="536bc-105">Остановите задание синхронизации и окончательно удалите все связанные с ним состояния.</span><span class="sxs-lookup"><span data-stu-id="536bc-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="536bc-106">Синхронизированные учетные записи остаются недоступными.</span><span class="sxs-lookup"><span data-stu-id="536bc-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="536bc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="536bc-107">Permissions</span></span>
<span data-ttu-id="536bc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="536bc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="536bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="536bc-110">Permission type</span></span>                        | <span data-ttu-id="536bc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="536bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="536bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="536bc-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="536bc-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="536bc-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="536bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="536bc-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="536bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="536bc-115">Not supported.</span></span>  |
|<span data-ttu-id="536bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="536bc-116">Application</span></span>                            |<span data-ttu-id="536bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="536bc-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="536bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="536bc-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="536bc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="536bc-119">Request headers</span></span>

| <span data-ttu-id="536bc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="536bc-120">Name</span></span>           | <span data-ttu-id="536bc-121">Тип</span><span class="sxs-lookup"><span data-stu-id="536bc-121">Type</span></span>    | <span data-ttu-id="536bc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="536bc-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="536bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="536bc-123">Authorization</span></span>  | <span data-ttu-id="536bc-124">string</span><span class="sxs-lookup"><span data-stu-id="536bc-124">string</span></span>  | <span data-ttu-id="536bc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="536bc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="536bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="536bc-127">Request body</span></span>

<span data-ttu-id="536bc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="536bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="536bc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="536bc-129">Response</span></span>

<span data-ttu-id="536bc-130">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="536bc-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="536bc-131">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="536bc-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="536bc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="536bc-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="536bc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="536bc-133">Request</span></span>
<span data-ttu-id="536bc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="536bc-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="536bc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="536bc-135">Response</span></span>
<span data-ttu-id="536bc-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="536bc-136">The following is an example of the response.</span></span> 

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
