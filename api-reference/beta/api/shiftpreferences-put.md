---
title: Обновление Шифтпреференцес
description: Обновление настроек смены пользователя.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b3f87e6981abf18a4f082839c3e3e47455d36961
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44154327"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="08b03-103">Обновление Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="08b03-103">Update shiftPreferences</span></span>

<span data-ttu-id="08b03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08b03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08b03-105">Обновление свойств и связей объекта [шифтпреференцес](../resources/shiftpreferences.md) .</span><span class="sxs-lookup"><span data-stu-id="08b03-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="08b03-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08b03-106">Permissions</span></span>

<span data-ttu-id="08b03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08b03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08b03-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08b03-109">Permission type</span></span>      | <span data-ttu-id="08b03-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08b03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08b03-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08b03-111">Delegated (work or school account)</span></span> | <span data-ttu-id="08b03-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08b03-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="08b03-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08b03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08b03-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08b03-114">Not supported.</span></span>    |
|<span data-ttu-id="08b03-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08b03-115">Application</span></span> | <span data-ttu-id="08b03-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08b03-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08b03-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08b03-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="08b03-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08b03-118">Request headers</span></span>

| <span data-ttu-id="08b03-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08b03-119">Header</span></span>       | <span data-ttu-id="08b03-120">Значение</span><span class="sxs-lookup"><span data-stu-id="08b03-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08b03-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08b03-121">Authorization</span></span>  | <span data-ttu-id="08b03-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08b03-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="08b03-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08b03-124">Content-Type</span></span>  | <span data-ttu-id="08b03-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08b03-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08b03-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08b03-127">Request body</span></span>
<span data-ttu-id="08b03-128">В тексте запроса добавьте представление объекта [шифтпреференцес](../resources/shiftpreferences.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08b03-128">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="08b03-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="08b03-129">Response</span></span>

<span data-ttu-id="08b03-130">В случае успешного выполнения этот метод возвращает код отклика `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="08b03-130">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="08b03-131">Пример</span><span class="sxs-lookup"><span data-stu-id="08b03-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="08b03-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="08b03-132">Request</span></span>

<span data-ttu-id="08b03-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08b03-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08b03-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="08b03-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
PUT https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
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
# <a name="c"></a>[<span data-ttu-id="08b03-135">C#</span><span class="sxs-lookup"><span data-stu-id="08b03-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08b03-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08b03-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08b03-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08b03-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="08b03-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="08b03-138">Response</span></span>

<span data-ttu-id="08b03-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="08b03-139">The following is an example of the response.</span></span>

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
