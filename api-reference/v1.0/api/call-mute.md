---
title: 'вызов: отключить'
description: Позволяет приложению отключить себя.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 016fbd3dbad85dfaf9eb0b09d840532ce27a1c01
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52784936"
---
# <a name="call-mute"></a><span data-ttu-id="449e5-103">вызов: отключить</span><span class="sxs-lookup"><span data-stu-id="449e5-103">call: mute</span></span>

<span data-ttu-id="449e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="449e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="449e5-105">Позволяет приложению отключить себя.</span><span class="sxs-lookup"><span data-stu-id="449e5-105">Allows the application to mute itself.</span></span>

<span data-ttu-id="449e5-106">Это отключить сервер, что означает, что сервер отпадет все аудио пакеты для этого участника, даже если участник продолжает поток звука.</span><span class="sxs-lookup"><span data-stu-id="449e5-106">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="449e5-107">Дополнительные сведения о том, как обрабатывать операции немой обработки, см. в материале [muteParticipantOperation](../resources/muteparticipantoperation.md)</span><span class="sxs-lookup"><span data-stu-id="449e5-107">For more details about how to handle mute operations, see [muteParticipantOperation](../resources/muteparticipantoperation.md)</span></span>

> <span data-ttu-id="449e5-108">**Примечание:** Этот метод поддерживается только для групповых вызовов.</span><span class="sxs-lookup"><span data-stu-id="449e5-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="449e5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="449e5-109">Permissions</span></span>
<span data-ttu-id="449e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="449e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="449e5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="449e5-112">Permission type</span></span>                        | <span data-ttu-id="449e5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="449e5-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="449e5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="449e5-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="449e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="449e5-115">Not Supported.</span></span>                               |
| <span data-ttu-id="449e5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="449e5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="449e5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="449e5-117">Not Supported.</span></span>                               |
| <span data-ttu-id="449e5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="449e5-118">Application</span></span>                            | <span data-ttu-id="449e5-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="449e5-119">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="449e5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="449e5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="449e5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="449e5-121">Request headers</span></span>
| <span data-ttu-id="449e5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="449e5-122">Name</span></span>          | <span data-ttu-id="449e5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="449e5-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="449e5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="449e5-124">Authorization</span></span> | <span data-ttu-id="449e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="449e5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="449e5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="449e5-127">Content-type</span></span> | <span data-ttu-id="449e5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="449e5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="449e5-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="449e5-130">Request body</span></span>
<span data-ttu-id="449e5-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="449e5-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="449e5-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="449e5-132">Parameter</span></span>      | <span data-ttu-id="449e5-133">Тип</span><span class="sxs-lookup"><span data-stu-id="449e5-133">Type</span></span>    |<span data-ttu-id="449e5-134">Описание</span><span class="sxs-lookup"><span data-stu-id="449e5-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="449e5-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="449e5-135">clientContext</span></span>|<span data-ttu-id="449e5-136">String</span><span class="sxs-lookup"><span data-stu-id="449e5-136">String</span></span>|<span data-ttu-id="449e5-137">Уникальная строка Client Context.</span><span class="sxs-lookup"><span data-stu-id="449e5-137">Unique Client Context string.</span></span> <span data-ttu-id="449e5-138">Максимальное ограничение — 256 шаров.</span><span class="sxs-lookup"><span data-stu-id="449e5-138">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="449e5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="449e5-139">Response</span></span>
<span data-ttu-id="449e5-140">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект muteParticipantOperation](../resources/muteParticipantoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="449e5-140">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

> <span data-ttu-id="449e5-141">**Примечание:** После успешного ответа на эту операцию все участники получат обновление реестра</span><span class="sxs-lookup"><span data-stu-id="449e5-141">**Note:** After this operation returns a successful response, all participants will receive a roster update</span></span>

## <a name="example"></a><span data-ttu-id="449e5-142">Пример</span><span class="sxs-lookup"><span data-stu-id="449e5-142">Example</span></span>
<span data-ttu-id="449e5-143">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="449e5-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="449e5-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="449e5-144">Request</span></span>
<span data-ttu-id="449e5-145">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="449e5-145">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="449e5-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="449e5-146">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="449e5-147">C#</span><span class="sxs-lookup"><span data-stu-id="449e5-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="449e5-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="449e5-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="449e5-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="449e5-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="449e5-150">Java</span><span class="sxs-lookup"><span data-stu-id="449e5-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="449e5-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="449e5-151">Response</span></span>

> <span data-ttu-id="449e5-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="449e5-152">**Note:** The response object shown here might be shortened for readability.</span></span> 
 
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

{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="449e5-153">Уведомление — список, обновленный с отключенным участником</span><span class="sxs-lookup"><span data-stu-id="449e5-153">Notification - roster updated with participant muted</span></span>

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

