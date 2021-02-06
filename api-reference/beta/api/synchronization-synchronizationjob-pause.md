---
title: 'synchronizationJob: pause'
description: Временно остановите синхронизацию. Все ходы выполнения, включая состояние задания, сохраняются, и задание продолжит работу с того места, где оно было отключено при запуске вызова.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: eba89e688b8dc9ea02fee633ee4beeb40bb55106
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137492"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="802a9-104">synchronizationJob: pause</span><span class="sxs-lookup"><span data-stu-id="802a9-104">synchronizationJob: pause</span></span>

<span data-ttu-id="802a9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="802a9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="802a9-106">Временно остановите синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="802a9-106">Temporarily stop synchronization.</span></span> <span data-ttu-id="802a9-107">Все ходы выполнения, включая состояние задания, сохраняются, и задание продолжит работу с того места, где оно было отключено при [запуске](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="802a9-107">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="802a9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="802a9-108">Permissions</span></span>
<span data-ttu-id="802a9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="802a9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="802a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="802a9-111">Permission type</span></span>                        | <span data-ttu-id="802a9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="802a9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="802a9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="802a9-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="802a9-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="802a9-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="802a9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="802a9-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="802a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="802a9-116">Not supported.</span></span>  |
|<span data-ttu-id="802a9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="802a9-117">Application</span></span>                            |<span data-ttu-id="802a9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="802a9-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="802a9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="802a9-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="802a9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="802a9-120">Request headers</span></span>

| <span data-ttu-id="802a9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="802a9-121">Name</span></span>           | <span data-ttu-id="802a9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="802a9-122">Type</span></span>    | <span data-ttu-id="802a9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="802a9-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="802a9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="802a9-124">Authorization</span></span>  | <span data-ttu-id="802a9-125">string</span><span class="sxs-lookup"><span data-stu-id="802a9-125">string</span></span>  | <span data-ttu-id="802a9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="802a9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="802a9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="802a9-128">Request body</span></span>

<span data-ttu-id="802a9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="802a9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="802a9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="802a9-130">Response</span></span>

<span data-ttu-id="802a9-131">В случае успеха возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="802a9-131">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="802a9-132">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="802a9-132">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="802a9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="802a9-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="802a9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="802a9-134">Request</span></span>
<span data-ttu-id="802a9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="802a9-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="802a9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="802a9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```
# <a name="c"></a>[<span data-ttu-id="802a9-137">C#</span><span class="sxs-lookup"><span data-stu-id="802a9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="802a9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="802a9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="802a9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="802a9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="802a9-140">Java</span><span class="sxs-lookup"><span data-stu-id="802a9-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="802a9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="802a9-141">Response</span></span>
<span data-ttu-id="802a9-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="802a9-142">The following is an example of a response.</span></span>
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
  ]
}
-->


