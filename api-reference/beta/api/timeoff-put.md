---
title: Замена Тимеофф
description: Замена существующего Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: baa95edcece586a481a538d2f0ff68a309c8ce10
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544353"
---
# <a name="replace-timeoff"></a><span data-ttu-id="a3b65-103">Замена Тимеофф</span><span class="sxs-lookup"><span data-stu-id="a3b65-103">Replace timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3b65-104">Замена существующего [тимеофф](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="a3b65-104">Replace an existing [timeOff](../resources/timeoff.md).</span></span>

<span data-ttu-id="a3b65-105">Если указанный [тимеофф](../resources/timeoff.md) не существует, этот метод возвращает значение `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="a3b65-105">If the specified [timeOff](../resources/timeoff.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3b65-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3b65-106">Permissions</span></span>

<span data-ttu-id="a3b65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3b65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3b65-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3b65-109">Permission type</span></span>      | <span data-ttu-id="a3b65-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3b65-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3b65-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3b65-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a3b65-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3b65-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3b65-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3b65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3b65-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3b65-114">Not supported.</span></span>    |
|<span data-ttu-id="a3b65-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3b65-115">Application</span></span> | <span data-ttu-id="a3b65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3b65-116">Not supported.</span></span> |

> <span data-ttu-id="a3b65-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="a3b65-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a3b65-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="a3b65-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a3b65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3b65-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="a3b65-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3b65-120">Request headers</span></span>

| <span data-ttu-id="a3b65-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3b65-121">Header</span></span>       | <span data-ttu-id="a3b65-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a3b65-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a3b65-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3b65-123">Authorization</span></span>  | <span data-ttu-id="a3b65-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3b65-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a3b65-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3b65-126">Content-Type</span></span>  | <span data-ttu-id="a3b65-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a3b65-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3b65-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3b65-128">Request body</span></span>

<span data-ttu-id="a3b65-129">В тексте запроса добавьте представление объекта [Тимеофф](../resources/timeoff.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3b65-129">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a3b65-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3b65-130">Response</span></span>

<span data-ttu-id="a3b65-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3b65-131">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3b65-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a3b65-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a3b65-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3b65-133">Request</span></span>

<span data-ttu-id="a3b65-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3b65-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
Content-type: application/json
Prefer: return=representation

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

#### <a name="response"></a><span data-ttu-id="a3b65-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3b65-135">Response</span></span>

<span data-ttu-id="a3b65-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a3b65-136">The following is an example of the response.</span></span> 

><span data-ttu-id="a3b65-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3b65-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Replace an existing timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
