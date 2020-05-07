---
title: Обновление Шифтпреференцес
description: Обновление настроек смены пользователя.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 51ebeecb555c426c124975682fb85f77988d6e99
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154709"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="a9abb-103">Обновление Шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="a9abb-103">Update shiftPreferences</span></span>

<span data-ttu-id="a9abb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9abb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9abb-105">Обновление свойств и связей объекта [шифтпреференцес](../resources/shiftpreferences.md) .</span><span class="sxs-lookup"><span data-stu-id="a9abb-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9abb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9abb-106">Permissions</span></span>

<span data-ttu-id="a9abb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9abb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9abb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9abb-109">Permission type</span></span>      | <span data-ttu-id="a9abb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9abb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9abb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9abb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9abb-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9abb-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9abb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9abb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9abb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9abb-114">Not supported.</span></span>    |
|<span data-ttu-id="a9abb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9abb-115">Application</span></span> | <span data-ttu-id="a9abb-116">Усершифтпреференцес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a9abb-116">UserShiftPreferences.ReadWrite.All</span></span> |

> <span data-ttu-id="a9abb-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="a9abb-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a9abb-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="a9abb-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a9abb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9abb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="a9abb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9abb-120">Request headers</span></span>

| <span data-ttu-id="a9abb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9abb-121">Header</span></span>       | <span data-ttu-id="a9abb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9abb-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9abb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9abb-123">Authorization</span></span>  | <span data-ttu-id="a9abb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9abb-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a9abb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a9abb-126">Content-Type</span></span>  | <span data-ttu-id="a9abb-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9abb-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9abb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9abb-129">Request body</span></span>
<span data-ttu-id="a9abb-130">В тексте запроса добавьте представление объекта [шифтпреференцес](../resources/shiftpreferences.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9abb-130">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a9abb-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9abb-131">Response</span></span>

<span data-ttu-id="a9abb-132">В случае успешного выполнения этот метод возвращает код отклика `204 NO CONTENT`.</span><span class="sxs-lookup"><span data-stu-id="a9abb-132">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9abb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a9abb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9abb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9abb-134">Request</span></span>

<span data-ttu-id="a9abb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9abb-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
PUT https://graph.microsoft.com/v1.0/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
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
---


### <a name="response"></a><span data-ttu-id="a9abb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9abb-136">Response</span></span>

<span data-ttu-id="a9abb-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a9abb-137">The following is an example of the response.</span></span>

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
