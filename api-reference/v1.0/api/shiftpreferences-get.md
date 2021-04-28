---
title: Получить shiftPreferences
description: Получите параметр shift preference by ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a4ee1518048931d605acfb4dd96908285fc44b9b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034856"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="621d9-103">Получить shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="621d9-103">Get shiftPreferences</span></span>

<span data-ttu-id="621d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="621d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="621d9-105">Извлечение свойств и связей [объекта shiftPreferences](../resources/shiftpreferences.md) по ID.</span><span class="sxs-lookup"><span data-stu-id="621d9-105">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="621d9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="621d9-106">Permissions</span></span>

<span data-ttu-id="621d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="621d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="621d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="621d9-109">Permission type</span></span>      | <span data-ttu-id="621d9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="621d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="621d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="621d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="621d9-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="621d9-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="621d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="621d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="621d9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="621d9-114">Not supported.</span></span>    |
|<span data-ttu-id="621d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="621d9-115">Application</span></span> | <span data-ttu-id="621d9-116">UserShiftPreferences.Read.All, UserShiftPreferences.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="621d9-116">UserShiftPreferences.Read.All, UserShiftPreferences.ReadWrite.All</span></span> |

> <span data-ttu-id="621d9-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="621d9-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="621d9-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="621d9-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="621d9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="621d9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="optional-query-parameters"></a><span data-ttu-id="621d9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="621d9-120">Optional query parameters</span></span>

<span data-ttu-id="621d9-121">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="621d9-121">This method does not support OData query parameters to customize the response.</span></span>


## <a name="request-headers"></a><span data-ttu-id="621d9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="621d9-122">Request headers</span></span>

| <span data-ttu-id="621d9-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="621d9-123">Header</span></span>       | <span data-ttu-id="621d9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="621d9-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="621d9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="621d9-125">Authorization</span></span>  | <span data-ttu-id="621d9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="621d9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="621d9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="621d9-128">Request body</span></span>
<span data-ttu-id="621d9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="621d9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="621d9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="621d9-130">Response</span></span>

<span data-ttu-id="621d9-131">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [shiftPreferences](../resources/shiftpreferences.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="621d9-131">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="621d9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="621d9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="621d9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="621d9-133">Request</span></span>

<span data-ttu-id="621d9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="621d9-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="621d9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="621d9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shiftpreferences"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
```
# <a name="c"></a>[<span data-ttu-id="621d9-136">C#</span><span class="sxs-lookup"><span data-stu-id="621d9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shiftpreferences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="621d9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="621d9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shiftpreferences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="621d9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="621d9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shiftpreferences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="621d9-139">Java</span><span class="sxs-lookup"><span data-stu-id="621d9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shiftpreferences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="621d9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="621d9-140">Response</span></span>

<span data-ttu-id="621d9-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="621d9-141">The following is an example of the response.</span></span>

><span data-ttu-id="621d9-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="621d9-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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

