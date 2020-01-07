---
title: Получение Шифтпреференцес
description: Получение предпочтения смены по ИДЕНТИФИКАТОРу.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0ef9a067cfb106c6cee5fadb113da5aabfa7f3a
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952120"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="22690-103">Получение Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="22690-103">Get shiftPreferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22690-104">Получение свойств и связей объекта [шифтпреференцес](../resources/shiftpreferences.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="22690-104">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="22690-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22690-105">Permissions</span></span>

<span data-ttu-id="22690-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22690-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22690-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22690-108">Permission type</span></span>      | <span data-ttu-id="22690-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22690-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22690-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22690-110">Delegated (work or school account)</span></span> | <span data-ttu-id="22690-111">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22690-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="22690-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22690-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22690-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22690-113">Not supported.</span></span>    |
|<span data-ttu-id="22690-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22690-114">Application</span></span> | <span data-ttu-id="22690-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22690-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22690-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22690-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="22690-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22690-117">Request headers</span></span>

| <span data-ttu-id="22690-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22690-118">Header</span></span>       | <span data-ttu-id="22690-119">Значение</span><span class="sxs-lookup"><span data-stu-id="22690-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="22690-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22690-120">Authorization</span></span>  | <span data-ttu-id="22690-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22690-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="22690-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22690-123">Request body</span></span>
<span data-ttu-id="22690-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22690-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22690-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="22690-125">Response</span></span>

<span data-ttu-id="22690-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [шифтпреференцес](../resources/shiftpreferences.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22690-126">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22690-127">Пример</span><span class="sxs-lookup"><span data-stu-id="22690-127">Example</span></span>

#### <a name="request"></a><span data-ttu-id="22690-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="22690-128">Request</span></span>

<span data-ttu-id="22690-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22690-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="22690-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="22690-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/shiftPreferences
```

#### <a name="response"></a><span data-ttu-id="22690-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="22690-131">Response</span></span>

<span data-ttu-id="22690-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22690-132">The following is an example of the response.</span></span>

><span data-ttu-id="22690-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22690-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
