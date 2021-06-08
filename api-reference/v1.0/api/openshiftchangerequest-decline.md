---
title: 'openShiftChangeRequest: снижение'
description: Отклонение openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eaa5e589a2c420203a4e03fbceda62a701873e3e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787795"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="94ed2-103">openShiftChangeRequest: снижение</span><span class="sxs-lookup"><span data-stu-id="94ed2-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="94ed2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94ed2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94ed2-105">Отклонение [объекта openShiftChangeRequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="94ed2-105">Decline an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94ed2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94ed2-106">Permissions</span></span>

<span data-ttu-id="94ed2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94ed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94ed2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94ed2-109">Permission type</span></span>                        | <span data-ttu-id="94ed2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94ed2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94ed2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94ed2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94ed2-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94ed2-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="94ed2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94ed2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94ed2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94ed2-114">Not supported.</span></span> |
| <span data-ttu-id="94ed2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94ed2-115">Application</span></span>                            | <span data-ttu-id="94ed2-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94ed2-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="94ed2-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="94ed2-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="94ed2-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="94ed2-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="94ed2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94ed2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="94ed2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94ed2-120">Request headers</span></span>

| <span data-ttu-id="94ed2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="94ed2-121">Name</span></span>          | <span data-ttu-id="94ed2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="94ed2-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="94ed2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94ed2-123">Authorization</span></span> | <span data-ttu-id="94ed2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94ed2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94ed2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94ed2-126">Content-type</span></span> | <span data-ttu-id="94ed2-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94ed2-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94ed2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94ed2-129">Request body</span></span>

<span data-ttu-id="94ed2-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="94ed2-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="94ed2-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="94ed2-131">Parameter</span></span>    | <span data-ttu-id="94ed2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="94ed2-132">Type</span></span>        | <span data-ttu-id="94ed2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="94ed2-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94ed2-134">message</span><span class="sxs-lookup"><span data-stu-id="94ed2-134">message</span></span>|<span data-ttu-id="94ed2-135">String</span><span class="sxs-lookup"><span data-stu-id="94ed2-135">String</span></span>|<span data-ttu-id="94ed2-136">Пользовательское сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="94ed2-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="94ed2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="94ed2-137">Response</span></span>

<span data-ttu-id="94ed2-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="94ed2-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94ed2-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="94ed2-140">Examples</span></span>

<span data-ttu-id="94ed2-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="94ed2-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="94ed2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="94ed2-142">Request</span></span>

<span data-ttu-id="94ed2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94ed2-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94ed2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="94ed2-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="94ed2-145">C#</span><span class="sxs-lookup"><span data-stu-id="94ed2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/openshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94ed2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94ed2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/openshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94ed2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94ed2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/openshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94ed2-148">Java</span><span class="sxs-lookup"><span data-stu-id="94ed2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/openshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="94ed2-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="94ed2-149">Response</span></span>

<span data-ttu-id="94ed2-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94ed2-150">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
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

