---
title: 'swapShiftsChangeRequest: снижение'
description: Отклонение запроса на смену замены.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 86ffd631b4fe85b383421ee2a3df7447420ee05f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787538"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="d2f2f-103">swapShiftsChangeRequest: снижение</span><span class="sxs-lookup"><span data-stu-id="d2f2f-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="d2f2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2f2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2f2f-105">Отклонение [объекта swapShiftsChangeRequest.](../resources/swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="d2f2f-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2f2f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f2f-106">Permissions</span></span>

<span data-ttu-id="d2f2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2f2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2f2f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f2f-109">Permission type</span></span>                        | <span data-ttu-id="d2f2f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2f2f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2f2f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2f2f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2f2f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f2f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d2f2f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2f2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2f2f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-114">Not supported.</span></span>                              |
| <span data-ttu-id="d2f2f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2f2f-115">Application</span></span>                            | <span data-ttu-id="d2f2f-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f2f-116">Schedule.ReadWrite.All</span></span>                      |

> <span data-ttu-id="d2f2f-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d2f2f-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d2f2f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2f2f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="d2f2f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2f2f-120">Request headers</span></span>

| <span data-ttu-id="d2f2f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d2f2f-121">Name</span></span>          | <span data-ttu-id="d2f2f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d2f2f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d2f2f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2f2f-123">Authorization</span></span> | <span data-ttu-id="d2f2f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2f2f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2f2f-126">Content-type</span></span> | <span data-ttu-id="d2f2f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2f2f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2f2f-129">Request body</span></span>

<span data-ttu-id="d2f2f-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d2f2f-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="d2f2f-131">Parameter</span></span>    | <span data-ttu-id="d2f2f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d2f2f-132">Type</span></span>        | <span data-ttu-id="d2f2f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d2f2f-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d2f2f-134">message</span><span class="sxs-lookup"><span data-stu-id="d2f2f-134">message</span></span>|<span data-ttu-id="d2f2f-135">String</span><span class="sxs-lookup"><span data-stu-id="d2f2f-135">String</span></span>|<span data-ttu-id="d2f2f-136">Пользовательское сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="d2f2f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f2f-137">Response</span></span>

<span data-ttu-id="d2f2f-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2f2f-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2f2f-140">Examples</span></span>

<span data-ttu-id="d2f2f-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d2f2f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2f2f-142">Request</span></span>

<span data-ttu-id="d2f2f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-143">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d2f2f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2f2f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d2f2f-145">C#</span><span class="sxs-lookup"><span data-stu-id="d2f2f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2f2f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2f2f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2f2f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2f2f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2f2f-148">Java</span><span class="sxs-lookup"><span data-stu-id="d2f2f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="d2f2f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f2f-149">Response</span></span>

<span data-ttu-id="d2f2f-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2f2f-150">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

