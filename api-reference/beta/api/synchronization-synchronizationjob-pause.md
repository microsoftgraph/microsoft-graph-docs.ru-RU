---
title: 'synchronizationJob: Приостановка'
description: Временно приостановить синхронизации. Сохраняются все текущие, включая состояние задания и задание продолжит работу с где остановились при вызове Пуск.
ms.openlocfilehash: dd46f5760d7ddcfff1e254d7c000e1cd80304f07
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077315"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="bc64c-104">synchronizationJob: Приостановка</span><span class="sxs-lookup"><span data-stu-id="bc64c-104">synchronizationJob: pause</span></span>

> <span data-ttu-id="bc64c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc64c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc64c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc64c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc64c-107">Временно приостановить синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bc64c-107">Temporarily stop synchronization.</span></span> <span data-ttu-id="bc64c-108">Сохраняются все текущие, включая состояние задания и задание продолжит работу с где оно было прервано Если [запустить](../api/synchronization-synchronizationjob-start.md) вызов.</span><span class="sxs-lookup"><span data-stu-id="bc64c-108">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc64c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc64c-109">Permissions</span></span>
<span data-ttu-id="bc64c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc64c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc64c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc64c-112">Permission type</span></span>                        | <span data-ttu-id="bc64c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc64c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc64c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc64c-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="bc64c-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc64c-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="bc64c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc64c-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="bc64c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc64c-117">Not supported.</span></span>  |
|<span data-ttu-id="bc64c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc64c-118">Application</span></span>                            |<span data-ttu-id="bc64c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc64c-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bc64c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc64c-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="bc64c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc64c-121">Request headers</span></span>

| <span data-ttu-id="bc64c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bc64c-122">Name</span></span>           | <span data-ttu-id="bc64c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="bc64c-123">Type</span></span>    | <span data-ttu-id="bc64c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="bc64c-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="bc64c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc64c-125">Authorization</span></span>  | <span data-ttu-id="bc64c-126">string</span><span class="sxs-lookup"><span data-stu-id="bc64c-126">string</span></span>  | <span data-ttu-id="bc64c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc64c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc64c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc64c-129">Request body</span></span>

<span data-ttu-id="bc64c-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc64c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc64c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc64c-131">Response</span></span>

<span data-ttu-id="bc64c-132">В случае успеха возвращает `204 No Content` ответа.</span><span class="sxs-lookup"><span data-stu-id="bc64c-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="bc64c-133">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bc64c-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc64c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="bc64c-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bc64c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc64c-135">Request</span></span>
<span data-ttu-id="bc64c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc64c-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="bc64c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc64c-137">Response</span></span>
<span data-ttu-id="bc64c-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bc64c-138">The following is an example of a response.</span></span>
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