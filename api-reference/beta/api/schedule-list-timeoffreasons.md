---
title: Список Тимеоффреасонс
description: Получение списка Тимеоффреасонс по расписанию.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 719123af222691b997685db7fb7274a4c60bfbae
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866986"
---
# <a name="list-timeoffreasons"></a><span data-ttu-id="e1af3-103">Список Тимеоффреасонс</span><span class="sxs-lookup"><span data-stu-id="e1af3-103">List timeOffReasons</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="e1af3-104">Получение списка [тимеоффреасонс](../resources/timeoffreason.md) по [расписанию](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="e1af3-104">Get the list of [timeOffReasons](../resources/timeoffreason.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e1af3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1af3-105">Permissions</span></span>

<span data-ttu-id="e1af3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1af3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1af3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1af3-108">Permission type</span></span>      | <span data-ttu-id="e1af3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1af3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1af3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1af3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1af3-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1af3-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1af3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1af3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1af3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1af3-113">Not supported.</span></span>    |
|<span data-ttu-id="e1af3-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="e1af3-114">Application</span></span> | <span data-ttu-id="e1af3-115">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="e1af3-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="e1af3-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="e1af3-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="e1af3-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="e1af3-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e1af3-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="e1af3-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e1af3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1af3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="e1af3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1af3-120">Request headers</span></span>

| <span data-ttu-id="e1af3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1af3-121">Header</span></span>       | <span data-ttu-id="e1af3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1af3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1af3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1af3-123">Authorization</span></span>  | <span data-ttu-id="e1af3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1af3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1af3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1af3-126">Request body</span></span>
<span data-ttu-id="e1af3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1af3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1af3-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1af3-128">Response</span></span>

<span data-ttu-id="e1af3-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тимеоффреасон](../resources/timeoffreason.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1af3-129">If successful, this method returns a `200 OK` response code and a collection of [timeOffReason](../resources/timeoffreason.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1af3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e1af3-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e1af3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1af3-131">Request</span></span>

<span data-ttu-id="e1af3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1af3-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e1af3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1af3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timeoffreasons"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1af3-134">C#</span><span class="sxs-lookup"><span data-stu-id="e1af3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1af3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1af3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1af3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1af3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e1af3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1af3-137">Response</span></span>

<span data-ttu-id="e1af3-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1af3-138">The following is an example of the response.</span></span> 

><span data-ttu-id="e1af3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1af3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
  ]
}
-->
