---
title: 'вызов: выкл.'
description: Позволяет приложению отключить себя.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c80228d654f41742eed2f96b9e18ac9bfd6ca4d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966270"
---
# <a name="call-mute"></a><span data-ttu-id="779a3-103">вызов: выкл.</span><span class="sxs-lookup"><span data-stu-id="779a3-103">call: mute</span></span>

<span data-ttu-id="779a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="779a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="779a3-105">Позволяет приложению отключить себя.</span><span class="sxs-lookup"><span data-stu-id="779a3-105">Allows the application to mute itself.</span></span>

<span data-ttu-id="779a3-106">Это Выключенный сервер, что означает, что сервер будет отбрасывать все звуковые пакеты для этого участника, даже если участник продолжает потоковую передачу звука.</span><span class="sxs-lookup"><span data-stu-id="779a3-106">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="779a3-107">Более подробную информацию о том, как обрабатывать операции отключения звука, можно узнать в статье [мутепартиЦипантоператион](../resources/muteparticipantoperation.md)</span><span class="sxs-lookup"><span data-stu-id="779a3-107">For more details about how to handle mute operations, see [muteParticipantOperation](../resources/muteparticipantoperation.md)</span></span>

> <span data-ttu-id="779a3-108">**Примечание:** Этот метод поддерживается только для вызовов групп.</span><span class="sxs-lookup"><span data-stu-id="779a3-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="779a3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="779a3-109">Permissions</span></span>
<span data-ttu-id="779a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="779a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="779a3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="779a3-112">Permission type</span></span>                        | <span data-ttu-id="779a3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="779a3-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="779a3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="779a3-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="779a3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="779a3-115">Not Supported.</span></span>                               |
| <span data-ttu-id="779a3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="779a3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="779a3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="779a3-117">Not Supported.</span></span>                               |
| <span data-ttu-id="779a3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="779a3-118">Application</span></span>                            | <span data-ttu-id="779a3-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="779a3-119">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="779a3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="779a3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="779a3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="779a3-121">Request headers</span></span>
| <span data-ttu-id="779a3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="779a3-122">Name</span></span>          | <span data-ttu-id="779a3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="779a3-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="779a3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="779a3-124">Authorization</span></span> | <span data-ttu-id="779a3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="779a3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="779a3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="779a3-127">Content-type</span></span> | <span data-ttu-id="779a3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="779a3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="779a3-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="779a3-130">Request body</span></span>
<span data-ttu-id="779a3-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="779a3-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="779a3-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="779a3-132">Parameter</span></span>      | <span data-ttu-id="779a3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="779a3-133">Type</span></span>    |<span data-ttu-id="779a3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="779a3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="779a3-135">Контекст</span><span class="sxs-lookup"><span data-stu-id="779a3-135">clientContext</span></span>|<span data-ttu-id="779a3-136">String</span><span class="sxs-lookup"><span data-stu-id="779a3-136">String</span></span>|<span data-ttu-id="779a3-137">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="779a3-137">Unique Client Context string.</span></span> <span data-ttu-id="779a3-138">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="779a3-138">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="779a3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="779a3-139">Response</span></span>
<span data-ttu-id="779a3-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мутепартиЦипантоператион](../resources/muteParticipantoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="779a3-140">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

> <span data-ttu-id="779a3-141">**Примечание:** После того как эта операция возвращает успешный ответ, все участники получат обновление списка</span><span class="sxs-lookup"><span data-stu-id="779a3-141">**Note:** After this operation returns a successful response, all participants will receive a roster update</span></span>

## <a name="example"></a><span data-ttu-id="779a3-142">Пример</span><span class="sxs-lookup"><span data-stu-id="779a3-142">Example</span></span>
<span data-ttu-id="779a3-143">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="779a3-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="779a3-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="779a3-144">Request</span></span>
<span data-ttu-id="779a3-145">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="779a3-145">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="779a3-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="779a3-146">HTTP</span></span>](#tab/http)
<!-- { 
  "blockType": "request", 
  "name": "call-mute" 
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/mute
Content-Type: application/json

{
  "clientContext": "clientContext-value"
}
```

# <a name="c"></a>[<span data-ttu-id="779a3-147">C#</span><span class="sxs-lookup"><span data-stu-id="779a3-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="779a3-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="779a3-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="779a3-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="779a3-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="779a3-150">Java</span><span class="sxs-lookup"><span data-stu-id="779a3-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="779a3-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="779a3-151">Response</span></span>

> <span data-ttu-id="779a3-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="779a3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
 
<!-- { 
  "blockType": "response", 
  "truncated": true, 
  "@odata.type": "microsoft.graph.muteParticipantOperation" 
} --> 
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.muteParticipantOperation",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="779a3-154">Список уведомлений обновлен с отключенным участником</span><span class="sxs-lookup"><span data-stu-id="779a3-154">Notification - roster updated with participant muted</span></span>

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

