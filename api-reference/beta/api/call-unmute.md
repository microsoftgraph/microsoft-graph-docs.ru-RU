---
title: 'вызов: включение звука'
description: Разрешить приложению включить Автоотключение.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7db831333982126b0edd24a5664388a89e8bc74d
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005932"
---
# <a name="call-unmute"></a><span data-ttu-id="25f89-103">вызов: включение звука</span><span class="sxs-lookup"><span data-stu-id="25f89-103">call: unmute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25f89-104">Разрешить приложению включить Автоотключение.</span><span class="sxs-lookup"><span data-stu-id="25f89-104">Allow the application to unmute itself.</span></span>

<span data-ttu-id="25f89-105">Это нерекомендуемый сервер, что означает, что сервер еще раз начнет отправлять звуковые пакеты для этого участника другим участникам.</span><span class="sxs-lookup"><span data-stu-id="25f89-105">This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.</span></span>

<span data-ttu-id="25f89-106">Дополнительные сведения об обработке операций можно найти в разделе [коммсоператион](../resources/commsOperation.md).</span><span class="sxs-lookup"><span data-stu-id="25f89-106">For more information about how to handle operations, see [commsOperation](../resources/commsOperation.md).</span></span>

> <span data-ttu-id="25f89-107">**Примечание:** Эта поддержка поддерживается только для звонков групп.</span><span class="sxs-lookup"><span data-stu-id="25f89-107">**Note:** This is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="25f89-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25f89-108">Permissions</span></span>

| <span data-ttu-id="25f89-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25f89-109">Permission type</span></span>                        | <span data-ttu-id="25f89-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25f89-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="25f89-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25f89-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="25f89-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25f89-112">Not supported.</span></span>                               |
| <span data-ttu-id="25f89-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25f89-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25f89-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25f89-114">Not supported.</span></span>                               |
| <span data-ttu-id="25f89-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25f89-115">Application</span></span>                            | <span data-ttu-id="25f89-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="25f89-116">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="25f89-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25f89-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /communications/calls/{id}/unmute
```
> <span data-ttu-id="25f89-118">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="25f89-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="25f89-119">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="25f89-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25f89-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25f89-120">Request headers</span></span>
| <span data-ttu-id="25f89-121">Имя</span><span class="sxs-lookup"><span data-stu-id="25f89-121">Name</span></span>          | <span data-ttu-id="25f89-122">Описание</span><span class="sxs-lookup"><span data-stu-id="25f89-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="25f89-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25f89-123">Authorization</span></span> | <span data-ttu-id="25f89-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25f89-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="25f89-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25f89-126">Content-type</span></span> | <span data-ttu-id="25f89-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25f89-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25f89-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25f89-129">Request body</span></span>
<span data-ttu-id="25f89-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="25f89-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="25f89-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="25f89-131">Parameter</span></span>      | <span data-ttu-id="25f89-132">Тип</span><span class="sxs-lookup"><span data-stu-id="25f89-132">Type</span></span>    |<span data-ttu-id="25f89-133">Описание</span><span class="sxs-lookup"><span data-stu-id="25f89-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25f89-134">Контекст</span><span class="sxs-lookup"><span data-stu-id="25f89-134">clientContext</span></span>|<span data-ttu-id="25f89-135">String</span><span class="sxs-lookup"><span data-stu-id="25f89-135">String</span></span>|<span data-ttu-id="25f89-136">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="25f89-136">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="25f89-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="25f89-137">Response</span></span>
<span data-ttu-id="25f89-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25f89-138">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

><span data-ttu-id="25f89-139">**Примечание:** Когда этот API возвращает успешный ответ, все участники получат обновление списка.</span><span class="sxs-lookup"><span data-stu-id="25f89-139">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="25f89-140">Пример</span><span class="sxs-lookup"><span data-stu-id="25f89-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25f89-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="25f89-141">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="25f89-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="25f89-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="25f89-143">C#</span><span class="sxs-lookup"><span data-stu-id="25f89-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25f89-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25f89-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="25f89-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25f89-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25f89-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="25f89-146">Response</span></span>

> <span data-ttu-id="25f89-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25f89-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---roster-updated-with-participant-unmuted"></a><span data-ttu-id="25f89-149">Список уведомлений обновлен с невключенным участником</span><span class="sxs-lookup"><span data-stu-id="25f89-149">Notification - roster updated with participant unmuted</span></span>

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
          "isMuted": false, // will be set to false on unmute
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
  "description": "call: unmute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
