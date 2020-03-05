---
title: 'Синчронизатионжоб: пауза'
description: Временная остановка синхронизации. Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении начального вызова.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e1dd3b835242f40af98bdfa7e3ce732adb78f6a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453007"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="b2556-104">Синчронизатионжоб: пауза</span><span class="sxs-lookup"><span data-stu-id="b2556-104">synchronizationJob: pause</span></span>

<span data-ttu-id="b2556-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b2556-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2556-106">Временная остановка синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b2556-106">Temporarily stop synchronization.</span></span> <span data-ttu-id="b2556-107">Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="b2556-107">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2556-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2556-108">Permissions</span></span>
<span data-ttu-id="b2556-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2556-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2556-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2556-111">Permission type</span></span>                        | <span data-ttu-id="b2556-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2556-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2556-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2556-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="b2556-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2556-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b2556-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2556-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b2556-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2556-116">Not supported.</span></span>  |
|<span data-ttu-id="b2556-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2556-117">Application</span></span>                            |<span data-ttu-id="b2556-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2556-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b2556-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2556-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="b2556-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b2556-120">Request headers</span></span>

| <span data-ttu-id="b2556-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b2556-121">Name</span></span>           | <span data-ttu-id="b2556-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b2556-122">Type</span></span>    | <span data-ttu-id="b2556-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b2556-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b2556-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2556-124">Authorization</span></span>  | <span data-ttu-id="b2556-125">string</span><span class="sxs-lookup"><span data-stu-id="b2556-125">string</span></span>  | <span data-ttu-id="b2556-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2556-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2556-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2556-128">Request body</span></span>

<span data-ttu-id="b2556-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2556-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2556-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2556-130">Response</span></span>

<span data-ttu-id="b2556-131">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="b2556-131">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="b2556-132">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b2556-132">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2556-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b2556-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b2556-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2556-134">Request</span></span>
<span data-ttu-id="b2556-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2556-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2556-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2556-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```
# <a name="c"></a>[<span data-ttu-id="b2556-137">C#</span><span class="sxs-lookup"><span data-stu-id="b2556-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2556-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2556-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2556-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2556-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b2556-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2556-140">Response</span></span>
<span data-ttu-id="b2556-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b2556-141">The following is an example of a response.</span></span>
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
