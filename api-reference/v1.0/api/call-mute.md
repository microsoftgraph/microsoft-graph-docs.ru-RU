---
title: 'вызов: выкл.'
description: Позволяет приложению отключить себя.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5adca2897a2582764bc435307e322edbd0af6c02
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913277"
---
# <a name="call-mute"></a><span data-ttu-id="c745c-103">вызов: выкл.</span><span class="sxs-lookup"><span data-stu-id="c745c-103">call: mute</span></span>

<span data-ttu-id="c745c-104">Позволяет приложению отключить себя.</span><span class="sxs-lookup"><span data-stu-id="c745c-104">Allows the application to mute itself.</span></span>

<span data-ttu-id="c745c-105">Это Выключенный сервер, что означает, что сервер будет отбрасывать все звуковые пакеты для этого участника, даже если участник продолжает потоковую передачу звука.</span><span class="sxs-lookup"><span data-stu-id="c745c-105">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="c745c-106">Более подробную информацию о том, как обрабатывать операции отключения звука, можно узнать в статье [мутепартиЦипантоператион](../resources/muteparticipantoperation.md)</span><span class="sxs-lookup"><span data-stu-id="c745c-106">For more details about how to handle mute operations, see [muteParticipantOperation](../resources/muteparticipantoperation.md)</span></span>

> <span data-ttu-id="c745c-107">**Примечание:** Этот метод поддерживается только для вызовов групп.</span><span class="sxs-lookup"><span data-stu-id="c745c-107">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="c745c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c745c-108">Permissions</span></span>
<span data-ttu-id="c745c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c745c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c745c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c745c-111">Permission type</span></span>                        | <span data-ttu-id="c745c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c745c-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c745c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c745c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c745c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c745c-114">Not Supported.</span></span>                               |
| <span data-ttu-id="c745c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c745c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c745c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c745c-116">Not Supported.</span></span>                               |
| <span data-ttu-id="c745c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c745c-117">Application</span></span>                            | <span data-ttu-id="c745c-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="c745c-118">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="c745c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c745c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="c745c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c745c-120">Request headers</span></span>
| <span data-ttu-id="c745c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c745c-121">Name</span></span>          | <span data-ttu-id="c745c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c745c-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c745c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c745c-123">Authorization</span></span> | <span data-ttu-id="c745c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c745c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c745c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c745c-126">Content-type</span></span> | <span data-ttu-id="c745c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c745c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c745c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c745c-129">Request body</span></span>
<span data-ttu-id="c745c-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c745c-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c745c-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="c745c-131">Parameter</span></span>      | <span data-ttu-id="c745c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c745c-132">Type</span></span>    |<span data-ttu-id="c745c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c745c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c745c-134">Контекст</span><span class="sxs-lookup"><span data-stu-id="c745c-134">clientContext</span></span>|<span data-ttu-id="c745c-135">String</span><span class="sxs-lookup"><span data-stu-id="c745c-135">String</span></span>|<span data-ttu-id="c745c-136">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="c745c-136">Unique Client Context string.</span></span> <span data-ttu-id="c745c-137">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="c745c-137">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="c745c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c745c-138">Response</span></span>
<span data-ttu-id="c745c-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [мутепартиЦипантоператион](../resources/muteParticipantoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c745c-139">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

> <span data-ttu-id="c745c-140">**Примечание:** После того как эта операция возвращает успешный ответ, все участники получат обновление списка</span><span class="sxs-lookup"><span data-stu-id="c745c-140">**Note:** After this operation returns a successful response, all participants will receive a roster update</span></span>

## <a name="example"></a><span data-ttu-id="c745c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c745c-141">Example</span></span>
<span data-ttu-id="c745c-142">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c745c-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c745c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="c745c-143">Request</span></span>
<span data-ttu-id="c745c-144">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c745c-144">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c745c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="c745c-145">HTTP</span></span>](#tab/http)
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

# <a name="ctabcsharp"></a>[<span data-ttu-id="c745c-146">C#</span><span class="sxs-lookup"><span data-stu-id="c745c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c745c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c745c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c745c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c745c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c745c-149">Java</span><span class="sxs-lookup"><span data-stu-id="c745c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c745c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c745c-150">Response</span></span>

> <span data-ttu-id="c745c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c745c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
 
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

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="c745c-153">Список уведомлений обновлен с отключенным участником</span><span class="sxs-lookup"><span data-stu-id="c745c-153">Notification - roster updated with participant muted</span></span>

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
