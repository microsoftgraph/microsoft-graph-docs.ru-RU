---
title: 'openShiftChangeRequest: утверждение'
description: Утверждение запроса openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d78d71d961fc820fd5cb7e4965f3e4ee545646d5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448178"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="ddf35-103">openShiftChangeRequest: утверждение</span><span class="sxs-lookup"><span data-stu-id="ddf35-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="ddf35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddf35-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ddf35-105">Утверждение [объекта openShiftChangeRequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="ddf35-105">Approve an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddf35-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddf35-106">Permissions</span></span>

<span data-ttu-id="ddf35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddf35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddf35-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddf35-109">Permission type</span></span>                        | <span data-ttu-id="ddf35-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddf35-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ddf35-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddf35-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddf35-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddf35-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ddf35-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddf35-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddf35-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddf35-114">Not supported.</span></span> |
| <span data-ttu-id="ddf35-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddf35-115">Application</span></span>                            | <span data-ttu-id="ddf35-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddf35-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="ddf35-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ddf35-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ddf35-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="ddf35-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ddf35-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddf35-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="ddf35-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddf35-120">Request headers</span></span>

| <span data-ttu-id="ddf35-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ddf35-121">Name</span></span>          | <span data-ttu-id="ddf35-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ddf35-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ddf35-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddf35-123">Authorization</span></span> | <span data-ttu-id="ddf35-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddf35-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddf35-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ddf35-126">Content-type</span></span> | <span data-ttu-id="ddf35-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddf35-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddf35-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddf35-129">Request body</span></span>

<span data-ttu-id="ddf35-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ddf35-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ddf35-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="ddf35-131">Parameter</span></span>    | <span data-ttu-id="ddf35-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ddf35-132">Type</span></span>        | <span data-ttu-id="ddf35-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ddf35-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ddf35-134">message</span><span class="sxs-lookup"><span data-stu-id="ddf35-134">message</span></span>|<span data-ttu-id="ddf35-135">String</span><span class="sxs-lookup"><span data-stu-id="ddf35-135">String</span></span>|<span data-ttu-id="ddf35-136">Пользовательское сообщение утверждения.</span><span class="sxs-lookup"><span data-stu-id="ddf35-136">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="ddf35-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddf35-137">Response</span></span>

<span data-ttu-id="ddf35-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ddf35-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddf35-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="ddf35-140">Examples</span></span>

<span data-ttu-id="ddf35-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ddf35-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ddf35-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddf35-142">Request</span></span>

<span data-ttu-id="ddf35-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddf35-143">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddf35-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddf35-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="ddf35-145">C#</span><span class="sxs-lookup"><span data-stu-id="ddf35-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/openshiftchangerequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddf35-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddf35-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/openshiftchangerequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddf35-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddf35-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/openshiftchangerequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddf35-148">Java</span><span class="sxs-lookup"><span data-stu-id="ddf35-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/openshiftchangerequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ddf35-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddf35-149">Response</span></span>

<span data-ttu-id="ddf35-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ddf35-150">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

