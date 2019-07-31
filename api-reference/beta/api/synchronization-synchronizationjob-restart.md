---
title: Перезапуск Синчронизатионжоб
description: Перезапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге. При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4c948c7643759d12ec2bd6731e3f78c527e4a6bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982713"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="fdec6-104">Перезапуск Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="fdec6-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdec6-105">Перезапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="fdec6-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="fdec6-106">При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.</span><span class="sxs-lookup"><span data-stu-id="fdec6-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdec6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fdec6-107">Permissions</span></span>
<span data-ttu-id="fdec6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdec6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdec6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdec6-110">Permission type</span></span>                        | <span data-ttu-id="fdec6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdec6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdec6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdec6-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="fdec6-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdec6-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="fdec6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdec6-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="fdec6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdec6-115">Not supported.</span></span> |
|<span data-ttu-id="fdec6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdec6-116">Application</span></span>                            |<span data-ttu-id="fdec6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdec6-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="fdec6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdec6-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="fdec6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdec6-119">Request headers</span></span>

| <span data-ttu-id="fdec6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fdec6-120">Name</span></span>           | <span data-ttu-id="fdec6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fdec6-121">Type</span></span>    | <span data-ttu-id="fdec6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fdec6-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="fdec6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdec6-123">Authorization</span></span>  | <span data-ttu-id="fdec6-124">string</span><span class="sxs-lookup"><span data-stu-id="fdec6-124">string</span></span>  | <span data-ttu-id="fdec6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdec6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdec6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fdec6-127">Request body</span></span>

<span data-ttu-id="fdec6-128">В тексте запроса укажите объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="fdec6-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="fdec6-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="fdec6-129">Parameter</span></span>     | <span data-ttu-id="fdec6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fdec6-130">Type</span></span>      | <span data-ttu-id="fdec6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fdec6-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="fdec6-132">criteria</span><span class="sxs-lookup"><span data-stu-id="fdec6-132">criteria</span></span>       |[<span data-ttu-id="fdec6-133">Синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="fdec6-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="fdec6-134">Условия перезапуска</span><span class="sxs-lookup"><span data-stu-id="fdec6-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="fdec6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdec6-135">Response</span></span>

<span data-ttu-id="fdec6-136">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="fdec6-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="fdec6-137">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fdec6-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdec6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="fdec6-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fdec6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdec6-139">Request</span></span>
<span data-ttu-id="fdec6-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdec6-140">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fdec6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdec6-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fdec6-142">C#</span><span class="sxs-lookup"><span data-stu-id="fdec6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-restart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fdec6-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="fdec6-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-restart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fdec6-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fdec6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-restart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fdec6-145">Java</span><span class="sxs-lookup"><span data-stu-id="fdec6-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-restart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fdec6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdec6-146">Response</span></span>
<span data-ttu-id="fdec6-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fdec6-147">The following is an example of a response.</span></span>

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
