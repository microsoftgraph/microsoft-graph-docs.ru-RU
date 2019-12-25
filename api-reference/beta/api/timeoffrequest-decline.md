---
title: 'Тимеоффрекуест: отклонить'
description: Отклонить объект тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 69dce3ef9a9486e204eca58421aff606b56385aa
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863630"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="8ad1b-103">Тимеоффрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="8ad1b-103">timeOffRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ad1b-104">Отклонить объект [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="8ad1b-104">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ad1b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ad1b-105">Permissions</span></span>

<span data-ttu-id="8ad1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ad1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ad1b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ad1b-108">Permission type</span></span>                        | <span data-ttu-id="8ad1b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ad1b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8ad1b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ad1b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ad1b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ad1b-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8ad1b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ad1b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ad1b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-113">Not supported.</span></span> |
|<span data-ttu-id="8ad1b-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="8ad1b-114">Application</span></span> | <span data-ttu-id="8ad1b-115">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="8ad1b-115">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="8ad1b-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="8ad1b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ad1b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/timeOffRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="8ad1b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ad1b-118">Request headers</span></span>

| <span data-ttu-id="8ad1b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8ad1b-119">Name</span></span>          | <span data-ttu-id="8ad1b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8ad1b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8ad1b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ad1b-121">Authorization</span></span> | <span data-ttu-id="8ad1b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ad1b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ad1b-124">Content-type</span></span> | <span data-ttu-id="8ad1b-125">приложение — JSON.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-125">application-json.</span></span> <span data-ttu-id="8ad1b-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ad1b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ad1b-127">Request body</span></span>

<span data-ttu-id="8ad1b-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ad1b-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="8ad1b-129">Parameter</span></span>    | <span data-ttu-id="8ad1b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8ad1b-130">Type</span></span>        | <span data-ttu-id="8ad1b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8ad1b-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ad1b-132">message</span><span class="sxs-lookup"><span data-stu-id="8ad1b-132">message</span></span>|<span data-ttu-id="8ad1b-133">String</span><span class="sxs-lookup"><span data-stu-id="8ad1b-133">String</span></span>|<span data-ttu-id="8ad1b-134">Настраиваемое сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-134">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="8ad1b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ad1b-135">Response</span></span>

<span data-ttu-id="8ad1b-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ad1b-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="8ad1b-138">Examples</span></span>

<span data-ttu-id="8ad1b-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-139">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8ad1b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ad1b-140">Request</span></span>

<span data-ttu-id="8ad1b-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8ad1b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ad1b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ad1b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ad1b-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ad1b-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ad1b-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8ad1b-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ad1b-145">Response</span></span>

<span data-ttu-id="8ad1b-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8ad1b-146">The following is an example of the response.</span></span>
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
