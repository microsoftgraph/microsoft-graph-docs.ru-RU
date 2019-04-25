---
title: 'Синчронизатионжоб: пауза'
description: Временная остановка синхронизации. Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении начального вызова.
localization_priority: Normal
ms.openlocfilehash: 9f8cac05511b5efd17234ccf16b763999418bf2a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537180"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="03b4f-104">Синчронизатионжоб: пауза</span><span class="sxs-lookup"><span data-stu-id="03b4f-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03b4f-105">Временная остановка синхронизации.</span><span class="sxs-lookup"><span data-stu-id="03b4f-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="03b4f-106">Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="03b4f-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="03b4f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03b4f-107">Permissions</span></span>
<span data-ttu-id="03b4f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03b4f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03b4f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03b4f-110">Permission type</span></span>                        | <span data-ttu-id="03b4f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03b4f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="03b4f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03b4f-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="03b4f-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03b4f-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="03b4f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03b4f-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="03b4f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03b4f-115">Not supported.</span></span>  |
|<span data-ttu-id="03b4f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03b4f-116">Application</span></span>                            |<span data-ttu-id="03b4f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03b4f-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="03b4f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03b4f-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="03b4f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03b4f-119">Request headers</span></span>

| <span data-ttu-id="03b4f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03b4f-120">Name</span></span>           | <span data-ttu-id="03b4f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="03b4f-121">Type</span></span>    | <span data-ttu-id="03b4f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="03b4f-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="03b4f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03b4f-123">Authorization</span></span>  | <span data-ttu-id="03b4f-124">string</span><span class="sxs-lookup"><span data-stu-id="03b4f-124">string</span></span>  | <span data-ttu-id="03b4f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03b4f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03b4f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03b4f-127">Request body</span></span>

<span data-ttu-id="03b4f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03b4f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03b4f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="03b4f-129">Response</span></span>

<span data-ttu-id="03b4f-130">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="03b4f-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="03b4f-131">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="03b4f-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03b4f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="03b4f-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="03b4f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="03b4f-133">Request</span></span>
<span data-ttu-id="03b4f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03b4f-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="03b4f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="03b4f-135">Response</span></span>
<span data-ttu-id="03b4f-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03b4f-136">The following is an example of a response.</span></span>
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
