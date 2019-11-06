---
title: 'участник: выкл.'
description: Отключение выключения определенного участника в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: cbf65ee703e22895e25ae18b2a94c4a1740527f2
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006503"
---
# <a name="participant-mute"></a><span data-ttu-id="d81cb-103">участник: выкл.</span><span class="sxs-lookup"><span data-stu-id="d81cb-103">participant: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d81cb-104">Отключение выключения определенного участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="d81cb-104">Mute a specific participant in the call.</span></span>

<span data-ttu-id="d81cb-105">Это Выключенный сервер, что означает, что сервер будет отбрасывать все звуковые пакеты для этого участника, даже если участник продолжает потоковую передачу звука.</span><span class="sxs-lookup"><span data-stu-id="d81cb-105">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="d81cb-106">Дополнительные сведения об обработке операций можно найти в разделе [коммсоператион](../resources/commsOperation.md).</span><span class="sxs-lookup"><span data-stu-id="d81cb-106">For more information about how to handle operations, see [commsOperation](../resources/commsOperation.md).</span></span>

> <span data-ttu-id="d81cb-107">**Примечание:** Эта поддержка поддерживается только для звонков групп.</span><span class="sxs-lookup"><span data-stu-id="d81cb-107">**Note:** This is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="d81cb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d81cb-108">Permissions</span></span>

| <span data-ttu-id="d81cb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d81cb-109">Permission type</span></span> | <span data-ttu-id="d81cb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d81cb-110">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="d81cb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d81cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d81cb-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d81cb-112">Not Supported</span></span>        |
| <span data-ttu-id="d81cb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d81cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d81cb-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d81cb-114">Not Supported</span></span>        |
| <span data-ttu-id="d81cb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d81cb-115">Application</span></span>     | <span data-ttu-id="d81cb-116">Нет</span><span class="sxs-lookup"><span data-stu-id="d81cb-116">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="d81cb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d81cb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /communications/calls/{id}/participants/{id}/mute
```
> <span data-ttu-id="d81cb-118">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="d81cb-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="d81cb-119">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="d81cb-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d81cb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d81cb-120">Request headers</span></span>
| <span data-ttu-id="d81cb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d81cb-121">Name</span></span>          | <span data-ttu-id="d81cb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d81cb-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d81cb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d81cb-123">Authorization</span></span> | <span data-ttu-id="d81cb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d81cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d81cb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d81cb-126">Content-type</span></span>  | <span data-ttu-id="d81cb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d81cb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d81cb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d81cb-129">Request body</span></span>
<span data-ttu-id="d81cb-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d81cb-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d81cb-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="d81cb-131">Parameter</span></span>      | <span data-ttu-id="d81cb-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d81cb-132">Type</span></span>    |<span data-ttu-id="d81cb-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d81cb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d81cb-134">Контекст</span><span class="sxs-lookup"><span data-stu-id="d81cb-134">clientContext</span></span>|<span data-ttu-id="d81cb-135">String</span><span class="sxs-lookup"><span data-stu-id="d81cb-135">String</span></span>|<span data-ttu-id="d81cb-136">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="d81cb-136">Unique Client Context string.</span></span> <span data-ttu-id="d81cb-137">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="d81cb-137">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="d81cb-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="d81cb-138">Response</span></span>
<span data-ttu-id="d81cb-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d81cb-139">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

><span data-ttu-id="d81cb-140">**Примечание:** Вхем этот API возвращает успешный ответ, все участники получат обновление списка.</span><span class="sxs-lookup"><span data-stu-id="d81cb-140">**Note:** Whem this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example---mute-specific-participant"></a><span data-ttu-id="d81cb-141">Пример: Специальный участник</span><span class="sxs-lookup"><span data-stu-id="d81cb-141">Example - Mute specific participant</span></span>
<span data-ttu-id="d81cb-142">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d81cb-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d81cb-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d81cb-143">Request</span></span>
<span data-ttu-id="d81cb-144">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d81cb-144">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d81cb-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d81cb-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants/2765eb15-01f8-47c6-b12b-c32111a4a86f/mute
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d81cb-146">C#</span><span class="sxs-lookup"><span data-stu-id="d81cb-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d81cb-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d81cb-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d81cb-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d81cb-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d81cb-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d81cb-149">Response</span></span>

> <span data-ttu-id="d81cb-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d81cb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 


<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.muteParticipantOperation",
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="d81cb-152">Список уведомлений обновлен с отключенным участником</span><span class="sxs-lookup"><span data-stu-id="d81cb-152">Notification - roster updated with participant muted</span></span>

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
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
