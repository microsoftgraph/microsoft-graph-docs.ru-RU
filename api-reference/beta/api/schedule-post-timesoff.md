---
title: Создание Тимеофф
description: Создание нового Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: df954be9d07797e663b205af6d4dc1ef5dfb20ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545642"
---
# <a name="create-timeoff"></a><span data-ttu-id="8c7c3-103">Создание Тимеофф</span><span class="sxs-lookup"><span data-stu-id="8c7c3-103">Create timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c7c3-104">Создайте новый экземпляр [тимеофф](../resources/timeoff.md) в расписании [](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="8c7c3-104">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c7c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c7c3-105">Permissions</span></span>

<span data-ttu-id="8c7c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c7c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c7c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c7c3-108">Permission type</span></span>      | <span data-ttu-id="8c7c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c7c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c7c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c7c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c7c3-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c7c3-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8c7c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c7c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c7c3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c7c3-113">Not supported.</span></span>    |
|<span data-ttu-id="8c7c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c7c3-114">Application</span></span> | <span data-ttu-id="8c7c3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c7c3-115">Not supported.</span></span> |

> <span data-ttu-id="8c7c3-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="8c7c3-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8c7c3-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="8c7c3-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8c7c3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c7c3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="8c7c3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c7c3-119">Request headers</span></span>

| <span data-ttu-id="8c7c3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c7c3-120">Header</span></span>       | <span data-ttu-id="8c7c3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8c7c3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c7c3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c7c3-122">Authorization</span></span>  | <span data-ttu-id="8c7c3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c7c3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8c7c3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c7c3-125">Content-Type</span></span>  | <span data-ttu-id="8c7c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c7c3-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="8c7c3-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c7c3-127">Response</span></span>

<span data-ttu-id="8c7c3-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c7c3-128">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c7c3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8c7c3-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8c7c3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c7c3-130">Request</span></span>

<span data-ttu-id="8c7c3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c7c3-131">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="8c7c3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c7c3-132">Response</span></span>

<span data-ttu-id="8c7c3-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c7c3-133">The following is an example of the response.</span></span> 

><span data-ttu-id="8c7c3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c7c3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "schedule-post-timesoff"
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
    "Error: /api-reference/beta/api/schedule-post-timesoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
