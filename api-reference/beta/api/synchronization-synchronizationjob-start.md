---
title: Начните синхронизациюJob
description: Запустите существующее задание синхронизации. Если задание находится в приостановленной работе, она будет продолжать обработку изменений с точки, где она была приостановлена. Если задание находится на карантине, состояние карантина будет очищено.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: fc70f816dfc1e564d27fe5c9be60580eded415e6
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626253"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="71f54-105">Начните синхронизациюJob</span><span class="sxs-lookup"><span data-stu-id="71f54-105">Start synchronizationJob</span></span>

<span data-ttu-id="71f54-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71f54-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71f54-107">Запустите существующее задание синхронизации.</span><span class="sxs-lookup"><span data-stu-id="71f54-107">Start an existing synchronization job.</span></span> <span data-ttu-id="71f54-108">Если задание находится в приостановленной работе, она будет продолжать обработку изменений с точки, где она была приостановлена.</span><span class="sxs-lookup"><span data-stu-id="71f54-108">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="71f54-109">Если задание находится на карантине, состояние карантина будет очищено.</span><span class="sxs-lookup"><span data-stu-id="71f54-109">If the job is in quarantine, the quarantine status will be cleared.</span></span> <span data-ttu-id="71f54-110">Не создавайте скрипты для непрерывного вызова задания запуска во время его работы, так как это может привести к остановке работы службы.</span><span class="sxs-lookup"><span data-stu-id="71f54-110">Do not create scripts to call the start job continuously while it's running because that can cause the service to stop running.</span></span> <span data-ttu-id="71f54-111">Используйте начните работу только в том случае, если задание приостановлено или находится на карантине.</span><span class="sxs-lookup"><span data-stu-id="71f54-111">Use the start job only when the job is currently paused or in quarantine.</span></span> 

## <a name="permissions"></a><span data-ttu-id="71f54-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71f54-112">Permissions</span></span>
<span data-ttu-id="71f54-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71f54-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71f54-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71f54-115">Permission type</span></span>                        | <span data-ttu-id="71f54-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71f54-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="71f54-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71f54-117">Delegated (work or school account)</span></span>     |<span data-ttu-id="71f54-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71f54-118">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="71f54-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71f54-119">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="71f54-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71f54-120">Not supported.</span></span> |
|<span data-ttu-id="71f54-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="71f54-121">Application</span></span>                            |<span data-ttu-id="71f54-122">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71f54-122">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="71f54-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71f54-123">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="71f54-124">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="71f54-124">Request headers</span></span>

| <span data-ttu-id="71f54-125">Имя</span><span class="sxs-lookup"><span data-stu-id="71f54-125">Name</span></span>           | <span data-ttu-id="71f54-126">Тип</span><span class="sxs-lookup"><span data-stu-id="71f54-126">Type</span></span>    | <span data-ttu-id="71f54-127">Описание</span><span class="sxs-lookup"><span data-stu-id="71f54-127">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="71f54-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="71f54-128">Authorization</span></span>  | <span data-ttu-id="71f54-129">string</span><span class="sxs-lookup"><span data-stu-id="71f54-129">string</span></span>  | <span data-ttu-id="71f54-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71f54-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71f54-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71f54-132">Request body</span></span>

<span data-ttu-id="71f54-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71f54-133">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="71f54-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="71f54-134">Response</span></span>

<span data-ttu-id="71f54-135">В случае успешного ответа `204 No Content` возвращается ответ.</span><span class="sxs-lookup"><span data-stu-id="71f54-135">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="71f54-136">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71f54-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71f54-137">Пример</span><span class="sxs-lookup"><span data-stu-id="71f54-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="71f54-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="71f54-138">Request</span></span>
<span data-ttu-id="71f54-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71f54-139">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71f54-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="71f54-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="71f54-141">C#</span><span class="sxs-lookup"><span data-stu-id="71f54-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71f54-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71f54-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71f54-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71f54-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71f54-144">Java</span><span class="sxs-lookup"><span data-stu-id="71f54-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="71f54-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="71f54-145">Response</span></span>
<span data-ttu-id="71f54-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71f54-146">The following is an example of a response.</span></span>
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
  ]
}
-->


