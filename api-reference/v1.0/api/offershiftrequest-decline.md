---
title: 'offerShiftRequest: снижение'
description: Отклонение запроса на перенос предложения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9cdb5fbe381008b4146d649fb862b25a3687c251
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786334"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="68b15-103">offerShiftRequest: снижение</span><span class="sxs-lookup"><span data-stu-id="68b15-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="68b15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68b15-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68b15-105">Отклонение [объекта offerShiftRequest.](../resources/offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="68b15-105">Decline an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="68b15-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68b15-106">Permissions</span></span>

<span data-ttu-id="68b15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68b15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68b15-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68b15-109">Permission type</span></span>                        | <span data-ttu-id="68b15-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68b15-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="68b15-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68b15-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="68b15-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68b15-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="68b15-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68b15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68b15-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68b15-114">Not supported.</span></span> |
| <span data-ttu-id="68b15-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68b15-115">Application</span></span>                            | <span data-ttu-id="68b15-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68b15-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68b15-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68b15-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="68b15-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68b15-118">Request headers</span></span>

| <span data-ttu-id="68b15-119">Имя</span><span class="sxs-lookup"><span data-stu-id="68b15-119">Name</span></span>          | <span data-ttu-id="68b15-120">Описание</span><span class="sxs-lookup"><span data-stu-id="68b15-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="68b15-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68b15-121">Authorization</span></span> | <span data-ttu-id="68b15-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68b15-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="68b15-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68b15-124">Content-type</span></span> | <span data-ttu-id="68b15-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68b15-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68b15-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68b15-127">Request body</span></span>

<span data-ttu-id="68b15-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="68b15-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="68b15-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="68b15-129">Parameter</span></span>    | <span data-ttu-id="68b15-130">Тип</span><span class="sxs-lookup"><span data-stu-id="68b15-130">Type</span></span>        | <span data-ttu-id="68b15-131">Описание</span><span class="sxs-lookup"><span data-stu-id="68b15-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="68b15-132">message</span><span class="sxs-lookup"><span data-stu-id="68b15-132">message</span></span>|<span data-ttu-id="68b15-133">String</span><span class="sxs-lookup"><span data-stu-id="68b15-133">String</span></span>|<span data-ttu-id="68b15-134">Настраиваемые сообщения, отправленные при отклонении.</span><span class="sxs-lookup"><span data-stu-id="68b15-134">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="68b15-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="68b15-135">Response</span></span>

<span data-ttu-id="68b15-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="68b15-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68b15-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="68b15-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68b15-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="68b15-139">Request</span></span>

<span data-ttu-id="68b15-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68b15-140">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="68b15-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="68b15-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="c"></a>[<span data-ttu-id="68b15-142">C#</span><span class="sxs-lookup"><span data-stu-id="68b15-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68b15-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68b15-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68b15-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68b15-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68b15-145">Java</span><span class="sxs-lookup"><span data-stu-id="68b15-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="68b15-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="68b15-146">Response</span></span>

<span data-ttu-id="68b15-147">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68b15-147">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

