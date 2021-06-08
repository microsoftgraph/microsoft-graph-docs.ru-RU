---
title: 'timeOffRequest: снижение'
description: Отклонение объекта timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0f745bea1f16680861c92fa8b4a5c18025c425da
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787321"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="8b48e-103">timeOffRequest: снижение</span><span class="sxs-lookup"><span data-stu-id="8b48e-103">timeOffRequest: decline</span></span>

<span data-ttu-id="8b48e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b48e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b48e-105">[Отклонение объекта timeoffrequest.](../resources/timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8b48e-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b48e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b48e-106">Permissions</span></span>

<span data-ttu-id="8b48e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b48e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b48e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b48e-109">Permission type</span></span>                        | <span data-ttu-id="8b48e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b48e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b48e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b48e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b48e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b48e-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8b48e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b48e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b48e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b48e-114">Not supported.</span></span> |
|<span data-ttu-id="8b48e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b48e-115">Application</span></span> | <span data-ttu-id="8b48e-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="8b48e-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="8b48e-117">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="8b48e-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="8b48e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b48e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="8b48e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b48e-119">Request headers</span></span>

| <span data-ttu-id="8b48e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8b48e-120">Name</span></span>          | <span data-ttu-id="8b48e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8b48e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8b48e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b48e-122">Authorization</span></span> | <span data-ttu-id="8b48e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b48e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b48e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b48e-125">Content-type</span></span> | <span data-ttu-id="8b48e-126">application-json.</span><span class="sxs-lookup"><span data-stu-id="8b48e-126">application-json.</span></span> <span data-ttu-id="8b48e-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8b48e-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b48e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b48e-128">Request body</span></span>

<span data-ttu-id="8b48e-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8b48e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b48e-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="8b48e-130">Parameter</span></span>    | <span data-ttu-id="8b48e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b48e-131">Type</span></span>        | <span data-ttu-id="8b48e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b48e-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8b48e-133">message</span><span class="sxs-lookup"><span data-stu-id="8b48e-133">message</span></span>|<span data-ttu-id="8b48e-134">String</span><span class="sxs-lookup"><span data-stu-id="8b48e-134">String</span></span>|<span data-ttu-id="8b48e-135">Пользовательское сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="8b48e-135">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="8b48e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b48e-136">Response</span></span>

<span data-ttu-id="8b48e-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b48e-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b48e-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b48e-139">Examples</span></span>

<span data-ttu-id="8b48e-140">Ниже приводится пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8b48e-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8b48e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b48e-141">Request</span></span>

<span data-ttu-id="8b48e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b48e-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b48e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b48e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="8b48e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b48e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b48e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b48e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8b48e-146">C#</span><span class="sxs-lookup"><span data-stu-id="8b48e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b48e-147">Java</span><span class="sxs-lookup"><span data-stu-id="8b48e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8b48e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b48e-148">Response</span></span>

<span data-ttu-id="8b48e-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8b48e-149">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


