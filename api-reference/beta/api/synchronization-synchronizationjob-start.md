---
title: Запуск Синчронизатионжоб
description: Запуск существующего задания синхронизации. Если задание приостановлено, оно продолжит обработку изменений с того места, где оно было приостановлено. Если задание находится в карантине, состояние карантина будет очищено.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6c27b2c0d43a32bd32b85671c445faca7d5689de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437521"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="7ad9e-105">Запуск Синчронизатионжоб</span><span class="sxs-lookup"><span data-stu-id="7ad9e-105">Start synchronizationJob</span></span>

<span data-ttu-id="7ad9e-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ad9e-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ad9e-107">Запуск существующего задания синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-107">Start an existing synchronization job.</span></span> <span data-ttu-id="7ad9e-108">Если задание приостановлено, оно продолжит обработку изменений с того места, где оно было приостановлено.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-108">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="7ad9e-109">Если задание находится в карантине, состояние карантина будет очищено.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-109">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ad9e-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ad9e-110">Permissions</span></span>
<span data-ttu-id="7ad9e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ad9e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ad9e-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ad9e-113">Permission type</span></span>                        | <span data-ttu-id="7ad9e-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ad9e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ad9e-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ad9e-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="7ad9e-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ad9e-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7ad9e-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ad9e-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7ad9e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-118">Not supported.</span></span> |
|<span data-ttu-id="7ad9e-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ad9e-119">Application</span></span>                            |<span data-ttu-id="7ad9e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7ad9e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ad9e-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="7ad9e-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7ad9e-122">Request headers</span></span>

| <span data-ttu-id="7ad9e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7ad9e-123">Name</span></span>           | <span data-ttu-id="7ad9e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7ad9e-124">Type</span></span>    | <span data-ttu-id="7ad9e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7ad9e-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7ad9e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ad9e-126">Authorization</span></span>  | <span data-ttu-id="7ad9e-127">string</span><span class="sxs-lookup"><span data-stu-id="7ad9e-127">string</span></span>  | <span data-ttu-id="7ad9e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ad9e-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ad9e-130">Request body</span></span>

<span data-ttu-id="7ad9e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-131">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="7ad9e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ad9e-132">Response</span></span>

<span data-ttu-id="7ad9e-133">В случае успеха возвращает `204 No Content` отклик.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-133">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="7ad9e-134">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ad9e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="7ad9e-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7ad9e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ad9e-136">Request</span></span>
<span data-ttu-id="7ad9e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-137">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ad9e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ad9e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="7ad9e-139">C#</span><span class="sxs-lookup"><span data-stu-id="7ad9e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ad9e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ad9e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ad9e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ad9e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7ad9e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ad9e-142">Response</span></span>
<span data-ttu-id="7ad9e-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ad9e-143">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
