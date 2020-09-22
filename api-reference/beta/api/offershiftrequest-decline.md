---
title: 'Оффершифтрекуест: отклонить'
description: Отклонить запрос на смену предложения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 315ff8ba05f2fad246938f1913458a726ce30356
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064684"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="7ef43-103">Оффершифтрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="7ef43-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="7ef43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ef43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ef43-105">Отклонить объект [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="7ef43-105">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ef43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ef43-106">Permissions</span></span>

<span data-ttu-id="7ef43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ef43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ef43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ef43-109">Permission type</span></span>                        | <span data-ttu-id="7ef43-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ef43-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7ef43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ef43-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ef43-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef43-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="7ef43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ef43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ef43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ef43-114">Not supported.</span></span> |
| <span data-ttu-id="7ef43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ef43-115">Application</span></span>                            | <span data-ttu-id="7ef43-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="7ef43-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="7ef43-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="7ef43-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="7ef43-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ef43-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="7ef43-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ef43-119">Request headers</span></span>

| <span data-ttu-id="7ef43-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7ef43-120">Name</span></span>          | <span data-ttu-id="7ef43-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef43-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7ef43-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ef43-122">Authorization</span></span> | <span data-ttu-id="7ef43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ef43-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ef43-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ef43-125">Content-type</span></span> | <span data-ttu-id="7ef43-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ef43-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ef43-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ef43-128">Request body</span></span>

<span data-ttu-id="7ef43-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7ef43-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7ef43-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="7ef43-130">Parameter</span></span>    | <span data-ttu-id="7ef43-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7ef43-131">Type</span></span>        | <span data-ttu-id="7ef43-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef43-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ef43-133">message</span><span class="sxs-lookup"><span data-stu-id="7ef43-133">message</span></span>|<span data-ttu-id="7ef43-134">String</span><span class="sxs-lookup"><span data-stu-id="7ef43-134">String</span></span>|<span data-ttu-id="7ef43-135">Настраиваемое сообщение, отправленное при отклонении.</span><span class="sxs-lookup"><span data-stu-id="7ef43-135">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="7ef43-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ef43-136">Response</span></span>

<span data-ttu-id="7ef43-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ef43-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ef43-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="7ef43-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7ef43-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ef43-140">Request</span></span>

<span data-ttu-id="7ef43-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ef43-141">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ef43-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ef43-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="javascript"></a>[<span data-ttu-id="7ef43-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ef43-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7ef43-144">C#</span><span class="sxs-lookup"><span data-stu-id="7ef43-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ef43-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ef43-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7ef43-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ef43-146">Response</span></span>

<span data-ttu-id="7ef43-147">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ef43-147">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


