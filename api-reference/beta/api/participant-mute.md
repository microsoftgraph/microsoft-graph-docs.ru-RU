---
title: 'участник: выкл.'
description: Отключение выключения определенного участника в вызове.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b2101b45826475013124149c90e10edb3147153f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455973"
---
# <a name="participant-mute"></a><span data-ttu-id="44c95-103">участник: выкл.</span><span class="sxs-lookup"><span data-stu-id="44c95-103">participant: mute</span></span>

<span data-ttu-id="44c95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44c95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44c95-105">Отключение выключения определенного участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="44c95-105">Mute a specific participant in the call.</span></span>

<span data-ttu-id="44c95-106">Это Выключенный сервер, что означает, что сервер будет отбрасывать все звуковые пакеты для этого участника, даже если участник продолжает потоковую передачу звука.</span><span class="sxs-lookup"><span data-stu-id="44c95-106">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="44c95-107">Дополнительные сведения о том, как обрабатывать операции отключения звука, можно найти в разделе [мутепартиЦипантоператион](../resources/muteParticipantoperation.md).</span><span class="sxs-lookup"><span data-stu-id="44c95-107">For more information about how to handle mute operations, see [muteParticipantOperation](../resources/muteParticipantoperation.md).</span></span>

> <span data-ttu-id="44c95-108">**Примечание:** Этот метод поддерживается только для вызовов групп.</span><span class="sxs-lookup"><span data-stu-id="44c95-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="44c95-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44c95-109">Permissions</span></span>

| <span data-ttu-id="44c95-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44c95-110">Permission type</span></span> | <span data-ttu-id="44c95-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44c95-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="44c95-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44c95-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="44c95-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="44c95-113">Not Supported</span></span>        |
| <span data-ttu-id="44c95-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44c95-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44c95-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="44c95-115">Not Supported</span></span>        |
| <span data-ttu-id="44c95-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44c95-116">Application</span></span>     | <span data-ttu-id="44c95-117">Нет</span><span class="sxs-lookup"><span data-stu-id="44c95-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="44c95-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44c95-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /communications/calls/{id}/participants/{id}/mute
```
> <span data-ttu-id="44c95-119">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="44c95-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="44c95-120">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="44c95-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44c95-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44c95-121">Request headers</span></span>
| <span data-ttu-id="44c95-122">Имя</span><span class="sxs-lookup"><span data-stu-id="44c95-122">Name</span></span>          | <span data-ttu-id="44c95-123">Описание</span><span class="sxs-lookup"><span data-stu-id="44c95-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="44c95-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44c95-124">Authorization</span></span> | <span data-ttu-id="44c95-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44c95-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44c95-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="44c95-127">Content-type</span></span>  | <span data-ttu-id="44c95-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44c95-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44c95-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44c95-130">Request body</span></span>
<span data-ttu-id="44c95-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="44c95-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="44c95-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="44c95-132">Parameter</span></span>      | <span data-ttu-id="44c95-133">Тип</span><span class="sxs-lookup"><span data-stu-id="44c95-133">Type</span></span>    |<span data-ttu-id="44c95-134">Описание</span><span class="sxs-lookup"><span data-stu-id="44c95-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44c95-135">Контекст</span><span class="sxs-lookup"><span data-stu-id="44c95-135">clientContext</span></span>|<span data-ttu-id="44c95-136">String</span><span class="sxs-lookup"><span data-stu-id="44c95-136">String</span></span>|<span data-ttu-id="44c95-137">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="44c95-137">Unique Client Context string.</span></span> <span data-ttu-id="44c95-138">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="44c95-138">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="44c95-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="44c95-139">Response</span></span>
<span data-ttu-id="44c95-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мутепартиЦипантоператион](../resources/muteParticipantoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44c95-140">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="44c95-141">**Примечание:** Когда этот API возвращает успешный ответ, все участники получат обновление списка.</span><span class="sxs-lookup"><span data-stu-id="44c95-141">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example---mute-specific-participant"></a><span data-ttu-id="44c95-142">Пример: Специальный участник</span><span class="sxs-lookup"><span data-stu-id="44c95-142">Example - Mute specific participant</span></span>
<span data-ttu-id="44c95-143">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="44c95-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="44c95-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="44c95-144">Request</span></span>
<span data-ttu-id="44c95-145">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44c95-145">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="44c95-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="44c95-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="44c95-147">C#</span><span class="sxs-lookup"><span data-stu-id="44c95-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44c95-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44c95-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44c95-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44c95-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="44c95-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="44c95-150">Response</span></span>

> <span data-ttu-id="44c95-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44c95-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 


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

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="44c95-153">Список уведомлений обновлен с отключенным участником</span><span class="sxs-lookup"><span data-stu-id="44c95-153">Notification - roster updated with participant muted</span></span>

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
