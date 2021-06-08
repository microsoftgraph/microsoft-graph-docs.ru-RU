---
title: 'offerShiftRequest: снижение'
description: Отклонение запроса на перенос предложения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 366fa33786deaeefe12beced8fdda66e61fe7f4f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786490"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="18454-103">offerShiftRequest: снижение</span><span class="sxs-lookup"><span data-stu-id="18454-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="18454-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18454-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18454-105">Отклонение [объекта offershiftrequest.](../resources/offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="18454-105">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="18454-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18454-106">Permissions</span></span>

<span data-ttu-id="18454-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18454-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18454-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18454-109">Permission type</span></span>                        | <span data-ttu-id="18454-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18454-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="18454-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18454-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="18454-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18454-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="18454-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18454-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18454-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18454-114">Not supported.</span></span> |
| <span data-ttu-id="18454-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="18454-115">Application</span></span>                            | <span data-ttu-id="18454-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18454-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18454-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18454-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="18454-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18454-118">Request headers</span></span>

| <span data-ttu-id="18454-119">Имя</span><span class="sxs-lookup"><span data-stu-id="18454-119">Name</span></span>          | <span data-ttu-id="18454-120">Описание</span><span class="sxs-lookup"><span data-stu-id="18454-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="18454-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18454-121">Authorization</span></span> | <span data-ttu-id="18454-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18454-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18454-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18454-124">Content-type</span></span> | <span data-ttu-id="18454-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18454-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18454-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18454-127">Request body</span></span>

<span data-ttu-id="18454-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="18454-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18454-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="18454-129">Parameter</span></span>    | <span data-ttu-id="18454-130">Тип</span><span class="sxs-lookup"><span data-stu-id="18454-130">Type</span></span>        | <span data-ttu-id="18454-131">Описание</span><span class="sxs-lookup"><span data-stu-id="18454-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="18454-132">message</span><span class="sxs-lookup"><span data-stu-id="18454-132">message</span></span>|<span data-ttu-id="18454-133">String</span><span class="sxs-lookup"><span data-stu-id="18454-133">String</span></span>|<span data-ttu-id="18454-134">Настраиваемые сообщения, отправленные при отклонении.</span><span class="sxs-lookup"><span data-stu-id="18454-134">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="18454-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="18454-135">Response</span></span>

<span data-ttu-id="18454-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18454-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18454-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="18454-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18454-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="18454-139">Request</span></span>

<span data-ttu-id="18454-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18454-140">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18454-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="18454-141">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="18454-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18454-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="18454-143">C#</span><span class="sxs-lookup"><span data-stu-id="18454-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18454-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18454-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18454-145">Java</span><span class="sxs-lookup"><span data-stu-id="18454-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18454-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="18454-146">Response</span></span>

<span data-ttu-id="18454-147">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18454-147">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


