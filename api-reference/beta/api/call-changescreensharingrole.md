---
title: 'Call: Чанжескриншарингроле'
description: Разрешить приложениям предоставлять доступ к содержимому экрана участникам группового вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 333a9a2ebb6fa5b3c43ccee47f0256ef5ba6dee3
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912771"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="27e1d-103">Call: Чанжескриншарингроле</span><span class="sxs-lookup"><span data-stu-id="27e1d-103">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27e1d-104">Разрешить приложениям предоставлять доступ к содержимому экрана участникам группового вызова.</span><span class="sxs-lookup"><span data-stu-id="27e1d-104">Allow applications to share screen content with the participants of a group call.</span></span>

> <span data-ttu-id="27e1d-105">**Примечание:** Это поддерживается только для звонков групп, использующих мультимедиа, размещаемых в приложении.</span><span class="sxs-lookup"><span data-stu-id="27e1d-105">**Note:** This is only supported for group calls that use App-Hosted Media.</span></span>

## <a name="permissions"></a><span data-ttu-id="27e1d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27e1d-106">Permissions</span></span>
<span data-ttu-id="27e1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27e1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27e1d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27e1d-109">Permission type</span></span>                        | <span data-ttu-id="27e1d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27e1d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27e1d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27e1d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="27e1d-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27e1d-112">Not Supported</span></span>                               |
| <span data-ttu-id="27e1d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27e1d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27e1d-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27e1d-114">Not Supported</span></span>                               |
| <span data-ttu-id="27e1d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27e1d-115">Application</span></span>                            | <span data-ttu-id="27e1d-116">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="27e1d-116">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="27e1d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27e1d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /communications/calls/{id}/changeScreenSharingRole
```
> <span data-ttu-id="27e1d-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="27e1d-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="27e1d-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="27e1d-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27e1d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27e1d-120">Request headers</span></span>
| <span data-ttu-id="27e1d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="27e1d-121">Name</span></span>          | <span data-ttu-id="27e1d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="27e1d-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="27e1d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27e1d-123">Authorization</span></span> | <span data-ttu-id="27e1d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27e1d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27e1d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27e1d-126">Content-type</span></span>  | <span data-ttu-id="27e1d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27e1d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27e1d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27e1d-129">Request body</span></span>
<span data-ttu-id="27e1d-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="27e1d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="27e1d-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="27e1d-131">Parameter</span></span>      | <span data-ttu-id="27e1d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="27e1d-132">Type</span></span>    |<span data-ttu-id="27e1d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="27e1d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27e1d-134">role</span><span class="sxs-lookup"><span data-stu-id="27e1d-134">role</span></span>|<span data-ttu-id="27e1d-135">String</span><span class="sxs-lookup"><span data-stu-id="27e1d-135">String</span></span>|<span data-ttu-id="27e1d-136">Возможные значения: "средство просмотра", "общий доступ"</span><span class="sxs-lookup"><span data-stu-id="27e1d-136">Possible values are: 'viewer', 'sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="27e1d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="27e1d-137">Response</span></span>
<span data-ttu-id="27e1d-138">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика, а все участники получат обновление списка.</span><span class="sxs-lookup"><span data-stu-id="27e1d-138">If successful, this method returns a `202 Accepted` response code, and all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="27e1d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="27e1d-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="27e1d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="27e1d-140">Request</span></span>
<span data-ttu-id="27e1d-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27e1d-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="27e1d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="27e1d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="27e1d-143">C#</span><span class="sxs-lookup"><span data-stu-id="27e1d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27e1d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27e1d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27e1d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27e1d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="27e1d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="27e1d-146">Response</span></span>
<span data-ttu-id="27e1d-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27e1d-147">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---roster-updated-with-participant-sending-screen-sharing-video"></a><span data-ttu-id="27e1d-148">Уведомление о подсписке, обновленный при отправке участником демонстрации экрана общего видео</span><span class="sxs-lookup"><span data-stu-id="27e1d-148">Notification - roster updated with participant sending screen sharing video</span></span>
<span data-ttu-id="27e1d-149">Обратите `direction: sendOnly` внимание на свойство в потоке мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="27e1d-149">Note the `direction: sendOnly` property on the media stream.</span></span>

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
              "mediaType": "videoBasedScreenSharing",
              "label": "applicationsharing-video",
              "sourceId": "1",
              "direction": "sendOnly"
            }
          ],
          "isMuted": false,
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
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
