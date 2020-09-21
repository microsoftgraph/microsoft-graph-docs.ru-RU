---
title: 'Call: Чанжескриншарингроле'
description: Разрешить приложениям предоставлять доступ к содержимому экрана участникам группового вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b6620eb941ef2b3a18bb15f756263c09388df84d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966382"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="4b6c6-103">Call: Чанжескриншарингроле</span><span class="sxs-lookup"><span data-stu-id="4b6c6-103">call: changeScreenSharingRole</span></span>

<span data-ttu-id="4b6c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b6c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4b6c6-105">Разрешить приложениям предоставлять доступ к содержимому экрана участникам группового вызова.</span><span class="sxs-lookup"><span data-stu-id="4b6c6-105">Allow applications to share screen content with the participants of a group call.</span></span>

> <span data-ttu-id="4b6c6-106">**Примечание:** Это поддерживается только для звонков групп, использующих мультимедиа, размещаемых в приложении.</span><span class="sxs-lookup"><span data-stu-id="4b6c6-106">**Note:** This is only supported for group calls that use App-Hosted Media.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b6c6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b6c6-107">Permissions</span></span>
<span data-ttu-id="4b6c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b6c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b6c6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b6c6-110">Permission type</span></span>                        | <span data-ttu-id="4b6c6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b6c6-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b6c6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b6c6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b6c6-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4b6c6-113">Not Supported</span></span>                               |
| <span data-ttu-id="4b6c6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b6c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b6c6-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4b6c6-115">Not Supported</span></span>                               |
| <span data-ttu-id="4b6c6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b6c6-116">Application</span></span>                            | <span data-ttu-id="4b6c6-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="4b6c6-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="4b6c6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b6c6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="4b6c6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b6c6-119">Request headers</span></span>
| <span data-ttu-id="4b6c6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4b6c6-120">Name</span></span>          | <span data-ttu-id="4b6c6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4b6c6-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4b6c6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b6c6-122">Authorization</span></span> | <span data-ttu-id="4b6c6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b6c6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b6c6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b6c6-125">Content-type</span></span>  | <span data-ttu-id="4b6c6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b6c6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b6c6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b6c6-128">Request body</span></span>
<span data-ttu-id="4b6c6-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4b6c6-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4b6c6-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="4b6c6-130">Parameter</span></span>      | <span data-ttu-id="4b6c6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b6c6-131">Type</span></span>    |<span data-ttu-id="4b6c6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b6c6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b6c6-133">role</span><span class="sxs-lookup"><span data-stu-id="4b6c6-133">role</span></span>|<span data-ttu-id="4b6c6-134">String</span><span class="sxs-lookup"><span data-stu-id="4b6c6-134">String</span></span>|<span data-ttu-id="4b6c6-135">Возможные значения: "средство просмотра", "общий доступ"</span><span class="sxs-lookup"><span data-stu-id="4b6c6-135">Possible values are: 'viewer', 'sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="4b6c6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b6c6-136">Response</span></span>
<span data-ttu-id="4b6c6-137">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика, а все участники получат обновление списка.</span><span class="sxs-lookup"><span data-stu-id="4b6c6-137">If successful, this method returns a `202 Accepted` response code, and all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="4b6c6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4b6c6-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4b6c6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b6c6-139">Request</span></span>
<span data-ttu-id="4b6c6-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b6c6-140">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b6c6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b6c6-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```
# <a name="c"></a>[<span data-ttu-id="4b6c6-142">C#</span><span class="sxs-lookup"><span data-stu-id="4b6c6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b6c6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b6c6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b6c6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b6c6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b6c6-145">Java</span><span class="sxs-lookup"><span data-stu-id="4b6c6-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-changescreensharingrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4b6c6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b6c6-146">Response</span></span>
<span data-ttu-id="4b6c6-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b6c6-147">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---roster-updated-with-participant-sending-screen-sharing-video"></a><span data-ttu-id="4b6c6-148">Уведомление о подсписке, обновленный при отправке участником демонстрации экрана общего видео</span><span class="sxs-lookup"><span data-stu-id="4b6c6-148">Notification - roster updated with participant sending screen sharing video</span></span>
<span data-ttu-id="4b6c6-149">Обратите внимание на `direction: sendOnly` свойство в потоке мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4b6c6-149">Note the `direction: sendOnly` property on the media stream.</span></span>

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

