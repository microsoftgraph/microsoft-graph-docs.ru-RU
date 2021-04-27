---
title: 'вызов: не игнорировать'
description: Разрешить приложению отметь себя.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1e995e17bfd98b26ae4680c1215a56d231e0116c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047604"
---
# <a name="call-unmute"></a><span data-ttu-id="03ec9-103">вызов: не игнорировать</span><span class="sxs-lookup"><span data-stu-id="03ec9-103">call: unmute</span></span>

<span data-ttu-id="03ec9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03ec9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03ec9-105">Разрешить приложению отметь себя.</span><span class="sxs-lookup"><span data-stu-id="03ec9-105">Allow the application to unmute itself.</span></span>

<span data-ttu-id="03ec9-106">Это неуправляемый сервер, что означает, что сервер снова начнет отправлять аудио пакеты для этого участника другим участникам.</span><span class="sxs-lookup"><span data-stu-id="03ec9-106">This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.</span></span>

<span data-ttu-id="03ec9-107">Дополнительные сведения о том, как обрабатывать незамысленные операции, см. в [нем unmuteParticipantOperation.](../resources/unmuteParticipantoperation.md)</span><span class="sxs-lookup"><span data-stu-id="03ec9-107">For more information about how to handle unmute operations, see [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md).</span></span>

> <span data-ttu-id="03ec9-108">**Примечание:** Этот метод поддерживается только для групповых вызовов.</span><span class="sxs-lookup"><span data-stu-id="03ec9-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="03ec9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03ec9-109">Permissions</span></span>

| <span data-ttu-id="03ec9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03ec9-110">Permission type</span></span>                        | <span data-ttu-id="03ec9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03ec9-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03ec9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03ec9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="03ec9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03ec9-113">Not supported.</span></span>                               |
| <span data-ttu-id="03ec9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03ec9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03ec9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03ec9-115">Not supported.</span></span>                               |
| <span data-ttu-id="03ec9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03ec9-116">Application</span></span>                            | <span data-ttu-id="03ec9-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="03ec9-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="03ec9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03ec9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /communications/calls/{id}/unmute
```
> <span data-ttu-id="03ec9-119">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="03ec9-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="03ec9-120">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="03ec9-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03ec9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03ec9-121">Request headers</span></span>
| <span data-ttu-id="03ec9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="03ec9-122">Name</span></span>          | <span data-ttu-id="03ec9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="03ec9-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="03ec9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03ec9-124">Authorization</span></span> | <span data-ttu-id="03ec9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03ec9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03ec9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03ec9-127">Content-type</span></span> | <span data-ttu-id="03ec9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03ec9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03ec9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03ec9-130">Request body</span></span>
<span data-ttu-id="03ec9-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="03ec9-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03ec9-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="03ec9-132">Parameter</span></span>      | <span data-ttu-id="03ec9-133">Тип</span><span class="sxs-lookup"><span data-stu-id="03ec9-133">Type</span></span>    |<span data-ttu-id="03ec9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="03ec9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03ec9-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="03ec9-135">clientContext</span></span>|<span data-ttu-id="03ec9-136">String</span><span class="sxs-lookup"><span data-stu-id="03ec9-136">String</span></span>|<span data-ttu-id="03ec9-137">Клиентский контекст.</span><span class="sxs-lookup"><span data-stu-id="03ec9-137">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="03ec9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="03ec9-138">Response</span></span>
<span data-ttu-id="03ec9-139">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="03ec9-139">If successful, this method returns a `200 OK` response code and a [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="03ec9-140">**Примечание:** Когда этот API возвращает успешный ответ, все участники получат обновление реестра.</span><span class="sxs-lookup"><span data-stu-id="03ec9-140">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="03ec9-141">Пример</span><span class="sxs-lookup"><span data-stu-id="03ec9-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="03ec9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="03ec9-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="03ec9-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="03ec9-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="03ec9-144">C#</span><span class="sxs-lookup"><span data-stu-id="03ec9-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03ec9-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03ec9-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03ec9-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03ec9-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03ec9-147">Java</span><span class="sxs-lookup"><span data-stu-id="03ec9-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-unmute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="03ec9-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="03ec9-148">Response</span></span>

> <span data-ttu-id="03ec9-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="03ec9-149">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.unmuteParticipantOperation",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.unmuteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#unmuteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-unmuted"></a><span data-ttu-id="03ec9-150">Уведомление — список обновляется с помощью ненагрузки участника</span><span class="sxs-lookup"><span data-stu-id="03ec9-150">Notification - roster updated with participant unmuted</span></span>

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


