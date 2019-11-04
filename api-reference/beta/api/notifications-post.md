---
title: Создание и отправление уведомления
description: Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 6062153c1eaff68a19cd5b27ac10efa9bacafb93
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937926"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="a61ee-103">Создание и отправление уведомления</span><span class="sxs-lookup"><span data-stu-id="a61ee-103">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a61ee-104">Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a61ee-104">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="a61ee-105">Уведомление хранится в хранилище каналов уведомлений Microsoft Graph и отправляется всем клиентам приложений во всех конечных точках устройств, в которых пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="a61ee-105">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="a61ee-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a61ee-106">Permissions</span></span>
<span data-ttu-id="a61ee-107">Служба приложения не требует дополнительных разрешений для отправки уведомлений целевому пользователю.</span><span class="sxs-lookup"><span data-stu-id="a61ee-107">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="a61ee-108">Если вы решите отправлять уведомления от имени пользователя через делегированные разрешения, то для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="a61ee-108">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="a61ee-109">Мы не рекомендуем использовать этот параметр для создания уведомлений.</span><span class="sxs-lookup"><span data-stu-id="a61ee-109">We don't recommend this option for creating notifications.</span></span> <span data-ttu-id="a61ee-110">Если вы хотите узнать больше, в том числе как выбирать разрешения, ознакомьтесь с разделом [разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a61ee-110">If you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a61ee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a61ee-111">Permission type</span></span>      | <span data-ttu-id="a61ee-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a61ee-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a61ee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a61ee-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a61ee-114">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a61ee-114">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a61ee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a61ee-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a61ee-116">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a61ee-116">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a61ee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a61ee-117">Application</span></span> | <span data-ttu-id="a61ee-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a61ee-118">Not supported.</span></span>|



## <a name="http-request"></a><span data-ttu-id="a61ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a61ee-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="a61ee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a61ee-120">Request headers</span></span>
|<span data-ttu-id="a61ee-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a61ee-121">Name</span></span> | <span data-ttu-id="a61ee-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a61ee-122">Type</span></span> | <span data-ttu-id="a61ee-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a61ee-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a61ee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a61ee-124">Authorization</span></span> | <span data-ttu-id="a61ee-125">string</span><span class="sxs-lookup"><span data-stu-id="a61ee-125">string</span></span> |<span data-ttu-id="a61ee-126">Заголовок Authorization используется для передачи учетных данных вызывающей стороны.</span><span class="sxs-lookup"><span data-stu-id="a61ee-126">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="a61ee-127">Bearer {Token}.</span><span class="sxs-lookup"><span data-stu-id="a61ee-127">Bearer {token}.</span></span> <span data-ttu-id="a61ee-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="a61ee-128">Required.</span></span> |
|<span data-ttu-id="a61ee-129">X – УНС — ID</span><span class="sxs-lookup"><span data-stu-id="a61ee-129">X-UNS-ID</span></span> | <span data-ttu-id="a61ee-130">string</span><span class="sxs-lookup"><span data-stu-id="a61ee-130">string</span></span> |<span data-ttu-id="a61ee-131">Усернотификатионсубскриптионид, возвращенный службой уведомлений Microsoft Graph после создания подписки, и используется для назначения определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a61ee-131">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription and is used to target the specific user.</span></span> <span data-ttu-id="a61ee-132">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a61ee-132">Required.</span></span> |
|<span data-ttu-id="a61ee-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a61ee-133">Content-type</span></span> | <span data-ttu-id="a61ee-134">апплиатион/JSON.</span><span class="sxs-lookup"><span data-stu-id="a61ee-134">appliation/json.</span></span> <span data-ttu-id="a61ee-135">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="a61ee-135">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a61ee-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a61ee-136">Request body</span></span>
<span data-ttu-id="a61ee-137">В тексте запроса добавьте представление объекта [уведомления](../resources/projectrome-notification.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a61ee-137">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a61ee-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a61ee-138">Response</span></span>
<span data-ttu-id="a61ee-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, указывающий, что уведомление было успешно создано и сохранено.</span><span class="sxs-lookup"><span data-stu-id="a61ee-139">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="a61ee-140">В дальнейшем уведомление будет развертывание которого выполняется на все указанные конечные точки с действующей подпиской.</span><span class="sxs-lookup"><span data-stu-id="a61ee-140">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

## <a name="example"></a><span data-ttu-id="a61ee-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a61ee-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a61ee-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a61ee-142">Request</span></span>
<span data-ttu-id="a61ee-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a61ee-143">The following is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2019-10-30T23:59:00.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
    "windows",
    "ios",
    "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "60"
}
```

### <a name="response"></a><span data-ttu-id="a61ee-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a61ee-144">Response</span></span>
<span data-ttu-id="a61ee-145">Ниже приведен пример соответствующего ответа.</span><span class="sxs-lookup"><span data-stu-id="a61ee-145">The following is an example of the corresponding response.</span></span>

```http
HTTP/1.1 201
client-request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781
content-length: 356
content-type: application/json
location: https://graph.microsoft.com/beta/me/activities/119081f2-f19d-4fa8-817c-7e01092c0f7d
request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('graphnotify%40contoso.com')/notifications/$entity",
    "displayTimeToLive": 59,
    "expirationDateTime": "2019-10-28T22:05:36.25Z",
    "groupName": "TestGroup",
    "id": "119081f2-f19d-4fa8-817c-7e01092c0f7d",
    "priority": "High",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```
