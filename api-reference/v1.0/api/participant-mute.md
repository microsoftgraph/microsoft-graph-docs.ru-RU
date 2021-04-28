---
title: 'участник: отключить'
description: Отключить определенный участник вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a74b2ed36831960ba27b48742f91f99333c69efb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051314"
---
# <a name="participant-mute"></a><span data-ttu-id="10df2-103">участник: отключить</span><span class="sxs-lookup"><span data-stu-id="10df2-103">participant: mute</span></span>

<span data-ttu-id="10df2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10df2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10df2-105">Отключить определенный участник вызова.</span><span class="sxs-lookup"><span data-stu-id="10df2-105">Mute a specific participant in the call.</span></span>

<span data-ttu-id="10df2-106">Это отключить сервер, что означает, что сервер отпадет все аудио пакеты для этого участника, даже если участник продолжает поток звука.</span><span class="sxs-lookup"><span data-stu-id="10df2-106">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="10df2-107">Дополнительные сведения об обработке операций немой обработки см. в [muteParticipantOperation.](../resources/muteParticipantoperation.md)</span><span class="sxs-lookup"><span data-stu-id="10df2-107">For more information about how to handle mute operations, see [muteParticipantOperation](../resources/muteParticipantoperation.md).</span></span>

> <span data-ttu-id="10df2-108">**Примечание:** Этот метод поддерживается только для групповых вызовов.</span><span class="sxs-lookup"><span data-stu-id="10df2-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="10df2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10df2-109">Permissions</span></span>

| <span data-ttu-id="10df2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10df2-110">Permission type</span></span> | <span data-ttu-id="10df2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10df2-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="10df2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10df2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="10df2-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10df2-113">Not Supported</span></span>        |
| <span data-ttu-id="10df2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10df2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10df2-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10df2-115">Not Supported</span></span>        |
| <span data-ttu-id="10df2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10df2-116">Application</span></span>     | <span data-ttu-id="10df2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="10df2-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="10df2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10df2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="10df2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10df2-119">Request headers</span></span>
| <span data-ttu-id="10df2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="10df2-120">Name</span></span>          | <span data-ttu-id="10df2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="10df2-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="10df2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10df2-122">Authorization</span></span> | <span data-ttu-id="10df2-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10df2-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="10df2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10df2-125">Content-type</span></span>  | <span data-ttu-id="10df2-p102">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10df2-p102">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10df2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10df2-128">Request body</span></span>
<span data-ttu-id="10df2-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="10df2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="10df2-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="10df2-130">Parameter</span></span>      | <span data-ttu-id="10df2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="10df2-131">Type</span></span>    |<span data-ttu-id="10df2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="10df2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10df2-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="10df2-133">clientContext</span></span>|<span data-ttu-id="10df2-134">String</span><span class="sxs-lookup"><span data-stu-id="10df2-134">String</span></span>|<span data-ttu-id="10df2-135">Уникальная строка Client Context.</span><span class="sxs-lookup"><span data-stu-id="10df2-135">Unique Client Context string.</span></span> <span data-ttu-id="10df2-136">Максимальное ограничение — 256 шаров.</span><span class="sxs-lookup"><span data-stu-id="10df2-136">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="10df2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="10df2-137">Response</span></span>
<span data-ttu-id="10df2-138">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект muteParticipantOperation](../resources/muteParticipantoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="10df2-138">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="10df2-139">**Примечание:** Когда этот API возвращает успешный ответ, все участники получат обновление реестра.</span><span class="sxs-lookup"><span data-stu-id="10df2-139">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example---mute-specific-participant"></a><span data-ttu-id="10df2-140">Пример : Отключить определенный участник</span><span class="sxs-lookup"><span data-stu-id="10df2-140">Example - Mute specific participant</span></span>
<span data-ttu-id="10df2-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="10df2-141">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="10df2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="10df2-142">Request</span></span>
<span data-ttu-id="10df2-143">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10df2-143">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10df2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="10df2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants/2765eb15-01f8-47c6-b12b-c32111a4a86f/mute
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```
# <a name="c"></a>[<span data-ttu-id="10df2-145">C#</span><span class="sxs-lookup"><span data-stu-id="10df2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10df2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10df2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10df2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10df2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10df2-148">Java</span><span class="sxs-lookup"><span data-stu-id="10df2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="10df2-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="10df2-149">Response</span></span>

> <span data-ttu-id="10df2-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="10df2-150">**Note:** The response object shown here might be shortened for readability.</span></span> 


<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.muteParticipantOperation",
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="10df2-151">Уведомление — список, обновленный с отключенным участником</span><span class="sxs-lookup"><span data-stu-id="10df2-151">Notification - roster updated with participant muted</span></span>

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

