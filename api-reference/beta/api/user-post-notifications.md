---
title: Создание и отправление уведомления
description: Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 8eb35ea0ade2e7d471674d8d064ba0ac38b361cc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996270"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="26dfb-103">Создание и отправление уведомления</span><span class="sxs-lookup"><span data-stu-id="26dfb-103">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26dfb-104">Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="26dfb-104">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="26dfb-105">Уведомление хранится в хранилище каналов уведомлений Microsoft Graph и отправляется всем клиентам приложений во всех конечных точках устройств, в которых пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="26dfb-105">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="26dfb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26dfb-106">Permissions</span></span>
<span data-ttu-id="26dfb-107">Служба приложения не требует дополнительных разрешений для отправки уведомлений целевому пользователю.</span><span class="sxs-lookup"><span data-stu-id="26dfb-107">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="26dfb-108">Если вы решите отправлять уведомления от имени пользователя через делегированные разрешения, то для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="26dfb-108">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="26dfb-109">Мы не рекомендуем использовать этот параметр для отправки уведомлений, но если вы хотите узнать больше, в том числе как выбирать разрешения, ознакомьтесь с разделом [разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26dfb-109">We don't recommend this option for posting notifications but if you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26dfb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26dfb-110">Permission type</span></span>      | <span data-ttu-id="26dfb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26dfb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26dfb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26dfb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="26dfb-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="26dfb-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="26dfb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26dfb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26dfb-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="26dfb-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
| <span data-ttu-id="26dfb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26dfb-116">Application</span></span>                           | <span data-ttu-id="26dfb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26dfb-117">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="26dfb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26dfb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="26dfb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26dfb-119">Request headers</span></span>
|<span data-ttu-id="26dfb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="26dfb-120">Name</span></span> | <span data-ttu-id="26dfb-121">Тип</span><span class="sxs-lookup"><span data-stu-id="26dfb-121">Type</span></span> | <span data-ttu-id="26dfb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="26dfb-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="26dfb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26dfb-123">Authorization</span></span> | <span data-ttu-id="26dfb-124">string</span><span class="sxs-lookup"><span data-stu-id="26dfb-124">string</span></span> |<span data-ttu-id="26dfb-125">Заголовок Authorization используется для передачи учетных данных вызывающей стороны.</span><span class="sxs-lookup"><span data-stu-id="26dfb-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="26dfb-126">Bearer {Token}.</span><span class="sxs-lookup"><span data-stu-id="26dfb-126">Bearer {token}.</span></span> <span data-ttu-id="26dfb-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="26dfb-127">Required.</span></span> |
|<span data-ttu-id="26dfb-128">X – УНС — ID</span><span class="sxs-lookup"><span data-stu-id="26dfb-128">X-UNS-ID</span></span> | <span data-ttu-id="26dfb-129">string</span><span class="sxs-lookup"><span data-stu-id="26dfb-129">string</span></span> |<span data-ttu-id="26dfb-130">Усернотификатионсубскриптионид, возвращенный службой уведомлений Microsoft Graph после создания подписки на стороне клиента, и используется для назначения определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="26dfb-130">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription on the client-side, and is used to target the specific user.</span></span> <span data-ttu-id="26dfb-131">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="26dfb-131">Required.</span></span> |
|<span data-ttu-id="26dfb-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26dfb-132">Content-type</span></span>| <span data-ttu-id="26dfb-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26dfb-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26dfb-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26dfb-135">Request body</span></span>
<span data-ttu-id="26dfb-136">В тексте запроса добавьте представление объекта [уведомления](../resources/projectrome-notification.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26dfb-136">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="26dfb-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="26dfb-137">Response</span></span>
<span data-ttu-id="26dfb-138">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, указывающий, что уведомление было успешно создано и сохранено.</span><span class="sxs-lookup"><span data-stu-id="26dfb-138">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="26dfb-139">В дальнейшем уведомление будет развертывание которого выполняется на все указанные конечные точки с действующей подпиской.</span><span class="sxs-lookup"><span data-stu-id="26dfb-139">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

## <a name="example"></a><span data-ttu-id="26dfb-140">Пример</span><span class="sxs-lookup"><span data-stu-id="26dfb-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="26dfb-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="26dfb-141">Request</span></span>
<span data-ttu-id="26dfb-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26dfb-142">The following is an example of a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="26dfb-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="26dfb-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notification_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/me/notifications
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "appNotificationId": "appNotificationID-value",
    "expirationDateTime": "datetime-value",
    "targetPolicy": {
      "platformTypes": [
        "platformTypes-value"
        ]
      }, 
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26dfb-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26dfb-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notification-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26dfb-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="26dfb-145">Response</span></span>
<span data-ttu-id="26dfb-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26dfb-146">The following is an example of the response.</span></span>

> <span data-ttu-id="26dfb-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26dfb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notification"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "expirationDateTime": "datetime-value",
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
