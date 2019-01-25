---
title: 'Вызовите: отклонить'
description: Отклонение входящего звонка.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5b42ebee208431cd0a02be291d07f580d98c87a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516191"
---
# <a name="call-reject"></a><span data-ttu-id="f3a14-103">Вызовите: отклонить</span><span class="sxs-lookup"><span data-stu-id="f3a14-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3a14-104">Отклонение входящего звонка.</span><span class="sxs-lookup"><span data-stu-id="f3a14-104">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3a14-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3a14-105">Permissions</span></span>
<span data-ttu-id="f3a14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3a14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f3a14-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3a14-108">Permission type</span></span> | <span data-ttu-id="f3a14-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3a14-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="f3a14-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3a14-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3a14-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f3a14-111">Not Supported</span></span>                       |
| <span data-ttu-id="f3a14-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3a14-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3a14-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f3a14-113">Not Supported</span></span>                       |
| <span data-ttu-id="f3a14-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3a14-114">Application</span></span>     | <span data-ttu-id="f3a14-115">Нет</span><span class="sxs-lookup"><span data-stu-id="f3a14-115">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="f3a14-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3a14-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="f3a14-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3a14-117">Request headers</span></span>
| <span data-ttu-id="f3a14-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f3a14-118">Name</span></span>          | <span data-ttu-id="f3a14-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f3a14-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f3a14-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3a14-120">Authorization</span></span> | <span data-ttu-id="f3a14-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3a14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3a14-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3a14-123">Request body</span></span>
<span data-ttu-id="f3a14-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f3a14-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f3a14-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="f3a14-125">Parameter</span></span>      | <span data-ttu-id="f3a14-126">Тип</span><span class="sxs-lookup"><span data-stu-id="f3a14-126">Type</span></span>    |<span data-ttu-id="f3a14-127">Описание</span><span class="sxs-lookup"><span data-stu-id="f3a14-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3a14-128">Причина</span><span class="sxs-lookup"><span data-stu-id="f3a14-128">reason</span></span>|<span data-ttu-id="f3a14-129">String</span><span class="sxs-lookup"><span data-stu-id="f3a14-129">String</span></span>|<span data-ttu-id="f3a14-130">Причину отклонения.</span><span class="sxs-lookup"><span data-stu-id="f3a14-130">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="f3a14-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3a14-131">Response</span></span>
<span data-ttu-id="f3a14-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f3a14-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="f3a14-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f3a14-134">Example</span></span>
<span data-ttu-id="f3a14-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f3a14-135">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="f3a14-136">Уведомления - входящие</span><span class="sxs-lookup"><span data-stu-id="f3a14-136">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="f3a14-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3a14-137">Request</span></span>
<span data-ttu-id="f3a14-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3a14-138">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="f3a14-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3a14-139">Response</span></span>
<span data-ttu-id="f3a14-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f3a14-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="f3a14-141">Уведомления - удалены</span><span class="sxs-lookup"><span data-stu-id="f3a14-141">Notification - deleted</span></span>

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
    "Error: /api-reference/beta/api/call-reject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
