---
title: Список Тимеоффреасонс
description: Получение списка Тимеоффреасонс по расписанию.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 78e2d91dd878c2ad4828ad5fdf25bc43e7b61dc8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331553"
---
# <a name="list-timeoffreasons"></a><span data-ttu-id="d2f11-103">Список Тимеоффреасонс</span><span class="sxs-lookup"><span data-stu-id="d2f11-103">List timeOffReasons</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="d2f11-104">Получение списка [тимеоффреасонс](../resources/timeoffreason.md) по расписанию. [](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="d2f11-104">Get the list of [timeOffReasons](../resources/timeoffreason.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2f11-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f11-105">Permissions</span></span>

<span data-ttu-id="d2f11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2f11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2f11-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f11-108">Permission type</span></span>      | <span data-ttu-id="d2f11-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2f11-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2f11-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2f11-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2f11-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f11-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2f11-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2f11-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2f11-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f11-113">Not supported.</span></span>    |
|<span data-ttu-id="d2f11-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2f11-114">Application</span></span> | <span data-ttu-id="d2f11-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f11-115">Not supported.</span></span> |

> <span data-ttu-id="d2f11-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="d2f11-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d2f11-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="d2f11-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d2f11-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2f11-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="d2f11-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2f11-119">Request headers</span></span>

| <span data-ttu-id="d2f11-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2f11-120">Header</span></span>       | <span data-ttu-id="d2f11-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d2f11-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2f11-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2f11-122">Authorization</span></span>  | <span data-ttu-id="d2f11-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2f11-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2f11-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2f11-125">Content-Type</span></span>  | <span data-ttu-id="d2f11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2f11-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2f11-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2f11-127">Request body</span></span>
<span data-ttu-id="d2f11-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2f11-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2f11-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2f11-129">Response</span></span>

<span data-ttu-id="d2f11-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тимеоффреасон](../resources/timeoffreason.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f11-130">If successful, this method returns a `200 OK` response code and a collection of [timeOffReason](../resources/timeoffreason.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2f11-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d2f11-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d2f11-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2f11-132">Request</span></span>

<span data-ttu-id="d2f11-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2f11-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-list-timeoffreasons"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
```

#### <a name="response"></a><span data-ttu-id="d2f11-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f11-134">Response</span></span>

<span data-ttu-id="d2f11-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f11-135">The following is an example of the response.</span></span> 

><span data-ttu-id="d2f11-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2f11-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of timeOffReason in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
