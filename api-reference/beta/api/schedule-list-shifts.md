---
title: ПереЧисление смещений
description: Получение списка смен по расписанию.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 88010a0d5ce3c14a06938fe32fc9d212b29e1e0f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331425"
---
# <a name="list-shifts"></a><span data-ttu-id="90e12-103">ПереЧисление смещений</span><span class="sxs-lookup"><span data-stu-id="90e12-103">List shifts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="90e12-104">Получение списка экземпляров [смены](../resources/shift.md) в расписании. [](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="90e12-104">Get the list of [shift](../resources/shift.md) instances in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="90e12-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90e12-105">Permissions</span></span>

<span data-ttu-id="90e12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90e12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90e12-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90e12-108">Permission type</span></span>      | <span data-ttu-id="90e12-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90e12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90e12-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90e12-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90e12-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90e12-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="90e12-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90e12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90e12-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90e12-113">Not supported.</span></span>    |
|<span data-ttu-id="90e12-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90e12-114">Application</span></span> | <span data-ttu-id="90e12-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90e12-115">Not supported.</span></span> |

> <span data-ttu-id="90e12-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="90e12-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="90e12-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="90e12-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="90e12-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90e12-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90e12-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="90e12-119">Optional query parameters</span></span>
<span data-ttu-id="90e12-120">Этот метод поддерживает $filter [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="90e12-120">This method supports the $filter [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90e12-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90e12-121">Request headers</span></span>

| <span data-ttu-id="90e12-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90e12-122">Header</span></span>       | <span data-ttu-id="90e12-123">Значение</span><span class="sxs-lookup"><span data-stu-id="90e12-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90e12-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90e12-124">Authorization</span></span>  | <span data-ttu-id="90e12-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90e12-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="90e12-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="90e12-127">Content-Type</span></span>  | <span data-ttu-id="90e12-128">application/json</span><span class="sxs-lookup"><span data-stu-id="90e12-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90e12-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90e12-129">Request body</span></span>
<span data-ttu-id="90e12-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90e12-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90e12-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="90e12-131">Response</span></span>

<span data-ttu-id="90e12-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [SHIFT](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90e12-132">If successful, this method returns a `200 OK` response code and a collection of [shift](../resources/shift.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90e12-133">Пример</span><span class="sxs-lookup"><span data-stu-id="90e12-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="90e12-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="90e12-134">Request</span></span>

<span data-ttu-id="90e12-135">Ниже приведен пример запроса, который получает все объекты **SHIFT** с общей версией и черновой версией в диапазоне от 11 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="90e12-135">The following is an example of a request that gets all **shift** objects that have a shared version and a draft version between March 11 - March 18, 2019.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-list-shifts"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts?$filter=sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z
```

#### <a name="response"></a><span data-ttu-id="90e12-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="90e12-136">Response</span></span>

<span data-ttu-id="90e12-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90e12-137">The following is an example of the response.</span></span> 

><span data-ttu-id="90e12-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90e12-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of shifts in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
