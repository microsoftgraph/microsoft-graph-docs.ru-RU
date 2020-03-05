---
title: 'Свапшифтсчанжерекуест: утверждение'
description: Утверждение запроса на смену замены.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 42b2d4991e0f24acac12901e3cde45e51d04c5af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453083"
---
# <a name="swapshiftschangerequest-approve"></a><span data-ttu-id="f8fe2-103">Свапшифтсчанжерекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="f8fe2-103">swapShiftsChangeRequest: approve</span></span>

<span data-ttu-id="f8fe2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f8fe2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8fe2-105">Утверждение объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="f8fe2-105">Approve a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8fe2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8fe2-106">Permissions</span></span>

<span data-ttu-id="f8fe2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8fe2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8fe2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8fe2-109">Permission type</span></span>                        | <span data-ttu-id="f8fe2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8fe2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f8fe2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8fe2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8fe2-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8fe2-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f8fe2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8fe2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8fe2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8fe2-114">Not supported.</span></span> |
| <span data-ttu-id="f8fe2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8fe2-115">Application</span></span>                            | <span data-ttu-id="f8fe2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8fe2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8fe2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8fe2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="f8fe2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8fe2-118">Request headers</span></span>

| <span data-ttu-id="f8fe2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f8fe2-119">Name</span></span>          | <span data-ttu-id="f8fe2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f8fe2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f8fe2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8fe2-121">Authorization</span></span> | <span data-ttu-id="f8fe2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8fe2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f8fe2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8fe2-124">Content-type</span></span> | <span data-ttu-id="f8fe2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8fe2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8fe2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8fe2-127">Request body</span></span>

<span data-ttu-id="f8fe2-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f8fe2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8fe2-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="f8fe2-129">Parameter</span></span>    | <span data-ttu-id="f8fe2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f8fe2-130">Type</span></span>        | <span data-ttu-id="f8fe2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f8fe2-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f8fe2-132">message</span><span class="sxs-lookup"><span data-stu-id="f8fe2-132">message</span></span>|<span data-ttu-id="f8fe2-133">String</span><span class="sxs-lookup"><span data-stu-id="f8fe2-133">String</span></span>|<span data-ttu-id="f8fe2-134">Настраиваемое сообщение утверждения.</span><span class="sxs-lookup"><span data-stu-id="f8fe2-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="f8fe2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8fe2-135">Response</span></span>

<span data-ttu-id="f8fe2-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f8fe2-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8fe2-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="f8fe2-138">Examples</span></span>

<span data-ttu-id="f8fe2-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f8fe2-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f8fe2-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8fe2-140">Request</span></span>

<span data-ttu-id="f8fe2-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8fe2-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f8fe2-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8fe2-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="f8fe2-143">C#</span><span class="sxs-lookup"><span data-stu-id="f8fe2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8fe2-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8fe2-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8fe2-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8fe2-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8fe2-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8fe2-146">Response</span></span>

<span data-ttu-id="f8fe2-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f8fe2-147">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
