---
title: Получение Тимеоффреасон
description: Получение Тимеоффреасон по ИДЕНТИФИКАТОРу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 54baa557317675b198b1d557e81cd7a675d82fee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544338"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="4eb3f-103">Получение Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="4eb3f-103">Get timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eb3f-104">Получение свойств и связей объекта [тимеоффреасон](../resources/timeoffreason.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-104">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="4eb3f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4eb3f-105">Permissions</span></span>

<span data-ttu-id="4eb3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eb3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eb3f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4eb3f-108">Permission type</span></span>      | <span data-ttu-id="4eb3f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4eb3f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4eb3f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4eb3f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4eb3f-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eb3f-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4eb3f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4eb3f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eb3f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-113">Not supported.</span></span>    |
|<span data-ttu-id="4eb3f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4eb3f-114">Application</span></span> | <span data-ttu-id="4eb3f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-115">Not supported.</span></span> |

> <span data-ttu-id="4eb3f-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4eb3f-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4eb3f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eb3f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="4eb3f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4eb3f-119">Request headers</span></span>

| <span data-ttu-id="4eb3f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4eb3f-120">Header</span></span>       | <span data-ttu-id="4eb3f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4eb3f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4eb3f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4eb3f-122">Authorization</span></span>  | <span data-ttu-id="4eb3f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4eb3f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4eb3f-125">Content-Type</span></span>  | <span data-ttu-id="4eb3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4eb3f-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4eb3f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4eb3f-127">Request body</span></span>
<span data-ttu-id="4eb3f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eb3f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4eb3f-129">Response</span></span>

<span data-ttu-id="4eb3f-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеоффреасон](../resources/timeoffreason.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-130">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eb3f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4eb3f-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4eb3f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eb3f-132">Request</span></span>

<span data-ttu-id="4eb3f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

#### <a name="response"></a><span data-ttu-id="4eb3f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eb3f-134">Response</span></span>

<span data-ttu-id="4eb3f-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-135">The following is an example of the response.</span></span> 

><span data-ttu-id="4eb3f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4eb3f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeOffReason by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
