---
title: 'openShiftChangeRequest: снижение'
description: Отклонение openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 56bcbf6c9c29b83582d14cc562768cb3385dc598
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448143"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="6c36d-103">openShiftChangeRequest: снижение</span><span class="sxs-lookup"><span data-stu-id="6c36d-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="6c36d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c36d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c36d-105">Отклонение [объекта openShiftChangeRequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="6c36d-105">Decline an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c36d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c36d-106">Permissions</span></span>

<span data-ttu-id="6c36d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c36d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c36d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c36d-109">Permission type</span></span>                        | <span data-ttu-id="6c36d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c36d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c36d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c36d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c36d-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c36d-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6c36d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c36d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c36d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c36d-114">Not supported.</span></span> |
| <span data-ttu-id="6c36d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c36d-115">Application</span></span>                            | <span data-ttu-id="6c36d-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c36d-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="6c36d-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="6c36d-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6c36d-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="6c36d-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6c36d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c36d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="6c36d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c36d-120">Request headers</span></span>

| <span data-ttu-id="6c36d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6c36d-121">Name</span></span>          | <span data-ttu-id="6c36d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6c36d-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6c36d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c36d-123">Authorization</span></span> | <span data-ttu-id="6c36d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c36d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c36d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c36d-126">Content-type</span></span> | <span data-ttu-id="6c36d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c36d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c36d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c36d-129">Request body</span></span>

<span data-ttu-id="6c36d-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6c36d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6c36d-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="6c36d-131">Parameter</span></span>    | <span data-ttu-id="6c36d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6c36d-132">Type</span></span>        | <span data-ttu-id="6c36d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6c36d-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c36d-134">message</span><span class="sxs-lookup"><span data-stu-id="6c36d-134">message</span></span>|<span data-ttu-id="6c36d-135">String</span><span class="sxs-lookup"><span data-stu-id="6c36d-135">String</span></span>|<span data-ttu-id="6c36d-136">Пользовательское сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="6c36d-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="6c36d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c36d-137">Response</span></span>

<span data-ttu-id="6c36d-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6c36d-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c36d-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c36d-140">Examples</span></span>

<span data-ttu-id="6c36d-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6c36d-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6c36d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c36d-142">Request</span></span>

<span data-ttu-id="6c36d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c36d-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c36d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c36d-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6c36d-145">C#</span><span class="sxs-lookup"><span data-stu-id="6c36d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/openshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c36d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c36d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/openshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c36d-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c36d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/openshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c36d-148">Java</span><span class="sxs-lookup"><span data-stu-id="6c36d-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/openshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c36d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c36d-149">Response</span></span>

<span data-ttu-id="6c36d-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6c36d-150">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

