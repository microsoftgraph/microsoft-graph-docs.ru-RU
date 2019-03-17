---
title: Создание смены
description: Создайте новую смену.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ae7ff2f598373d58b2a01b678dbb70ae8e290b2d
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657548"
---
# <a name="create-shift"></a><span data-ttu-id="0c90e-103">Создание смены</span><span class="sxs-lookup"><span data-stu-id="0c90e-103">Create shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c90e-104">Создайте новый экземпляр [SHIFT](../resources/shift.md) в расписании [](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="0c90e-104">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c90e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c90e-105">Permissions</span></span>

<span data-ttu-id="0c90e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c90e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c90e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c90e-108">Permission type</span></span>      | <span data-ttu-id="0c90e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c90e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c90e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c90e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c90e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c90e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c90e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c90e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c90e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c90e-113">Not supported.</span></span>    |
|<span data-ttu-id="0c90e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c90e-114">Application</span></span> | <span data-ttu-id="0c90e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c90e-115">Not supported.</span></span> |

> <span data-ttu-id="0c90e-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="0c90e-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0c90e-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="0c90e-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0c90e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c90e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="0c90e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c90e-119">Request headers</span></span>

| <span data-ttu-id="0c90e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c90e-120">Header</span></span>       | <span data-ttu-id="0c90e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0c90e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c90e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c90e-122">Authorization</span></span>  | <span data-ttu-id="0c90e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c90e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0c90e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c90e-125">Content-Type</span></span>  | <span data-ttu-id="0c90e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c90e-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="0c90e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c90e-127">Response</span></span>

<span data-ttu-id="0c90e-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [сдвига](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c90e-128">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c90e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0c90e-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0c90e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c90e-130">Request</span></span>

<span data-ttu-id="0c90e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c90e-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-post-shifts"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts
Content-type: application/json

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```

#### <a name="response"></a><span data-ttu-id="0c90e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c90e-132">Response</span></span>

<span data-ttu-id="0c90e-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c90e-133">The following is an example of the response.</span></span> 

><span data-ttu-id="0c90e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c90e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-post-shifts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
