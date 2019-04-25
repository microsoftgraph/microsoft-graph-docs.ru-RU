---
title: Перезапуск Синчронизатионжоб
description: ПереЗапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге. При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.
localization_priority: Normal
ms.openlocfilehash: 169f95c3662fd774207584b54fcf27fb2548c795
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537101"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="7677d-104">Перезапуск Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="7677d-104">Restart synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7677d-105">ПереЗапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге.</span><span class="sxs-lookup"><span data-stu-id="7677d-105">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="7677d-106">При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.</span><span class="sxs-lookup"><span data-stu-id="7677d-106">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="7677d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7677d-107">Permissions</span></span>
<span data-ttu-id="7677d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7677d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7677d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7677d-110">Permission type</span></span>                        | <span data-ttu-id="7677d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7677d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7677d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7677d-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="7677d-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7677d-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7677d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7677d-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7677d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7677d-115">Not supported.</span></span> |
|<span data-ttu-id="7677d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7677d-116">Application</span></span>                            |<span data-ttu-id="7677d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7677d-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="7677d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7677d-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="7677d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7677d-119">Request headers</span></span>

| <span data-ttu-id="7677d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7677d-120">Name</span></span>           | <span data-ttu-id="7677d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7677d-121">Type</span></span>    | <span data-ttu-id="7677d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7677d-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7677d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7677d-123">Authorization</span></span>  | <span data-ttu-id="7677d-124">string</span><span class="sxs-lookup"><span data-stu-id="7677d-124">string</span></span>  | <span data-ttu-id="7677d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7677d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7677d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7677d-127">Request body</span></span>

<span data-ttu-id="7677d-128">В тексте запроса укажите объект JSON со следующим параметром.</span><span class="sxs-lookup"><span data-stu-id="7677d-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="7677d-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="7677d-129">Parameter</span></span>     | <span data-ttu-id="7677d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7677d-130">Type</span></span>      | <span data-ttu-id="7677d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7677d-131">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="7677d-132">criteria</span><span class="sxs-lookup"><span data-stu-id="7677d-132">criteria</span></span>       |[<span data-ttu-id="7677d-133">Синчронизатионжобрестарткритериа</span><span class="sxs-lookup"><span data-stu-id="7677d-133">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="7677d-134">Условия переЗапуска</span><span class="sxs-lookup"><span data-stu-id="7677d-134">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="7677d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7677d-135">Response</span></span>

<span data-ttu-id="7677d-136">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="7677d-136">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="7677d-137">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7677d-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7677d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7677d-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7677d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7677d-139">Request</span></span>
<span data-ttu-id="7677d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7677d-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7677d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7677d-141">Response</span></span>
<span data-ttu-id="7677d-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7677d-142">The following is an example of a response.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-restart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
