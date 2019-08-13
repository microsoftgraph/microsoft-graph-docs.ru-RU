---
title: Перезапуск Синчронизатионжоб
description: Перезапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге. При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 97d85ea53d1cf49d65c62b3e913338d76b4b7bdd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363510"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="8f577-104">Перезапуск Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="8f577-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f577-105">Перезапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="8f577-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="8f577-106">При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.</span><span class="sxs-lookup"><span data-stu-id="8f577-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f577-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f577-107">Permissions</span></span>
<span data-ttu-id="8f577-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f577-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f577-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f577-110">Permission type</span></span>                        | <span data-ttu-id="8f577-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f577-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f577-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f577-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="8f577-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f577-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8f577-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f577-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8f577-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f577-115">Not supported.</span></span> |
|<span data-ttu-id="8f577-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f577-116">Application</span></span>                            |<span data-ttu-id="8f577-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f577-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="8f577-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f577-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="8f577-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f577-119">Request headers</span></span>

| <span data-ttu-id="8f577-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8f577-120">Name</span></span>           | <span data-ttu-id="8f577-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8f577-121">Type</span></span>    | <span data-ttu-id="8f577-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8f577-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8f577-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f577-123">Authorization</span></span>  | <span data-ttu-id="8f577-124">string</span><span class="sxs-lookup"><span data-stu-id="8f577-124">string</span></span>  | <span data-ttu-id="8f577-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f577-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f577-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f577-127">Request body</span></span>

<span data-ttu-id="8f577-128">В тексте запроса укажите объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="8f577-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="8f577-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="8f577-129">Parameter</span></span>     | <span data-ttu-id="8f577-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8f577-130">Type</span></span>      | <span data-ttu-id="8f577-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8f577-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="8f577-132">criteria</span><span class="sxs-lookup"><span data-stu-id="8f577-132">criteria</span></span>       |[<span data-ttu-id="8f577-133">синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="8f577-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="8f577-134">Условия перезапуска</span><span class="sxs-lookup"><span data-stu-id="8f577-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="8f577-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f577-135">Response</span></span>

<span data-ttu-id="8f577-136">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="8f577-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="8f577-137">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8f577-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f577-138">Пример</span><span class="sxs-lookup"><span data-stu-id="8f577-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8f577-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f577-139">Request</span></span>
<span data-ttu-id="8f577-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f577-140">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f577-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f577-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f577-142">C#</span><span class="sxs-lookup"><span data-stu-id="8f577-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-restart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f577-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f577-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-restart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f577-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8f577-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-restart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f577-145">Java</span><span class="sxs-lookup"><span data-stu-id="8f577-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-restart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8f577-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f577-146">Response</span></span>
<span data-ttu-id="8f577-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f577-147">The following is an example of a response.</span></span>

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
