---
title: Get timeCard
description: Получите карточку timeCard по ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f1e2424a9303caa69aa2f64798f9c61388418723
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787910"
---
# <a name="get-timecard"></a><span data-ttu-id="e88fc-103">Get timeCard</span><span class="sxs-lookup"><span data-stu-id="e88fc-103">Get timeCard</span></span>

<span data-ttu-id="e88fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e88fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e88fc-105">Извлечение свойств и связей объекта [timeCard](../resources/timeCard.md) по ID.</span><span class="sxs-lookup"><span data-stu-id="e88fc-105">Retrieve the properties and relationships of a [timeCard](../resources/timeCard.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="e88fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e88fc-106">Permissions</span></span>

<span data-ttu-id="e88fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e88fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e88fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e88fc-109">Permission type</span></span>      | <span data-ttu-id="e88fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e88fc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e88fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e88fc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e88fc-112">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e88fc-112">Schedule.Read.All, Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="e88fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e88fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e88fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e88fc-114">Not supported.</span></span>    |
|<span data-ttu-id="e88fc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e88fc-115">Application</span></span> | <span data-ttu-id="e88fc-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="e88fc-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="e88fc-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="e88fc-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="e88fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e88fc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards/{timecardID}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="e88fc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e88fc-119">Optional query parameters</span></span>
<span data-ttu-id="e88fc-120">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e88fc-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e88fc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e88fc-121">Request headers</span></span>

| <span data-ttu-id="e88fc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e88fc-122">Header</span></span>       | <span data-ttu-id="e88fc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e88fc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e88fc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e88fc-124">Authorization</span></span>  | <span data-ttu-id="e88fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e88fc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e88fc-127">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="e88fc-127">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="e88fc-128">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="e88fc-128">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="e88fc-129">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="e88fc-129">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e88fc-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e88fc-130">Request body</span></span>
<span data-ttu-id="e88fc-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e88fc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e88fc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e88fc-132">Response</span></span>

<span data-ttu-id="e88fc-133">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект timeCard](../resources/timeCard.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e88fc-133">If successful, this method returns a `200 OK` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e88fc-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e88fc-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e88fc-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e88fc-135">Request</span></span>
<span data-ttu-id="e88fc-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e88fc-136">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="e88fc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e88fc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-get"
}-->

```http
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972
```

### <a name="response"></a><span data-ttu-id="e88fc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e88fc-138">Response</span></span>

<span data-ttu-id="e88fc-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e88fc-139">The following is an example of the response.</span></span> 

><span data-ttu-id="e88fc-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e88fc-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972",
    "createdDateTime": "2021-05-27T22:58:41.327Z",
    "lastModifiedDateTime": "2021-05-27T23:02:04.187Z",
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedOut",
    "confirmedBy": "user,manager",
    "notes": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    },
    "clockInEvent": {
        "dateTime": "2021-05-27T22:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock in notes"
        }
    },
    "clockOutEvent": {
        "dateTime": "2021-05-27T23:01:46.205Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock out smaple notes"
        }
    },
    "breaks": [
        {
            "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
            "notes": null,
            "start": {
                "dateTime": "2021-05-27T22:59:59.328Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "start break smaple notes"
                }
            },
            "end": {
                "dateTime": "2021-05-27T23:01:10.205Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "end break smaple notes"
                }
            }
        }
    ],
    "originalEntry": {
        "clockInEvent": {
            "dateTime": "2021-05-27T22:58:41.327Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock in notes"
            }
        },
        "clockOutEvent": {
            "dateTime": "2021-05-27T23:01:46.205Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock out smaple notes"
            }
        },
        "breaks": [
            {
                "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
                "notes": null,
                "start": {
                    "dateTime": "2021-05-27T22:59:59.328Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "start break smaple notes"
                    }
                },
                "end": {
                    "dateTime": "2021-05-27T23:01:10.205Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "end break smaple notes"
                    }
                }
            }
        ]
    },
    "createdBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeCard by ID",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
