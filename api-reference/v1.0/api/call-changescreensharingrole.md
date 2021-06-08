---
title: 'вызов: changeScreenSharingRole'
description: Разрешить приложениям обмениваться контентом экрана с участниками группового вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2defaeb01463fbaed957990716d2870844345088
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786056"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="2b4b1-103">вызов: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="2b4b1-103">call: changeScreenSharingRole</span></span>

<span data-ttu-id="2b4b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b4b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b4b1-105">Разрешить приложениям обмениваться контентом экрана с участниками группового вызова.</span><span class="sxs-lookup"><span data-stu-id="2b4b1-105">Allow applications to share screen content with the participants of a group call.</span></span>

> <span data-ttu-id="2b4b1-106">**Примечание:** Это поддерживается только для групповых вызовов, которые используют App-Hosted Media.</span><span class="sxs-lookup"><span data-stu-id="2b4b1-106">**Note:** This is only supported for group calls that use App-Hosted Media.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b4b1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b4b1-107">Permissions</span></span>
<span data-ttu-id="2b4b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b4b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b4b1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b4b1-110">Permission type</span></span>                        | <span data-ttu-id="2b4b1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b4b1-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2b4b1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b4b1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b4b1-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b4b1-113">Not Supported</span></span>                               |
| <span data-ttu-id="2b4b1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b4b1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b4b1-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b4b1-115">Not Supported</span></span>                               |
| <span data-ttu-id="2b4b1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b4b1-116">Application</span></span>                            | <span data-ttu-id="2b4b1-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="2b4b1-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="2b4b1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b4b1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="2b4b1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b4b1-119">Request headers</span></span>
| <span data-ttu-id="2b4b1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2b4b1-120">Name</span></span>          | <span data-ttu-id="2b4b1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2b4b1-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2b4b1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b4b1-122">Authorization</span></span> | <span data-ttu-id="2b4b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b4b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b4b1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b4b1-125">Content-type</span></span>  | <span data-ttu-id="2b4b1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b4b1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b4b1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b4b1-128">Request body</span></span>
<span data-ttu-id="2b4b1-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2b4b1-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2b4b1-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="2b4b1-130">Parameter</span></span>      | <span data-ttu-id="2b4b1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b4b1-131">Type</span></span>    |<span data-ttu-id="2b4b1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b4b1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b4b1-133">role</span><span class="sxs-lookup"><span data-stu-id="2b4b1-133">role</span></span>|<span data-ttu-id="2b4b1-134">String</span><span class="sxs-lookup"><span data-stu-id="2b4b1-134">String</span></span>|<span data-ttu-id="2b4b1-135">Возможные значения: "зритель", "sharer"</span><span class="sxs-lookup"><span data-stu-id="2b4b1-135">Possible values are: 'viewer', 'sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="2b4b1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b4b1-136">Response</span></span>
<span data-ttu-id="2b4b1-137">В случае успешной работы этот метод возвращает код ответа, и все участники `202 Accepted` получат обновление реестра.</span><span class="sxs-lookup"><span data-stu-id="2b4b1-137">If successful, this method returns a `202 Accepted` response code, and all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="2b4b1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2b4b1-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2b4b1-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b4b1-139">Request</span></span>
<span data-ttu-id="2b4b1-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b4b1-140">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b4b1-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b4b1-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2b4b1-142">C#</span><span class="sxs-lookup"><span data-stu-id="2b4b1-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b4b1-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b4b1-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b4b1-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b4b1-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b4b1-145">Java</span><span class="sxs-lookup"><span data-stu-id="2b4b1-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-changescreensharingrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2b4b1-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b4b1-146">Response</span></span>
<span data-ttu-id="2b4b1-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b4b1-147">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---roster-updated-with-participant-sending-screen-sharing-video"></a><span data-ttu-id="2b4b1-148">Уведомление — список обновляется с помощью видео отправки участниками совместного доступа к экранам</span><span class="sxs-lookup"><span data-stu-id="2b4b1-148">Notification - roster updated with participant sending screen sharing video</span></span>
<span data-ttu-id="2b4b1-149">Обратите внимание `direction: sendOnly` на свойство в потоке мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="2b4b1-149">Note the `direction: sendOnly` property on the media stream.</span></span>

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

