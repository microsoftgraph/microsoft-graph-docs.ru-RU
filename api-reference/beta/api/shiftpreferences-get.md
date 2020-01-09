---
title: Получение Шифтпреференцес
description: Получение предпочтения смены по ИДЕНТИФИКАТОРу.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ad82aeba9384b98c3bfc798f032ef54c79f05238
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994810"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="a5fd7-103">Получение Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="a5fd7-103">Get shiftPreferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5fd7-104">Получение свойств и связей объекта [шифтпреференцес](../resources/shiftpreferences.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="a5fd7-104">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5fd7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5fd7-105">Permissions</span></span>

<span data-ttu-id="a5fd7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5fd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5fd7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5fd7-108">Permission type</span></span>      | <span data-ttu-id="a5fd7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5fd7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5fd7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5fd7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5fd7-111">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5fd7-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5fd7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5fd7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5fd7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5fd7-113">Not supported.</span></span>    |
|<span data-ttu-id="a5fd7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5fd7-114">Application</span></span> | <span data-ttu-id="a5fd7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5fd7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5fd7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5fd7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="a5fd7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5fd7-117">Request headers</span></span>

| <span data-ttu-id="a5fd7-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5fd7-118">Header</span></span>       | <span data-ttu-id="a5fd7-119">Значение</span><span class="sxs-lookup"><span data-stu-id="a5fd7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5fd7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5fd7-120">Authorization</span></span>  | <span data-ttu-id="a5fd7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5fd7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5fd7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5fd7-123">Request body</span></span>
<span data-ttu-id="a5fd7-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5fd7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5fd7-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5fd7-125">Response</span></span>

<span data-ttu-id="a5fd7-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [шифтпреференцес](../resources/shiftpreferences.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a5fd7-126">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5fd7-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a5fd7-127">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a5fd7-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5fd7-128">Request</span></span>

<span data-ttu-id="a5fd7-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5fd7-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a5fd7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5fd7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/shiftPreferences
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a5fd7-131">C#</span><span class="sxs-lookup"><span data-stu-id="a5fd7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5fd7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5fd7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a5fd7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5fd7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a5fd7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5fd7-134">Response</span></span>

<span data-ttu-id="a5fd7-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5fd7-135">The following is an example of the response.</span></span>

><span data-ttu-id="a5fd7-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5fd7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
