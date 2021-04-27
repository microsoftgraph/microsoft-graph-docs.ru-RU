---
title: Создание offerShiftRequest
description: Создание экземпляра offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 06f9e15e6edf50156a100039c4eac7e0e7e79ce7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038269"
---
# <a name="create-offershiftrequest"></a><span data-ttu-id="1449d-103">Создание offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="1449d-103">Create offerShiftRequest</span></span>

<span data-ttu-id="1449d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1449d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1449d-105">Создание экземпляра [offerShiftRequest](../resources/offershiftrequest.md).</span><span class="sxs-lookup"><span data-stu-id="1449d-105">Create an instance of an [offerShiftRequest](../resources/offershiftrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1449d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1449d-106">Permissions</span></span>

<span data-ttu-id="1449d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1449d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1449d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1449d-109">Permission type</span></span>                        | <span data-ttu-id="1449d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1449d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1449d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1449d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1449d-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1449d-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1449d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1449d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1449d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1449d-114">Not supported.</span></span> |
| <span data-ttu-id="1449d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1449d-115">Application</span></span>                            | <span data-ttu-id="1449d-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1449d-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1449d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1449d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="request-headers"></a><span data-ttu-id="1449d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1449d-118">Request headers</span></span>

| <span data-ttu-id="1449d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1449d-119">Name</span></span>      |<span data-ttu-id="1449d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1449d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1449d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1449d-121">Authorization</span></span> | <span data-ttu-id="1449d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1449d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1449d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1449d-124">Request body</span></span>
<span data-ttu-id="1449d-125">Предоставление нового [объекта offershiftrequest](../resources/offershiftrequest.md) в теле запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1449d-125">Provide the new [offershiftrequest](../resources/offershiftrequest.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1449d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1449d-126">Response</span></span>

<span data-ttu-id="1449d-127">В случае успеха этот метод возвращает код отклика и `200 OK` [объект offerShiftRequest](../resources/offershiftrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1449d-127">If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1449d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="1449d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1449d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1449d-129">Request</span></span>

<span data-ttu-id="1449d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1449d-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1449d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1449d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest_3"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/offershiftrequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c"
}
```
# <a name="c"></a>[<span data-ttu-id="1449d-132">C#</span><span class="sxs-lookup"><span data-stu-id="1449d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1449d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1449d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1449d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1449d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1449d-135">Java</span><span class="sxs-lookup"><span data-stu-id="1449d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1449d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1449d-136">Response</span></span>

<span data-ttu-id="1449d-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1449d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="1449d-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1449d-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.etag": "\"4000ee23-0000-0700-0000-5d1415f60000\"",
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "createdDateTime": "2019-09-27T01:01:04.566Z",
  "lastModifiedDateTime": "2019-09-28T01:03:48.874Z",
  "assignedTo": "recipient",
  "state": "pending",
  "senderDateTime": "2019-09-27T01:01:04.566",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "senderUserId": "a4704dd0-3f4c-4f2c-9bb5-8cc575703f30",
  "managerActionDateTime": null,
  "managerActionMessage": null,
  "managerUserId": null,
  "recipientActionDateTime": null,
  "recipientActionMessage": null,
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
      "displayName": "Employee 1"
    }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get offerShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


