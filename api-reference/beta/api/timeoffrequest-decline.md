---
title: 'Тимеоффрекуест: отклонить'
description: Отклонить объект тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 468e4e05ace42405f216f6611c34560604a102c3
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154362"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="60ed8-103">Тимеоффрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="60ed8-103">timeOffRequest: decline</span></span>

<span data-ttu-id="60ed8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60ed8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60ed8-105">Отклонить объект [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="60ed8-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="60ed8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60ed8-106">Permissions</span></span>

<span data-ttu-id="60ed8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60ed8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60ed8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60ed8-109">Permission type</span></span>                        | <span data-ttu-id="60ed8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60ed8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="60ed8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60ed8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="60ed8-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ed8-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="60ed8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60ed8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60ed8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60ed8-114">Not supported.</span></span> |
|<span data-ttu-id="60ed8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60ed8-115">Application</span></span> | <span data-ttu-id="60ed8-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="60ed8-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="60ed8-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="60ed8-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="60ed8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60ed8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="60ed8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60ed8-119">Request headers</span></span>

| <span data-ttu-id="60ed8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="60ed8-120">Name</span></span>          | <span data-ttu-id="60ed8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="60ed8-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="60ed8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60ed8-122">Authorization</span></span> | <span data-ttu-id="60ed8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60ed8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60ed8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60ed8-125">Content-type</span></span> | <span data-ttu-id="60ed8-126">приложение — JSON.</span><span class="sxs-lookup"><span data-stu-id="60ed8-126">application-json.</span></span> <span data-ttu-id="60ed8-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="60ed8-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60ed8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60ed8-128">Request body</span></span>

<span data-ttu-id="60ed8-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="60ed8-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60ed8-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="60ed8-130">Parameter</span></span>    | <span data-ttu-id="60ed8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="60ed8-131">Type</span></span>        | <span data-ttu-id="60ed8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="60ed8-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="60ed8-133">message</span><span class="sxs-lookup"><span data-stu-id="60ed8-133">message</span></span>|<span data-ttu-id="60ed8-134">String</span><span class="sxs-lookup"><span data-stu-id="60ed8-134">String</span></span>|<span data-ttu-id="60ed8-135">Настраиваемое сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="60ed8-135">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="60ed8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="60ed8-136">Response</span></span>

<span data-ttu-id="60ed8-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="60ed8-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60ed8-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="60ed8-139">Examples</span></span>

<span data-ttu-id="60ed8-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="60ed8-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="60ed8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="60ed8-141">Request</span></span>

<span data-ttu-id="60ed8-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60ed8-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="60ed8-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="60ed8-143">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="60ed8-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60ed8-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60ed8-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60ed8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60ed8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="60ed8-146">Response</span></span>

<span data-ttu-id="60ed8-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="60ed8-147">The following is an example of the response.</span></span>
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
