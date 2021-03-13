---
title: 'синхронизацияJob: пауза'
description: Временно прекратите синхронизацию. Все ходы, включая состояние задания, сохраняются, и задание будет продолжено с того места, где оно было отключено при запуске вызова.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 868184491c13e67b9bcd773f0a82383a5310d67b
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50776237"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="d4771-104">синхронизацияJob: пауза</span><span class="sxs-lookup"><span data-stu-id="d4771-104">synchronizationJob: pause</span></span>

<span data-ttu-id="d4771-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4771-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4771-106">Временно прекратите синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="d4771-106">Temporarily stop synchronization.</span></span> <span data-ttu-id="d4771-107">Все ходы, включая состояние задания, сохраняются, и задание будет продолжено [](../api/synchronization-synchronizationjob-start.md) с того места, где оно было отключено при запуске вызова.</span><span class="sxs-lookup"><span data-stu-id="d4771-107">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4771-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4771-108">Permissions</span></span>
<span data-ttu-id="d4771-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4771-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4771-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4771-111">Permission type</span></span>                        | <span data-ttu-id="d4771-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4771-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4771-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4771-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="d4771-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4771-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d4771-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4771-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d4771-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4771-116">Not supported.</span></span>  |
|<span data-ttu-id="d4771-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4771-117">Application</span></span>                            |<span data-ttu-id="d4771-118">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4771-118">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d4771-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4771-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="d4771-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d4771-120">Request headers</span></span>

| <span data-ttu-id="d4771-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d4771-121">Name</span></span>           | <span data-ttu-id="d4771-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d4771-122">Type</span></span>    | <span data-ttu-id="d4771-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d4771-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d4771-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4771-124">Authorization</span></span>  | <span data-ttu-id="d4771-125">string</span><span class="sxs-lookup"><span data-stu-id="d4771-125">string</span></span>  | <span data-ttu-id="d4771-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4771-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4771-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4771-128">Request body</span></span>

<span data-ttu-id="d4771-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4771-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4771-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4771-130">Response</span></span>

<span data-ttu-id="d4771-131">В случае успешного ответа `204 No Content` возвращается ответ.</span><span class="sxs-lookup"><span data-stu-id="d4771-131">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="d4771-132">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d4771-132">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4771-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d4771-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d4771-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4771-134">Request</span></span>
<span data-ttu-id="d4771-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4771-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4771-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4771-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```
# <a name="c"></a>[<span data-ttu-id="d4771-137">C#</span><span class="sxs-lookup"><span data-stu-id="d4771-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4771-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4771-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4771-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4771-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4771-140">Java</span><span class="sxs-lookup"><span data-stu-id="d4771-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d4771-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4771-141">Response</span></span>
<span data-ttu-id="d4771-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4771-142">The following is an example of a response.</span></span>
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


