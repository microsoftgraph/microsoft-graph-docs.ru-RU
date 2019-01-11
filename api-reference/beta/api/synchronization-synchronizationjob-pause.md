---
title: 'synchronizationJob: Приостановка'
description: Временно приостановить синхронизации. Сохраняются все текущие, включая состояние задания и задание продолжит работу с где остановились при вызове Пуск.
localization_priority: Normal
ms.openlocfilehash: f39b3a700b31169ea15f089da8873b517b50dc15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804881"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="08da7-104">synchronizationJob: Приостановка</span><span class="sxs-lookup"><span data-stu-id="08da7-104">synchronizationJob: pause</span></span>

> <span data-ttu-id="08da7-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="08da7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08da7-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08da7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08da7-107">Временно приостановить синхронизации.</span><span class="sxs-lookup"><span data-stu-id="08da7-107">Temporarily stop synchronization.</span></span> <span data-ttu-id="08da7-108">Сохраняются все текущие, включая состояние задания и задание продолжит работу с где оно было прервано Если [запустить](../api/synchronization-synchronizationjob-start.md) вызов.</span><span class="sxs-lookup"><span data-stu-id="08da7-108">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="08da7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08da7-109">Permissions</span></span>
<span data-ttu-id="08da7-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08da7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08da7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08da7-112">Permission type</span></span>                        | <span data-ttu-id="08da7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08da7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="08da7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08da7-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="08da7-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08da7-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="08da7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08da7-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="08da7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08da7-117">Not supported.</span></span>  |
|<span data-ttu-id="08da7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08da7-118">Application</span></span>                            |<span data-ttu-id="08da7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08da7-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="08da7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08da7-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="08da7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08da7-121">Request headers</span></span>

| <span data-ttu-id="08da7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="08da7-122">Name</span></span>           | <span data-ttu-id="08da7-123">Тип</span><span class="sxs-lookup"><span data-stu-id="08da7-123">Type</span></span>    | <span data-ttu-id="08da7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="08da7-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="08da7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="08da7-125">Authorization</span></span>  | <span data-ttu-id="08da7-126">string</span><span class="sxs-lookup"><span data-stu-id="08da7-126">string</span></span>  | <span data-ttu-id="08da7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08da7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08da7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08da7-129">Request body</span></span>

<span data-ttu-id="08da7-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08da7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08da7-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="08da7-131">Response</span></span>

<span data-ttu-id="08da7-132">В случае успеха возвращает `204 No Content` ответа.</span><span class="sxs-lookup"><span data-stu-id="08da7-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="08da7-133">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="08da7-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08da7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="08da7-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="08da7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="08da7-135">Request</span></span>
<span data-ttu-id="08da7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08da7-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="08da7-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="08da7-137">Response</span></span>
<span data-ttu-id="08da7-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="08da7-138">The following is an example of a response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
