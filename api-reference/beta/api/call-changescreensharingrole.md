---
title: 'Call: Чанжескриншарингроле'
description: Разрешить приложениям предоставлять доступ к содержимому экрана участникам группового вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d670e2b1be4450b33e57ca0834aecd1f6427603d
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006356"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="f7dc6-103">Call: Чанжескриншарингроле</span><span class="sxs-lookup"><span data-stu-id="f7dc6-103">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7dc6-104">Разрешить приложениям предоставлять доступ к содержимому экрана участникам группового вызова.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-104">Allow applications to share screen content with the participants of a group call.</span></span>

> <span data-ttu-id="f7dc6-105">**Примечание:** Это поддерживается только для звонков групп, использующих мультимедиа, размещаемых в приложении.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-105">**Note:** This is only supported for group calls that use App-Hosted Media.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7dc6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7dc6-106">Permissions</span></span>
<span data-ttu-id="f7dc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7dc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7dc6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7dc6-109">Permission type</span></span>                        | <span data-ttu-id="f7dc6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7dc6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7dc6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7dc6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7dc6-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f7dc6-112">Not Supported</span></span>                               |
| <span data-ttu-id="f7dc6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7dc6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7dc6-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f7dc6-114">Not Supported</span></span>                               |
| <span data-ttu-id="f7dc6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7dc6-115">Application</span></span>                            | <span data-ttu-id="f7dc6-116">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="f7dc6-116">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="f7dc6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7dc6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /communications/calls/{id}/changeScreenSharingRole
```
> <span data-ttu-id="f7dc6-118">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="f7dc6-119">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7dc6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7dc6-120">Request headers</span></span>
| <span data-ttu-id="f7dc6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f7dc6-121">Name</span></span>          | <span data-ttu-id="f7dc6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f7dc6-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f7dc6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7dc6-123">Authorization</span></span> | <span data-ttu-id="f7dc6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7dc6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7dc6-126">Content-type</span></span>  | <span data-ttu-id="f7dc6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7dc6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7dc6-129">Request body</span></span>
<span data-ttu-id="f7dc6-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7dc6-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="f7dc6-131">Parameter</span></span>      | <span data-ttu-id="f7dc6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f7dc6-132">Type</span></span>    |<span data-ttu-id="f7dc6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f7dc6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7dc6-134">role</span><span class="sxs-lookup"><span data-stu-id="f7dc6-134">role</span></span>|<span data-ttu-id="f7dc6-135">String</span><span class="sxs-lookup"><span data-stu-id="f7dc6-135">String</span></span>|<span data-ttu-id="f7dc6-136">Возможные значения: "средство просмотра", "общий доступ"</span><span class="sxs-lookup"><span data-stu-id="f7dc6-136">Possible values are: 'viewer', 'sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="f7dc6-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7dc6-137">Response</span></span>
<span data-ttu-id="f7dc6-138">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика, а все участники получат обновление списка.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-138">If successful, this method returns a `202 Accepted` response code, and all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="f7dc6-139">Пример</span><span class="sxs-lookup"><span data-stu-id="f7dc6-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f7dc6-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7dc6-140">Request</span></span>
<span data-ttu-id="f7dc6-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f7dc6-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7dc6-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7dc6-143">C#</span><span class="sxs-lookup"><span data-stu-id="f7dc6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7dc6-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7dc6-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7dc6-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7dc6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f7dc6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7dc6-146">Response</span></span>
<span data-ttu-id="f7dc6-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-147">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---roster-updated-with-participant-sending-screen-sharing-video"></a><span data-ttu-id="f7dc6-148">Уведомление о подсписке, обновленный при отправке участником демонстрации экрана общего видео</span><span class="sxs-lookup"><span data-stu-id="f7dc6-148">Notification - roster updated with participant sending screen sharing video</span></span>
<span data-ttu-id="f7dc6-149">Обратите `direction: sendOnly` внимание на свойство в потоке мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="f7dc6-149">Note the `direction: sendOnly` property on the media stream.</span></span>

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
