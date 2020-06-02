---
title: 'Свапшифтсчанжерекуест: утверждение'
description: Утверждение запроса на смену замены.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b564884e57cd5ce1e4350034b0b98380eb8f8b7c
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44154131"
---
# <a name="swapshiftschangerequest-approve"></a><span data-ttu-id="fc51d-103">Свапшифтсчанжерекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="fc51d-103">swapShiftsChangeRequest: approve</span></span>

<span data-ttu-id="fc51d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc51d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc51d-105">Утверждение объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="fc51d-105">Approve a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc51d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc51d-106">Permissions</span></span>

<span data-ttu-id="fc51d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc51d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc51d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc51d-109">Permission type</span></span>                        | <span data-ttu-id="fc51d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc51d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fc51d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc51d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc51d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc51d-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="fc51d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc51d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc51d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc51d-114">Not supported.</span></span> |
| <span data-ttu-id="fc51d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc51d-115">Application</span></span>                            | <span data-ttu-id="fc51d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc51d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc51d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc51d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="fc51d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc51d-118">Request headers</span></span>

| <span data-ttu-id="fc51d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fc51d-119">Name</span></span>          | <span data-ttu-id="fc51d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fc51d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fc51d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc51d-121">Authorization</span></span> | <span data-ttu-id="fc51d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc51d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc51d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc51d-124">Content-type</span></span> | <span data-ttu-id="fc51d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc51d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc51d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc51d-127">Request body</span></span>

<span data-ttu-id="fc51d-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fc51d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc51d-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="fc51d-129">Parameter</span></span>    | <span data-ttu-id="fc51d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fc51d-130">Type</span></span>        | <span data-ttu-id="fc51d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fc51d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc51d-132">message</span><span class="sxs-lookup"><span data-stu-id="fc51d-132">message</span></span>|<span data-ttu-id="fc51d-133">String</span><span class="sxs-lookup"><span data-stu-id="fc51d-133">String</span></span>|<span data-ttu-id="fc51d-134">Настраиваемое сообщение утверждения.</span><span class="sxs-lookup"><span data-stu-id="fc51d-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="fc51d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc51d-135">Response</span></span>

<span data-ttu-id="fc51d-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fc51d-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc51d-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="fc51d-138">Examples</span></span>

<span data-ttu-id="fc51d-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="fc51d-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="fc51d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc51d-140">Request</span></span>

<span data-ttu-id="fc51d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc51d-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc51d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc51d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="fc51d-143">C#</span><span class="sxs-lookup"><span data-stu-id="fc51d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc51d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc51d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc51d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc51d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fc51d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc51d-146">Response</span></span>

<span data-ttu-id="fc51d-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fc51d-147">The following is an example of the response.</span></span>
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
