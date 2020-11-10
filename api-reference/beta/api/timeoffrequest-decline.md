---
title: 'Тимеоффрекуест: отклонить'
description: Отклонить объект тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9fb4432cc9cf05689ec26a6b8ebe8b0447f33ca6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981363"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="6111c-103">Тимеоффрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="6111c-103">timeOffRequest: decline</span></span>

<span data-ttu-id="6111c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6111c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6111c-105">Отклонить объект [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="6111c-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6111c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6111c-106">Permissions</span></span>

<span data-ttu-id="6111c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6111c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6111c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6111c-109">Permission type</span></span>                        | <span data-ttu-id="6111c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6111c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6111c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6111c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6111c-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6111c-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6111c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6111c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6111c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6111c-114">Not supported.</span></span> |
|<span data-ttu-id="6111c-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6111c-115">Application</span></span> | <span data-ttu-id="6111c-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="6111c-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="6111c-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="6111c-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="6111c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6111c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="6111c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6111c-119">Request headers</span></span>

| <span data-ttu-id="6111c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6111c-120">Name</span></span>          | <span data-ttu-id="6111c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6111c-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6111c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6111c-122">Authorization</span></span> | <span data-ttu-id="6111c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6111c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6111c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6111c-125">Content-type</span></span> | <span data-ttu-id="6111c-126">приложение — JSON.</span><span class="sxs-lookup"><span data-stu-id="6111c-126">application-json.</span></span> <span data-ttu-id="6111c-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6111c-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6111c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6111c-128">Request body</span></span>

<span data-ttu-id="6111c-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6111c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6111c-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="6111c-130">Parameter</span></span>    | <span data-ttu-id="6111c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6111c-131">Type</span></span>        | <span data-ttu-id="6111c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6111c-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6111c-133">message</span><span class="sxs-lookup"><span data-stu-id="6111c-133">message</span></span>|<span data-ttu-id="6111c-134">String</span><span class="sxs-lookup"><span data-stu-id="6111c-134">String</span></span>|<span data-ttu-id="6111c-135">Настраиваемое сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="6111c-135">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="6111c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6111c-136">Response</span></span>

<span data-ttu-id="6111c-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6111c-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6111c-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="6111c-139">Examples</span></span>

<span data-ttu-id="6111c-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6111c-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6111c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6111c-141">Request</span></span>

<span data-ttu-id="6111c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6111c-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6111c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6111c-143">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="6111c-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6111c-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6111c-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6111c-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6111c-146">C#</span><span class="sxs-lookup"><span data-stu-id="6111c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6111c-147">Java</span><span class="sxs-lookup"><span data-stu-id="6111c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6111c-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6111c-148">Response</span></span>

<span data-ttu-id="6111c-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6111c-149">The following is an example of the response.</span></span>
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
  "description": "timeOffRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


