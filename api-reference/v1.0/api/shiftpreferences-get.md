---
title: Получение Шифтпреференцес
description: Получение предпочтения смены по ИДЕНТИФИКАТОРу.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a83331992092cec3204b0279944a13c17870c295
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217363"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="42346-103">Получение Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="42346-103">Get shiftPreferences</span></span>

<span data-ttu-id="42346-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42346-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="42346-105">Получение свойств и связей объекта [шифтпреференцес](../resources/shiftpreferences.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="42346-105">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="42346-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42346-106">Permissions</span></span>

<span data-ttu-id="42346-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42346-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42346-109">Permission type</span></span>      | <span data-ttu-id="42346-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42346-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42346-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42346-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42346-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42346-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="42346-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42346-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42346-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42346-114">Not supported.</span></span>    |
|<span data-ttu-id="42346-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42346-115">Application</span></span> | <span data-ttu-id="42346-116">Усершифтпреференцес. Read. ALL, Усершифтпреференцес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="42346-116">UserShiftPreferences.Read.All, UserShiftPreferences.ReadWrite.All</span></span> |

> <span data-ttu-id="42346-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="42346-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="42346-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="42346-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="42346-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42346-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42346-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42346-120">Optional query parameters</span></span>

<span data-ttu-id="42346-121">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="42346-121">This method does not support OData query parameters to customize the response.</span></span>


## <a name="request-headers"></a><span data-ttu-id="42346-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42346-122">Request headers</span></span>

| <span data-ttu-id="42346-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42346-123">Header</span></span>       | <span data-ttu-id="42346-124">Значение</span><span class="sxs-lookup"><span data-stu-id="42346-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42346-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42346-125">Authorization</span></span>  | <span data-ttu-id="42346-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42346-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="42346-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42346-128">Request body</span></span>
<span data-ttu-id="42346-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42346-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42346-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="42346-130">Response</span></span>

<span data-ttu-id="42346-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [шифтпреференцес](../resources/shiftpreferences.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42346-131">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42346-132">Пример</span><span class="sxs-lookup"><span data-stu-id="42346-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="42346-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="42346-133">Request</span></span>

<span data-ttu-id="42346-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42346-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="42346-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="42346-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/871dbd5c-3a6a-4392-bfe1-042452793a50/shiftPreferences
```
# <a name="c"></a>[<span data-ttu-id="42346-136">C#</span><span class="sxs-lookup"><span data-stu-id="42346-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42346-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42346-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42346-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42346-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42346-139">Java</span><span class="sxs-lookup"><span data-stu-id="42346-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="42346-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="42346-140">Response</span></span>

<span data-ttu-id="42346-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="42346-141">The following is an example of the response.</span></span>

><span data-ttu-id="42346-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42346-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
