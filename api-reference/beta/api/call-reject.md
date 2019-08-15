---
title: 'вызов: отклонено'
description: Отклонение входящего вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 61a7b417d2688539d705e1718813ea54c538bddf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418882"
---
# <a name="call-reject"></a><span data-ttu-id="56fb9-103">вызов: отклонено</span><span class="sxs-lookup"><span data-stu-id="56fb9-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56fb9-104">Отклонение входящего вызова.</span><span class="sxs-lookup"><span data-stu-id="56fb9-104">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="56fb9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56fb9-105">Permissions</span></span>
<span data-ttu-id="56fb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56fb9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56fb9-108">Permission type</span></span> | <span data-ttu-id="56fb9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56fb9-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="56fb9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56fb9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="56fb9-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="56fb9-111">Not Supported</span></span>                       |
| <span data-ttu-id="56fb9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56fb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56fb9-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="56fb9-113">Not Supported</span></span>                       |
| <span data-ttu-id="56fb9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56fb9-114">Application</span></span>     | <span data-ttu-id="56fb9-115">Нет</span><span class="sxs-lookup"><span data-stu-id="56fb9-115">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="56fb9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56fb9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="56fb9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56fb9-117">Request headers</span></span>
| <span data-ttu-id="56fb9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="56fb9-118">Name</span></span>          | <span data-ttu-id="56fb9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="56fb9-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="56fb9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56fb9-120">Authorization</span></span> | <span data-ttu-id="56fb9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56fb9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56fb9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56fb9-123">Request body</span></span>
<span data-ttu-id="56fb9-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="56fb9-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56fb9-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="56fb9-125">Parameter</span></span>      | <span data-ttu-id="56fb9-126">Тип</span><span class="sxs-lookup"><span data-stu-id="56fb9-126">Type</span></span>    |<span data-ttu-id="56fb9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="56fb9-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56fb9-128">причиной</span><span class="sxs-lookup"><span data-stu-id="56fb9-128">reason</span></span>|<span data-ttu-id="56fb9-129">String</span><span class="sxs-lookup"><span data-stu-id="56fb9-129">String</span></span>|<span data-ttu-id="56fb9-130">Причина отклонения.</span><span class="sxs-lookup"><span data-stu-id="56fb9-130">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="56fb9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="56fb9-131">Response</span></span>
<span data-ttu-id="56fb9-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="56fb9-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="56fb9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="56fb9-134">Example</span></span>
<span data-ttu-id="56fb9-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="56fb9-135">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="56fb9-136">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="56fb9-136">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="56fb9-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="56fb9-137">Request</span></span>
<span data-ttu-id="56fb9-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56fb9-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="56fb9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="56fb9-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="56fb9-140">C#</span><span class="sxs-lookup"><span data-stu-id="56fb9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56fb9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56fb9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56fb9-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="56fb9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="56fb9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="56fb9-143">Response</span></span>
<span data-ttu-id="56fb9-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56fb9-144">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="56fb9-145">Уведомление удалено</span><span class="sxs-lookup"><span data-stu-id="56fb9-145">Notification - deleted</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\""
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
