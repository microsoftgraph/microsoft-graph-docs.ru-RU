---
title: Обновление Шифтпреференцес
description: Обновление настроек смены пользователя.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 83bec268e918bc65f1ce139081ff88c0290acf4d
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952085"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="90c39-103">Обновление Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="90c39-103">Update shiftPreferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90c39-104">Обновление свойств и связей объекта [шифтпреференцес](../resources/shiftpreferences.md) .</span><span class="sxs-lookup"><span data-stu-id="90c39-104">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90c39-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90c39-105">Permissions</span></span>

<span data-ttu-id="90c39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90c39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90c39-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90c39-108">Permission type</span></span>      | <span data-ttu-id="90c39-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90c39-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90c39-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90c39-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90c39-111">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90c39-111">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="90c39-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90c39-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90c39-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90c39-113">Not supported.</span></span>    |
|<span data-ttu-id="90c39-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90c39-114">Application</span></span> | <span data-ttu-id="90c39-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90c39-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90c39-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90c39-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="90c39-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90c39-117">Request headers</span></span>

| <span data-ttu-id="90c39-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90c39-118">Header</span></span>       | <span data-ttu-id="90c39-119">Значение</span><span class="sxs-lookup"><span data-stu-id="90c39-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90c39-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90c39-120">Authorization</span></span>  | <span data-ttu-id="90c39-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90c39-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="90c39-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="90c39-123">Content-Type</span></span>  | <span data-ttu-id="90c39-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90c39-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90c39-126">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="90c39-126">Request body</span></span>
<span data-ttu-id="90c39-127">Укажите новый объект [шифтпреференцес](../resources/shiftpreferences.md) в тексте запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90c39-127">Provide the new [shiftPreferences](../resources/shiftpreferences.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90c39-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="90c39-128">Response</span></span>

<span data-ttu-id="90c39-129">В случае успешного выполнения этот метод возвращает код отклика `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="90c39-129">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="90c39-130">Пример</span><span class="sxs-lookup"><span data-stu-id="90c39-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="90c39-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="90c39-131">Request</span></span>

<span data-ttu-id="90c39-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90c39-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90c39-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="90c39-133">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="90c39-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c39-134">Response</span></span>

<span data-ttu-id="90c39-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="90c39-135">The following is an example of the response.</span></span>

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
