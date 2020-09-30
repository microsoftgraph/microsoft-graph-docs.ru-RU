---
title: Создание Оффершифтрекуест
description: Создайте экземпляр объекта Оффершифтрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 85b5b725860671c2c951ffb359d6b6cdccccf408
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313725"
---
# <a name="create-offershiftrequest"></a><span data-ttu-id="f9dec-103">Создание Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="f9dec-103">Create offerShiftRequest</span></span>

<span data-ttu-id="f9dec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9dec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9dec-105">Создайте экземпляр объекта [оффершифтрекуест](../resources/offershiftrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f9dec-105">Create an instance of an [offerShiftRequest](../resources/offershiftrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9dec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9dec-106">Permissions</span></span>

<span data-ttu-id="f9dec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9dec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9dec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9dec-109">Permission type</span></span>                        | <span data-ttu-id="f9dec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9dec-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f9dec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9dec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9dec-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f9dec-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f9dec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9dec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9dec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9dec-114">Not supported.</span></span> |
| <span data-ttu-id="f9dec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9dec-115">Application</span></span>                            | <span data-ttu-id="f9dec-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9dec-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9dec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9dec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="request-headers"></a><span data-ttu-id="f9dec-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9dec-118">Request headers</span></span>

| <span data-ttu-id="f9dec-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f9dec-119">Name</span></span>      |<span data-ttu-id="f9dec-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f9dec-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9dec-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9dec-121">Authorization</span></span> | <span data-ttu-id="f9dec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9dec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9dec-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9dec-124">Request body</span></span>
<span data-ttu-id="f9dec-125">Укажите новый объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9dec-125">Provide the new [offershiftrequest](../resources/offershiftrequest.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9dec-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9dec-126">Response</span></span>

<span data-ttu-id="f9dec-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9dec-127">If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9dec-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f9dec-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9dec-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9dec-129">Request</span></span>

<span data-ttu-id="f9dec-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9dec-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9dec-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9dec-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
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
# <a name="c"></a>[<span data-ttu-id="f9dec-132">C#</span><span class="sxs-lookup"><span data-stu-id="f9dec-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9dec-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9dec-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9dec-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9dec-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f9dec-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9dec-135">Response</span></span>

<span data-ttu-id="f9dec-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f9dec-136">The following is an example of the response.</span></span>

> <span data-ttu-id="f9dec-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9dec-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


