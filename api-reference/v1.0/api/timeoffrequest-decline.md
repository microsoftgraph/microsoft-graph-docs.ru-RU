---
title: 'timeOffRequest: снижение'
description: Отклонение объекта timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7f9e5f6151e30dbbfcfc74db51a9a8e2afacab1c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787424"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="1dce9-103">timeOffRequest: снижение</span><span class="sxs-lookup"><span data-stu-id="1dce9-103">timeOffRequest: decline</span></span>

<span data-ttu-id="1dce9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dce9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1dce9-105">[Отклонение объекта timeoffrequest.](../resources/timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="1dce9-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dce9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1dce9-106">Permissions</span></span>

<span data-ttu-id="1dce9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dce9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1dce9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dce9-109">Permission type</span></span>                        | <span data-ttu-id="1dce9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dce9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="1dce9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dce9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1dce9-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dce9-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1dce9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dce9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dce9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dce9-114">Not supported.</span></span>    |
|<span data-ttu-id="1dce9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dce9-115">Application</span></span> | <span data-ttu-id="1dce9-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dce9-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="1dce9-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="1dce9-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1dce9-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="1dce9-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1dce9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dce9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="1dce9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dce9-120">Request headers</span></span>

| <span data-ttu-id="1dce9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1dce9-121">Name</span></span>          | <span data-ttu-id="1dce9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1dce9-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1dce9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dce9-123">Authorization</span></span> | <span data-ttu-id="1dce9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dce9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1dce9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1dce9-126">Content-type</span></span> | <span data-ttu-id="1dce9-127">application-json.</span><span class="sxs-lookup"><span data-stu-id="1dce9-127">application-json.</span></span> <span data-ttu-id="1dce9-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1dce9-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dce9-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1dce9-129">Request body</span></span>

<span data-ttu-id="1dce9-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1dce9-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1dce9-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="1dce9-131">Parameter</span></span>    | <span data-ttu-id="1dce9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="1dce9-132">Type</span></span>        | <span data-ttu-id="1dce9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="1dce9-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1dce9-134">message</span><span class="sxs-lookup"><span data-stu-id="1dce9-134">message</span></span>|<span data-ttu-id="1dce9-135">String</span><span class="sxs-lookup"><span data-stu-id="1dce9-135">String</span></span>|<span data-ttu-id="1dce9-136">Пользовательское сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="1dce9-136">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="1dce9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dce9-137">Response</span></span>

<span data-ttu-id="1dce9-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1dce9-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1dce9-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="1dce9-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1dce9-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dce9-141">Request</span></span>

<span data-ttu-id="1dce9-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dce9-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1dce9-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dce9-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1dce9-144">C#</span><span class="sxs-lookup"><span data-stu-id="1dce9-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dce9-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dce9-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dce9-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dce9-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dce9-147">Java</span><span class="sxs-lookup"><span data-stu-id="1dce9-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="1dce9-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dce9-148">Response</span></span>

<span data-ttu-id="1dce9-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1dce9-149">The following is an example of the response.</span></span>
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
  "description": "timeOffRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

