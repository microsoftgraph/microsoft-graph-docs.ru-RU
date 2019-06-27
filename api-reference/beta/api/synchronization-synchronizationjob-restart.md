---
title: Перезапуск Синчронизатионжоб
description: Перезапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге. При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.
localization_priority: Normal
ms.openlocfilehash: a97aa458bdecb9e6755add708a5e9799e1365b74
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271367"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="14312-104">Перезапуск Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="14312-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14312-105">Перезапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="14312-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="14312-106">При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.</span><span class="sxs-lookup"><span data-stu-id="14312-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="14312-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14312-107">Permissions</span></span>
<span data-ttu-id="14312-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14312-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14312-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14312-110">Permission type</span></span>                        | <span data-ttu-id="14312-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14312-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="14312-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14312-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="14312-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14312-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="14312-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14312-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="14312-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14312-115">Not supported.</span></span> |
|<span data-ttu-id="14312-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14312-116">Application</span></span>                            |<span data-ttu-id="14312-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14312-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="14312-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14312-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="14312-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14312-119">Request headers</span></span>

| <span data-ttu-id="14312-120">Имя</span><span class="sxs-lookup"><span data-stu-id="14312-120">Name</span></span>           | <span data-ttu-id="14312-121">Тип</span><span class="sxs-lookup"><span data-stu-id="14312-121">Type</span></span>    | <span data-ttu-id="14312-122">Описание</span><span class="sxs-lookup"><span data-stu-id="14312-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="14312-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14312-123">Authorization</span></span>  | <span data-ttu-id="14312-124">string</span><span class="sxs-lookup"><span data-stu-id="14312-124">string</span></span>  | <span data-ttu-id="14312-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14312-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14312-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14312-127">Request body</span></span>

<span data-ttu-id="14312-128">В тексте запроса укажите объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="14312-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="14312-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="14312-129">Parameter</span></span>     | <span data-ttu-id="14312-130">Тип</span><span class="sxs-lookup"><span data-stu-id="14312-130">Type</span></span>      | <span data-ttu-id="14312-131">Описание</span><span class="sxs-lookup"><span data-stu-id="14312-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="14312-132">criteria</span><span class="sxs-lookup"><span data-stu-id="14312-132">criteria</span></span>       |[<span data-ttu-id="14312-133">Синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="14312-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="14312-134">Условия перезапуска</span><span class="sxs-lookup"><span data-stu-id="14312-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="14312-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="14312-135">Response</span></span>

<span data-ttu-id="14312-136">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="14312-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="14312-137">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="14312-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14312-138">Пример</span><span class="sxs-lookup"><span data-stu-id="14312-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="14312-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="14312-139">Request</span></span>
<span data-ttu-id="14312-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14312-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="14312-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="14312-141">Response</span></span>
<span data-ttu-id="14312-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14312-142">The following is an example of a response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="14312-143">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="14312-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="14312-144">C#</span><span class="sxs-lookup"><span data-stu-id="14312-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14312-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="14312-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="14312-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="14312-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
