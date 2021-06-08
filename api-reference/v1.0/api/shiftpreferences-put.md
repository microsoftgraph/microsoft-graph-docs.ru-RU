---
title: Обновление shiftPreferences
description: Обновление личных предпочтений пользователя.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fc88bccb2360d2b0de5e7336a507f760485a4b42
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787746"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="3e7dc-103">Обновление shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="3e7dc-103">Update shiftPreferences</span></span>

<span data-ttu-id="3e7dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e7dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e7dc-105">Обновление свойств и связей объекта [shiftPreferences.](../resources/shiftpreferences.md)</span><span class="sxs-lookup"><span data-stu-id="3e7dc-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e7dc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7dc-106">Permissions</span></span>

<span data-ttu-id="3e7dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e7dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e7dc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7dc-109">Permission type</span></span>      | <span data-ttu-id="3e7dc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e7dc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e7dc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e7dc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e7dc-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e7dc-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e7dc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e7dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e7dc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-114">Not supported.</span></span>    |
|<span data-ttu-id="3e7dc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e7dc-115">Application</span></span> | <span data-ttu-id="3e7dc-116">UserShiftPreferences.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e7dc-116">UserShiftPreferences.ReadWrite.All</span></span> |

> <span data-ttu-id="3e7dc-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3e7dc-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3e7dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e7dc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="3e7dc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e7dc-120">Request headers</span></span>

| <span data-ttu-id="3e7dc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e7dc-121">Header</span></span>       | <span data-ttu-id="3e7dc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e7dc-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e7dc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e7dc-123">Authorization</span></span>  | <span data-ttu-id="3e7dc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3e7dc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e7dc-126">Content-Type</span></span>  | <span data-ttu-id="3e7dc-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e7dc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e7dc-129">Request body</span></span>
<span data-ttu-id="3e7dc-130">В теле запроса поставляем представление JSON объекта [shiftPreferences.](../resources/shiftpreferences.md)</span><span class="sxs-lookup"><span data-stu-id="3e7dc-130">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3e7dc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e7dc-131">Response</span></span>

<span data-ttu-id="3e7dc-132">В случае успешного выполнения этот метод возвращает код отклика `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-132">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3e7dc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3e7dc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e7dc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e7dc-134">Request</span></span>

<span data-ttu-id="3e7dc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3e7dc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e7dc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get-2"
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
# <a name="c"></a>[<span data-ttu-id="3e7dc-137">C#</span><span class="sxs-lookup"><span data-stu-id="3e7dc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e7dc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e7dc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e7dc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e7dc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e7dc-140">Java</span><span class="sxs-lookup"><span data-stu-id="3e7dc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="3e7dc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e7dc-141">Response</span></span>

<span data-ttu-id="3e7dc-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
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

