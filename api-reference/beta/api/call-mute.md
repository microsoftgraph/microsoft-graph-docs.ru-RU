---
title: 'вызов: выкл.'
description: Позволяет приложению отключить себя.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d1c9093f6c86f11588b0758a80fdbe8682d6d216
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005978"
---
# <a name="call-mute"></a><span data-ttu-id="0f109-103">вызов: выкл.</span><span class="sxs-lookup"><span data-stu-id="0f109-103">call: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f109-104">Позволяет приложению отключить себя.</span><span class="sxs-lookup"><span data-stu-id="0f109-104">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f109-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f109-105">Permissions</span></span>
<span data-ttu-id="0f109-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f109-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f109-108">Permission type</span></span>                        | <span data-ttu-id="0f109-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f109-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0f109-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f109-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f109-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f109-111">Not Supported.</span></span>                               |
| <span data-ttu-id="0f109-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f109-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f109-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f109-113">Not Supported.</span></span>                               |
| <span data-ttu-id="0f109-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f109-114">Application</span></span>                            | <span data-ttu-id="0f109-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="0f109-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="0f109-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f109-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /communications/calls/{id}/mute
```
> <span data-ttu-id="0f109-117">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="0f109-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="0f109-118">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="0f109-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f109-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f109-119">Request headers</span></span>
| <span data-ttu-id="0f109-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0f109-120">Name</span></span>          | <span data-ttu-id="0f109-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0f109-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0f109-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f109-122">Authorization</span></span> | <span data-ttu-id="0f109-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f109-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f109-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f109-125">Request body</span></span>
<span data-ttu-id="0f109-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0f109-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0f109-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="0f109-127">Parameter</span></span>      | <span data-ttu-id="0f109-128">Тип</span><span class="sxs-lookup"><span data-stu-id="0f109-128">Type</span></span>    |<span data-ttu-id="0f109-129">Описание</span><span class="sxs-lookup"><span data-stu-id="0f109-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f109-130">Контекст</span><span class="sxs-lookup"><span data-stu-id="0f109-130">clientContext</span></span>|<span data-ttu-id="0f109-131">String</span><span class="sxs-lookup"><span data-stu-id="0f109-131">String</span></span>|<span data-ttu-id="0f109-132">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="0f109-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="0f109-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f109-133">Response</span></span>
<span data-ttu-id="0f109-134">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f109-134">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f109-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0f109-135">Example</span></span>
<span data-ttu-id="0f109-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="0f109-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0f109-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f109-137">Request</span></span>
<span data-ttu-id="0f109-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f109-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0f109-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f109-139">HTTP</span></span>](#tab/http)
<!-- { 
  "blockType": "request", 
  "name": "call-mute" 
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/mute
Content-Type: application/json

{
  "clientContext": "clientContext-value"
}
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="0f109-140">C#</span><span class="sxs-lookup"><span data-stu-id="0f109-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f109-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f109-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f109-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f109-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0f109-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f109-143">Response</span></span>

> <span data-ttu-id="0f109-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f109-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
 
<!-- { 
  "blockType": "response", 
  "truncated": true, 
  "@odata.type": "microsoft.graph.commsOperation" 
} --> 
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#commsOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="0f109-146">Список уведомлений обновлен с отключенным участником</span><span class="sxs-lookup"><span data-stu-id="0f109-146">Notification - roster updated with participant muted</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "2765eb15-01f8-47c6-b12b-c32111a4a86f",
          "info": {
            "identity": {
              "user": {
                "displayName": "Bob",
                "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive"
            }
          ],
          "isMuted": true, // will be set to true on mute
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
