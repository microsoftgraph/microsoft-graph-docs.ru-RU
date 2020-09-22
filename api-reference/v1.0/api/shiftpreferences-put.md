---
title: Обновление Шифтпреференцес
description: Обновление настроек смены пользователя.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0b554db9b320e4eb403aa51f67f31006f9a3b0cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984581"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="88309-103">Обновление Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="88309-103">Update shiftPreferences</span></span>

<span data-ttu-id="88309-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88309-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88309-105">Обновление свойств и связей объекта [шифтпреференцес](../resources/shiftpreferences.md) .</span><span class="sxs-lookup"><span data-stu-id="88309-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="88309-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88309-106">Permissions</span></span>

<span data-ttu-id="88309-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88309-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88309-109">Permission type</span></span>      | <span data-ttu-id="88309-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88309-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88309-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88309-111">Delegated (work or school account)</span></span> | <span data-ttu-id="88309-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88309-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="88309-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88309-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88309-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88309-114">Not supported.</span></span>    |
|<span data-ttu-id="88309-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88309-115">Application</span></span> | <span data-ttu-id="88309-116">Усершифтпреференцес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="88309-116">UserShiftPreferences.ReadWrite.All</span></span> |

> <span data-ttu-id="88309-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="88309-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="88309-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="88309-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="88309-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88309-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="88309-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88309-120">Request headers</span></span>

| <span data-ttu-id="88309-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88309-121">Header</span></span>       | <span data-ttu-id="88309-122">Значение</span><span class="sxs-lookup"><span data-stu-id="88309-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88309-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88309-123">Authorization</span></span>  | <span data-ttu-id="88309-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88309-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="88309-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88309-126">Content-Type</span></span>  | <span data-ttu-id="88309-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88309-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88309-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88309-129">Request body</span></span>
<span data-ttu-id="88309-130">В тексте запроса добавьте представление объекта [шифтпреференцес](../resources/shiftpreferences.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88309-130">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="88309-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="88309-131">Response</span></span>

<span data-ttu-id="88309-132">В случае успешного выполнения этот метод возвращает код отклика `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="88309-132">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88309-133">Пример</span><span class="sxs-lookup"><span data-stu-id="88309-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="88309-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="88309-134">Request</span></span>

<span data-ttu-id="88309-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88309-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="88309-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="88309-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
Content-type: application/json

{
    "id": "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
    "@odata.etag": "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
    "availability": [
        {
            "recurrence": {
                "pattern": {
                    "type": "Weekly",
                    "daysOfWeek": ["Monday", "Wednesday", "Friday"],
                    "interval": 1
                },
                "range": {
                    "type": "noEnd"
                }
            },
            "timeZone": "Pacific Standard Time",
            "timeSlots": null
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="88309-137">C#</span><span class="sxs-lookup"><span data-stu-id="88309-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88309-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88309-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88309-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88309-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88309-140">Java</span><span class="sxs-lookup"><span data-stu-id="88309-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="88309-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="88309-141">Response</span></span>

<span data-ttu-id="88309-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="88309-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-12-12 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update a user's shift preferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

