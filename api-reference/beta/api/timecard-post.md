---
title: Создание timeCard
description: Создайте экземпляр timeCard в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e1a03dd2139070fa06156689bf332d0e7c1a3dcb
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870096"
---
# <a name="create-timecard"></a><span data-ttu-id="226fa-103">Создание timeCard</span><span class="sxs-lookup"><span data-stu-id="226fa-103">Create timeCard</span></span>

<span data-ttu-id="226fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="226fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="226fa-105">Создание [экземпляра timeCard](../resources/timeCard.md) в [расписании.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="226fa-105">Create a [timeCard](../resources/timeCard.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="226fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="226fa-106">Permissions</span></span>

<span data-ttu-id="226fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="226fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="226fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="226fa-109">Permission type</span></span>      | <span data-ttu-id="226fa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="226fa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="226fa-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="226fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="226fa-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="226fa-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="226fa-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="226fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="226fa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="226fa-114">Not supported.</span></span>    |
|<span data-ttu-id="226fa-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="226fa-115">Application</span></span> | <span data-ttu-id="226fa-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="226fa-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="226fa-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="226fa-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="226fa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="226fa-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards
```

## <a name="request-headers"></a><span data-ttu-id="226fa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="226fa-119">Request headers</span></span>

| <span data-ttu-id="226fa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="226fa-120">Header</span></span>       | <span data-ttu-id="226fa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="226fa-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="226fa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="226fa-122">Authorization</span></span>  | <span data-ttu-id="226fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="226fa-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="226fa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="226fa-125">Content-type</span></span> | <span data-ttu-id="226fa-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="226fa-p103">application/json. Required.</span></span>|
| <span data-ttu-id="226fa-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="226fa-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="226fa-129">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="226fa-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="226fa-130">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="226fa-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="226fa-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="226fa-131">Request body</span></span>

<span data-ttu-id="226fa-132">Предокажи новый [объект timeCard](../resources/timecard.md) в теле запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="226fa-132">Provide the new [timeCard](../resources/timecard.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="226fa-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="226fa-133">Response</span></span>

<span data-ttu-id="226fa-134">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект timeCard](../resources/timeCard.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="226fa-134">If successful, this method returns a `201 Created` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="226fa-135">Пример</span><span class="sxs-lookup"><span data-stu-id="226fa-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="226fa-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="226fa-136">Request</span></span>
<span data-ttu-id="226fa-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="226fa-137">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="226fa-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="226fa-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-post"
}-->

```http
POST https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards
Content-type: application/json

{
  "onBehalfOfUserId":"a3601044-a1b5-438e-b742-f78d01d68a67",
  "clockInEvent":{
     "dateTime":"2019-03-18T00:00:00.000Z",
     "atApprovedLocation":true,
     "notes": {
        "content": "Started late due to traffic in CA 237",
        "contentType": "text"
     },
  },
  "notes":{
        "content": "8 To 5 Inventory management",
        "contentType": "text"
   },
  "breaks":[
     {
       "breakId": "string",
        "notes":{
             "content": "Lunch break",
             "contentType": "text"
        },
        "start":{
           "dateTime":"2019-03-18T02:00:00.000Z",
           "atApprovedLocation":true,
           "notes": {
                "content": "Reduced break to make up for lost time",
                "contentType": "text"
             },
        }
     }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="226fa-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="226fa-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="226fa-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="226fa-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="226fa-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="226fa-141">Response</span></span>

<span data-ttu-id="226fa-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="226fa-142">The following is an example of the response.</span></span> 

><span data-ttu-id="226fa-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="226fa-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "id":"3895809b-a618-4c0d-86a0-d42b25b7d74f",
   "userId":"a3601044-a1b5-438e-b742-f78d01d68a67",
   "createdDateTime":"2019-03-18T00:00:00.000Z",
   "createdBy":{
      "user":{
         "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
         "displayName":"Dwight Schrute"
      }
   },
   "lastModifiedDateTime":"2019-03-18T00:00:00.000Z",
   "lastModifiedBy":{
      "user":{
         "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
         "displayName":"Dwight Schrute"
      }
   },
   "state":"onBreak",
   "confirmationStatus":"notConfirmed",
   "originalEntry":{
      "clockInEvent":{
         "dateTime":"2019-03-18T00:00:00.000Z",
         "atApprovedLocation":true,
         "notes": {
            "content": "Started late due to traffic in CA 237",
           "contentType": "text"
         },
      },
      "clockOutEvent":null,
      "breaks":[
         {
            "breakId":"string",
            "notes":{
                "content": "Lunch break",
                "contentType": "text"
             },
            "start":{
               "dateTime":"2019-03-18T02:00:00.000Z",
               "atApprovedLocation":true,
               "notes": {
                  "content": "Reduced break to make up for lost time",
                  "contentType": "text"
               },
            },
            "end":null
         }
      ]
   },
   "clockInEvent":{
      "dateTime":"2019-03-18T00:00:00.000Z",
      "atApprovedLocation":true,
      "notes": {
        "content": "Started late due to traffic in CA 237",
        "contentType": "text"
     },
   },
   "clockOutEvent":null,
   "notes":{
        "content": "8 To 5 Inventory management",
        "contentType": "text"
   },
   "breaks":[
      {
         "breakId":"string",
         "notes":{
             "content": "Lunch break",
             "contentType": "text"
         },
         "start":{
            "dateTime":"2019-03-18T02:00:00.000Z",
            "atApprovedLocation":true,
            "notes": {
                "content": "Reduced break to make up for lost time",
                "contentType": "text"
             },
         },
         "end":null
      }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
