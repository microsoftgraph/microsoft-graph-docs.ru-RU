---
title: 'вызов: включение звука'
description: Разрешить приложению включить Автоотключение.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 51ad26211208934599feb65d4f932d8654fd170e
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913634"
---
# <a name="call-unmute"></a><span data-ttu-id="a4ba9-103">вызов: включение звука</span><span class="sxs-lookup"><span data-stu-id="a4ba9-103">call: unmute</span></span>

<span data-ttu-id="a4ba9-104">Разрешить приложению включить Автоотключение.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-104">Allow the application to unmute itself.</span></span>

<span data-ttu-id="a4ba9-105">Это нерекомендуемый сервер, что означает, что сервер еще раз начнет отправлять звуковые пакеты для этого участника другим участникам.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-105">This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.</span></span>

<span data-ttu-id="a4ba9-106">Дополнительные сведения о том, как обрабатывать звуковые операции, приведены в статье [унмутепартиЦипантоператион](../resources/unmuteParticipantoperation.md).</span><span class="sxs-lookup"><span data-stu-id="a4ba9-106">For more information about how to handle unmute operations, see [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md).</span></span>

> <span data-ttu-id="a4ba9-107">**Примечание:** Этот метод поддерживается только для вызовов групп.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-107">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4ba9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4ba9-108">Permissions</span></span>

| <span data-ttu-id="a4ba9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4ba9-109">Permission type</span></span>                        | <span data-ttu-id="a4ba9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4ba9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a4ba9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4ba9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4ba9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-112">Not supported.</span></span>                               |
| <span data-ttu-id="a4ba9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4ba9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4ba9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-114">Not supported.</span></span>                               |
| <span data-ttu-id="a4ba9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4ba9-115">Application</span></span>                            | <span data-ttu-id="a4ba9-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-116">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="a4ba9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4ba9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="a4ba9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4ba9-118">Request headers</span></span>
| <span data-ttu-id="a4ba9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a4ba9-119">Name</span></span>          | <span data-ttu-id="a4ba9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ba9-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a4ba9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4ba9-121">Authorization</span></span> | <span data-ttu-id="a4ba9-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4ba9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4ba9-124">Content-type</span></span> | <span data-ttu-id="a4ba9-p102">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-p102">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4ba9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4ba9-127">Request body</span></span>
<span data-ttu-id="a4ba9-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4ba9-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="a4ba9-129">Parameter</span></span>      | <span data-ttu-id="a4ba9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a4ba9-130">Type</span></span>    |<span data-ttu-id="a4ba9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ba9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4ba9-132">Контекст</span><span class="sxs-lookup"><span data-stu-id="a4ba9-132">clientContext</span></span>|<span data-ttu-id="a4ba9-133">String</span><span class="sxs-lookup"><span data-stu-id="a4ba9-133">String</span></span>|<span data-ttu-id="a4ba9-134">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-134">Unique Client Context string.</span></span> <span data-ttu-id="a4ba9-135">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-135">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="a4ba9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4ba9-136">Response</span></span>
<span data-ttu-id="a4ba9-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [унмутепартиЦипантоператион](../resources/unmuteParticipantoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-137">If successful, this method returns a `200 OK` response code and a [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="a4ba9-138">**Примечание:** Когда этот API возвращает успешный ответ, все участники получат обновление списка.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-138">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="a4ba9-139">Пример</span><span class="sxs-lookup"><span data-stu-id="a4ba9-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a4ba9-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4ba9-140">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a4ba9-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4ba9-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4ba9-142">C#</span><span class="sxs-lookup"><span data-stu-id="a4ba9-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4ba9-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4ba9-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4ba9-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4ba9-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a4ba9-145">Java</span><span class="sxs-lookup"><span data-stu-id="a4ba9-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-unmute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a4ba9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4ba9-146">Response</span></span>

> <span data-ttu-id="a4ba9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4ba9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#unmuteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-unmuted"></a><span data-ttu-id="a4ba9-149">Список уведомлений обновлен с невключенным участником</span><span class="sxs-lookup"><span data-stu-id="a4ba9-149">Notification - roster updated with participant unmuted</span></span>

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
