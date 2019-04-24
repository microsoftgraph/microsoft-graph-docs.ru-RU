---
title: 'вызов: отклонено'
description: Отклонение входящего вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5b42ebee208431cd0a02be291d07f580d98c87a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461321"
---
# <a name="call-reject"></a><span data-ttu-id="5e9d4-103">вызов: отклонено</span><span class="sxs-lookup"><span data-stu-id="5e9d4-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e9d4-104">Отклонение входящего вызова.</span><span class="sxs-lookup"><span data-stu-id="5e9d4-104">Reject an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e9d4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e9d4-105">Permissions</span></span>
<span data-ttu-id="5e9d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e9d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e9d4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e9d4-108">Permission type</span></span> | <span data-ttu-id="5e9d4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e9d4-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="5e9d4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e9d4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e9d4-111">Неподдерживаемая функция</span><span class="sxs-lookup"><span data-stu-id="5e9d4-111">Not Supported</span></span>                       |
| <span data-ttu-id="5e9d4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e9d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e9d4-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5e9d4-113">Not Supported</span></span>                       |
| <span data-ttu-id="5e9d4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e9d4-114">Application</span></span>     | <span data-ttu-id="5e9d4-115">Нет</span><span class="sxs-lookup"><span data-stu-id="5e9d4-115">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="5e9d4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e9d4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /applications/{id}/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="5e9d4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e9d4-117">Request headers</span></span>
| <span data-ttu-id="5e9d4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5e9d4-118">Name</span></span>          | <span data-ttu-id="5e9d4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5e9d4-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5e9d4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e9d4-120">Authorization</span></span> | <span data-ttu-id="5e9d4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e9d4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e9d4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e9d4-123">Request body</span></span>
<span data-ttu-id="5e9d4-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5e9d4-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5e9d4-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="5e9d4-125">Parameter</span></span>      | <span data-ttu-id="5e9d4-126">Тип</span><span class="sxs-lookup"><span data-stu-id="5e9d4-126">Type</span></span>    |<span data-ttu-id="5e9d4-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5e9d4-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e9d4-128">причиной</span><span class="sxs-lookup"><span data-stu-id="5e9d4-128">reason</span></span>|<span data-ttu-id="5e9d4-129">String</span><span class="sxs-lookup"><span data-stu-id="5e9d4-129">String</span></span>|<span data-ttu-id="5e9d4-130">Причина отклонения.</span><span class="sxs-lookup"><span data-stu-id="5e9d4-130">The rejection reason.</span></span>|

## <a name="response"></a><span data-ttu-id="5e9d4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e9d4-131">Response</span></span>
<span data-ttu-id="5e9d4-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5e9d4-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

```http
Returns `202 Accepted` response code
```

## <a name="example"></a><span data-ttu-id="5e9d4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="5e9d4-134">Example</span></span>
<span data-ttu-id="5e9d4-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="5e9d4-135">The following example shows how to call this API.</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="5e9d4-136">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="5e9d4-136">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="5e9d4-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e9d4-137">Request</span></span>
<span data-ttu-id="5e9d4-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e9d4-138">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="5e9d4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e9d4-139">Response</span></span>
<span data-ttu-id="5e9d4-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5e9d4-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="5e9d4-141">Уведомление удалено</span><span class="sxs-lookup"><span data-stu-id="5e9d4-141">Notification - deleted</span></span>

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
