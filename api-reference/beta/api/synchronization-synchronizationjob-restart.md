---
title: Restart synchronizationJob
description: Перезапустите задание синхронизации, принудительно обжав все объекты в каталоге. При желании очищает существующее состояние синхронизации и предыдущие ошибки.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: dc257c78f5f7463cafb987a0d34c8fed546f3dd8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132785"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="92d2e-104">Restart synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="92d2e-104">Restart synchronizationJob</span></span>

<span data-ttu-id="92d2e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92d2e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92d2e-106">Перезапустите задание синхронизации, принудительно обобсвив все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="92d2e-106">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="92d2e-107">При желании очищает существующее состояние синхронизации и предыдущие ошибки.</span><span class="sxs-lookup"><span data-stu-id="92d2e-107">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="92d2e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92d2e-108">Permissions</span></span>
<span data-ttu-id="92d2e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92d2e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92d2e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92d2e-111">Permission type</span></span>                        | <span data-ttu-id="92d2e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92d2e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="92d2e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92d2e-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="92d2e-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92d2e-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="92d2e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92d2e-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="92d2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92d2e-116">Not supported.</span></span> |
|<span data-ttu-id="92d2e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92d2e-117">Application</span></span>                            |<span data-ttu-id="92d2e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92d2e-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="92d2e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92d2e-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="92d2e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92d2e-120">Request headers</span></span>

| <span data-ttu-id="92d2e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="92d2e-121">Name</span></span>           | <span data-ttu-id="92d2e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="92d2e-122">Type</span></span>    | <span data-ttu-id="92d2e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="92d2e-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="92d2e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="92d2e-124">Authorization</span></span>  | <span data-ttu-id="92d2e-125">string</span><span class="sxs-lookup"><span data-stu-id="92d2e-125">string</span></span>  | <span data-ttu-id="92d2e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92d2e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92d2e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92d2e-128">Request body</span></span>

<span data-ttu-id="92d2e-129">В теле запроса укажу объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="92d2e-129">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="92d2e-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="92d2e-130">Parameter</span></span>     | <span data-ttu-id="92d2e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="92d2e-131">Type</span></span>      | <span data-ttu-id="92d2e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="92d2e-132">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="92d2e-133">criteria</span><span class="sxs-lookup"><span data-stu-id="92d2e-133">criteria</span></span>       |[<span data-ttu-id="92d2e-134">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="92d2e-134">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="92d2e-135">Условия перезапуска</span><span class="sxs-lookup"><span data-stu-id="92d2e-135">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="92d2e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="92d2e-136">Response</span></span>

<span data-ttu-id="92d2e-137">В случае успеха возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="92d2e-137">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="92d2e-138">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="92d2e-138">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92d2e-139">Пример</span><span class="sxs-lookup"><span data-stu-id="92d2e-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="92d2e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="92d2e-140">Request</span></span>
<span data-ttu-id="92d2e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92d2e-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92d2e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="92d2e-142">HTTP</span></span>](#tab/http)
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
       "resetScope": "Watermark, Escrows, QuarantineState"
   }
}
```
# <a name="c"></a>[<span data-ttu-id="92d2e-143">C#</span><span class="sxs-lookup"><span data-stu-id="92d2e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-restart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92d2e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92d2e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-restart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92d2e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92d2e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-restart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92d2e-146">Java</span><span class="sxs-lookup"><span data-stu-id="92d2e-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-restart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="92d2e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="92d2e-147">Response</span></span>
<span data-ttu-id="92d2e-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92d2e-148">The following is an example of a response.</span></span>

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
  ]
}
-->


