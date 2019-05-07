---
title: Перезапуск Синчронизатионжоб
description: Перезапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге. При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.
localization_priority: Normal
ms.openlocfilehash: ae88562bba0c3d0b9d618272015f2c9044fc8c95
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638027"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="2ad5c-104">Перезапуск Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="2ad5c-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ad5c-105">Перезапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="2ad5c-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="2ad5c-106">При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.</span><span class="sxs-lookup"><span data-stu-id="2ad5c-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ad5c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ad5c-107">Permissions</span></span>
<span data-ttu-id="2ad5c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ad5c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ad5c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ad5c-110">Permission type</span></span>                        | <span data-ttu-id="2ad5c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ad5c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ad5c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ad5c-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="2ad5c-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ad5c-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2ad5c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ad5c-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2ad5c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ad5c-115">Not supported.</span></span> |
|<span data-ttu-id="2ad5c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ad5c-116">Application</span></span>                            |<span data-ttu-id="2ad5c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ad5c-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="2ad5c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ad5c-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="2ad5c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ad5c-119">Request headers</span></span>

| <span data-ttu-id="2ad5c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2ad5c-120">Name</span></span>           | <span data-ttu-id="2ad5c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2ad5c-121">Type</span></span>    | <span data-ttu-id="2ad5c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2ad5c-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="2ad5c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ad5c-123">Authorization</span></span>  | <span data-ttu-id="2ad5c-124">string</span><span class="sxs-lookup"><span data-stu-id="2ad5c-124">string</span></span>  | <span data-ttu-id="2ad5c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ad5c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ad5c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ad5c-127">Request body</span></span>

<span data-ttu-id="2ad5c-128">В тексте запроса укажите объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="2ad5c-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="2ad5c-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="2ad5c-129">Parameter</span></span>     | <span data-ttu-id="2ad5c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2ad5c-130">Type</span></span>      | <span data-ttu-id="2ad5c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2ad5c-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="2ad5c-132">criteria</span><span class="sxs-lookup"><span data-stu-id="2ad5c-132">criteria</span></span>       |[<span data-ttu-id="2ad5c-133">Синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="2ad5c-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="2ad5c-134">Условия перезапуска</span><span class="sxs-lookup"><span data-stu-id="2ad5c-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="2ad5c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ad5c-135">Response</span></span>

<span data-ttu-id="2ad5c-136">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="2ad5c-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="2ad5c-137">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2ad5c-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ad5c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2ad5c-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2ad5c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ad5c-139">Request</span></span>
<span data-ttu-id="2ad5c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ad5c-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2ad5c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ad5c-141">Response</span></span>
<span data-ttu-id="2ad5c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ad5c-142">The following is an example of a response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2ad5c-143">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="2ad5c-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2ad5c-144">Языках</span><span class="sxs-lookup"><span data-stu-id="2ad5c-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ad5c-145">Язык</span><span class="sxs-lookup"><span data-stu-id="2ad5c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_restart-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
