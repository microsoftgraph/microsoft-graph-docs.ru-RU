---
title: Создание Тимеофф
description: Создание нового Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c929f28663fafba30f95a3e00e517a958237143
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978067"
---
# <a name="create-timeoff"></a><span data-ttu-id="f25a1-103">Создание Тимеофф</span><span class="sxs-lookup"><span data-stu-id="f25a1-103">Create timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f25a1-104">Создайте новый экземпляр [тимеофф](../resources/timeoff.md) в расписании [](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="f25a1-104">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f25a1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f25a1-105">Permissions</span></span>

<span data-ttu-id="f25a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f25a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f25a1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f25a1-108">Permission type</span></span>      | <span data-ttu-id="f25a1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f25a1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f25a1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f25a1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f25a1-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f25a1-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f25a1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f25a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f25a1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f25a1-113">Not supported.</span></span>    |
|<span data-ttu-id="f25a1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f25a1-114">Application</span></span> | <span data-ttu-id="f25a1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f25a1-115">Not supported.</span></span> |

> <span data-ttu-id="f25a1-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f25a1-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f25a1-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="f25a1-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f25a1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f25a1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="f25a1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f25a1-119">Request headers</span></span>

| <span data-ttu-id="f25a1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f25a1-120">Header</span></span>       | <span data-ttu-id="f25a1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f25a1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f25a1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f25a1-122">Authorization</span></span>  | <span data-ttu-id="f25a1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f25a1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f25a1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f25a1-125">Content-Type</span></span>  | <span data-ttu-id="f25a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f25a1-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="f25a1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f25a1-127">Response</span></span>

<span data-ttu-id="f25a1-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f25a1-128">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f25a1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f25a1-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f25a1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f25a1-130">Request</span></span>

<span data-ttu-id="f25a1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f25a1-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f25a1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f25a1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-post"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff
Content-type: application/json

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f25a1-133">C#</span><span class="sxs-lookup"><span data-stu-id="f25a1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f25a1-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="f25a1-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f25a1-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f25a1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f25a1-136">Java</span><span class="sxs-lookup"><span data-stu-id="f25a1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f25a1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f25a1-137">Response</span></span>

<span data-ttu-id="f25a1-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f25a1-138">The following is an example of the response.</span></span> 

><span data-ttu-id="f25a1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f25a1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type":"microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
