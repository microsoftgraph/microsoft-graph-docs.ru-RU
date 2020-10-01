---
title: 'Оффершифтрекуест: отклонить'
description: Отклонить запрос на смену предложения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 54c33624d924f9f424a99ff0668f8c1f7dd9c37a
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313676"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="ba7bb-103">Оффершифтрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="ba7bb-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="ba7bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba7bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba7bb-105">Отклонить объект [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ba7bb-105">Decline an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba7bb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba7bb-106">Permissions</span></span>

<span data-ttu-id="ba7bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba7bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba7bb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba7bb-109">Permission type</span></span>                        | <span data-ttu-id="ba7bb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba7bb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba7bb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba7bb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba7bb-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ba7bb-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ba7bb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba7bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba7bb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba7bb-114">Not supported.</span></span> |
| <span data-ttu-id="ba7bb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba7bb-115">Application</span></span>                            | <span data-ttu-id="ba7bb-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba7bb-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba7bb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba7bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="ba7bb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba7bb-118">Request headers</span></span>

| <span data-ttu-id="ba7bb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ba7bb-119">Name</span></span>          | <span data-ttu-id="ba7bb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ba7bb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ba7bb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba7bb-121">Authorization</span></span> | <span data-ttu-id="ba7bb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba7bb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba7bb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba7bb-124">Content-type</span></span> | <span data-ttu-id="ba7bb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba7bb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba7bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba7bb-127">Request body</span></span>

<span data-ttu-id="ba7bb-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ba7bb-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ba7bb-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="ba7bb-129">Parameter</span></span>    | <span data-ttu-id="ba7bb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ba7bb-130">Type</span></span>        | <span data-ttu-id="ba7bb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ba7bb-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba7bb-132">message</span><span class="sxs-lookup"><span data-stu-id="ba7bb-132">message</span></span>|<span data-ttu-id="ba7bb-133">String</span><span class="sxs-lookup"><span data-stu-id="ba7bb-133">String</span></span>|<span data-ttu-id="ba7bb-134">Настраиваемое сообщение, отправленное при отклонении.</span><span class="sxs-lookup"><span data-stu-id="ba7bb-134">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="ba7bb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba7bb-135">Response</span></span>

<span data-ttu-id="ba7bb-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba7bb-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba7bb-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba7bb-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba7bb-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba7bb-139">Request</span></span>

<span data-ttu-id="ba7bb-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba7bb-140">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba7bb-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba7bb-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ba7bb-142">C#</span><span class="sxs-lookup"><span data-stu-id="ba7bb-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba7bb-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba7bb-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba7bb-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba7bb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba7bb-145">Java</span><span class="sxs-lookup"><span data-stu-id="ba7bb-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="ba7bb-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba7bb-146">Response</span></span>

<span data-ttu-id="ba7bb-147">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba7bb-147">The following example shows the response.</span></span>
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

