---
title: 'Синчронизатионжоб: пауза'
description: Временная остановка синхронизации. Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении начального вызова.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a1503aa6de14f3738248020c10c3b5d53111476
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977816"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="25d4c-104">Синчронизатионжоб: пауза</span><span class="sxs-lookup"><span data-stu-id="25d4c-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25d4c-105">Временная остановка синхронизации.</span><span class="sxs-lookup"><span data-stu-id="25d4c-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="25d4c-106">Все ход выполнения, включая состояние задания, хранятся, а задание продолжится с того места, где оно было отключено при выполнении [начального](../api/synchronization-synchronizationjob-start.md) вызова.</span><span class="sxs-lookup"><span data-stu-id="25d4c-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="25d4c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25d4c-107">Permissions</span></span>
<span data-ttu-id="25d4c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25d4c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25d4c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25d4c-110">Permission type</span></span>                        | <span data-ttu-id="25d4c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25d4c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="25d4c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25d4c-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="25d4c-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25d4c-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="25d4c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25d4c-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="25d4c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25d4c-115">Not supported.</span></span>  |
|<span data-ttu-id="25d4c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25d4c-116">Application</span></span>                            |<span data-ttu-id="25d4c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25d4c-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="25d4c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25d4c-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="25d4c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25d4c-119">Request headers</span></span>

| <span data-ttu-id="25d4c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="25d4c-120">Name</span></span>           | <span data-ttu-id="25d4c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="25d4c-121">Type</span></span>    | <span data-ttu-id="25d4c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="25d4c-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="25d4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="25d4c-123">Authorization</span></span>  | <span data-ttu-id="25d4c-124">string</span><span class="sxs-lookup"><span data-stu-id="25d4c-124">string</span></span>  | <span data-ttu-id="25d4c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25d4c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25d4c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25d4c-127">Request body</span></span>

<span data-ttu-id="25d4c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25d4c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25d4c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="25d4c-129">Response</span></span>

<span data-ttu-id="25d4c-130">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="25d4c-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="25d4c-131">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="25d4c-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25d4c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="25d4c-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25d4c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="25d4c-133">Request</span></span>
<span data-ttu-id="25d4c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25d4c-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="25d4c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="25d4c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="25d4c-136">C#</span><span class="sxs-lookup"><span data-stu-id="25d4c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25d4c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="25d4c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="25d4c-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="25d4c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="25d4c-139">Java</span><span class="sxs-lookup"><span data-stu-id="25d4c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25d4c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="25d4c-140">Response</span></span>
<span data-ttu-id="25d4c-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25d4c-141">The following is an example of a response.</span></span>
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
