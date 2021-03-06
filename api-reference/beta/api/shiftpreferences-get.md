---
title: Получить shiftPreferences
description: Получите параметр shift preference by ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 247e4626c35eb9b0d9d3cf82d5ebc32621922755
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516803"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="1160b-103">Получить shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="1160b-103">Get shiftPreferences</span></span>

<span data-ttu-id="1160b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1160b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1160b-105">Извлечение свойств и связей [объекта shiftPreferences](../resources/shiftpreferences.md) по ID.</span><span class="sxs-lookup"><span data-stu-id="1160b-105">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="1160b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1160b-106">Permissions</span></span>

<span data-ttu-id="1160b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1160b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1160b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1160b-109">Permission type</span></span>      | <span data-ttu-id="1160b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1160b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1160b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1160b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1160b-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1160b-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="1160b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1160b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1160b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1160b-114">Not supported.</span></span>    |
|<span data-ttu-id="1160b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1160b-115">Application</span></span> | <span data-ttu-id="1160b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1160b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1160b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1160b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1160b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1160b-118">Optional query parameters</span></span>

<span data-ttu-id="1160b-119">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1160b-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1160b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1160b-120">Request headers</span></span>

| <span data-ttu-id="1160b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1160b-121">Header</span></span>       | <span data-ttu-id="1160b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1160b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1160b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1160b-123">Authorization</span></span>  | <span data-ttu-id="1160b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1160b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1160b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1160b-126">Request body</span></span>
<span data-ttu-id="1160b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1160b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1160b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1160b-128">Response</span></span>

<span data-ttu-id="1160b-129">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [shiftPreferences](../resources/shiftpreferences.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1160b-129">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1160b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1160b-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1160b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1160b-131">Request</span></span>

<span data-ttu-id="1160b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1160b-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1160b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1160b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
```
# <a name="c"></a>[<span data-ttu-id="1160b-134">C#</span><span class="sxs-lookup"><span data-stu-id="1160b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1160b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1160b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1160b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1160b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1160b-137">Java</span><span class="sxs-lookup"><span data-stu-id="1160b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1160b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1160b-138">Response</span></span>

<span data-ttu-id="1160b-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1160b-139">The following is an example of the response.</span></span>

><span data-ttu-id="1160b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1160b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shiftPreferences"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "id": "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
    "@odata.etag": "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
    "availability": [
        {
            "recurrence": {
                "pattern": {
                    "type": "Weekly",
                    "daysOfWeek": ["Tuesday"],
                    "interval": 1
                },
                "range": {
                    "type": "noEnd"
                }
            },
            "timeZone": "Pacific Standard Time",
            "timeSlots": [
                {
                    "startTime": "09:15:00.000000",
                    "endTime": "12:30:00.000000"
                },
                {
                    "startTime": "16:00:00.000000",
                    "endTime": "20:00:00.000000"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-12-12 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a user's shift preferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


