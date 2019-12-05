---
title: Создание и отправление уведомления
description: Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 6aa436a7c2283cad0eba7b1840e120a38ccf2632
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844199"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="a5447-103">Создание и отправление уведомления</span><span class="sxs-lookup"><span data-stu-id="a5447-103">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5447-104">Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a5447-104">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="a5447-105">Уведомление хранится в хранилище каналов уведомлений Microsoft Graph и отправляется всем клиентам приложений во всех конечных точках устройств, в которых пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="a5447-105">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="a5447-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5447-106">Permissions</span></span>
<span data-ttu-id="a5447-107">Служба приложения не требует дополнительных разрешений для отправки уведомлений целевому пользователю.</span><span class="sxs-lookup"><span data-stu-id="a5447-107">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="a5447-108">Если вы решите отправлять уведомления от имени пользователя через делегированные разрешения, то для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="a5447-108">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="a5447-109">Мы не рекомендуем использовать этот параметр для создания уведомлений.</span><span class="sxs-lookup"><span data-stu-id="a5447-109">We don't recommend this option for creating notifications.</span></span> <span data-ttu-id="a5447-110">Если вы хотите узнать больше, в том числе как выбирать разрешения, ознакомьтесь с разделом [разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5447-110">If you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5447-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5447-111">Permission type</span></span>      | <span data-ttu-id="a5447-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5447-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5447-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5447-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a5447-114">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a5447-114">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a5447-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5447-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5447-116">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a5447-116">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a5447-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5447-117">Application</span></span> | <span data-ttu-id="a5447-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5447-118">Not supported.</span></span>|



## <a name="http-request"></a><span data-ttu-id="a5447-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5447-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="a5447-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5447-120">Request headers</span></span>
|<span data-ttu-id="a5447-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a5447-121">Name</span></span> | <span data-ttu-id="a5447-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a5447-122">Description</span></span>|
|:----|:-----------|
|<span data-ttu-id="a5447-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5447-123">Authorization</span></span> | <span data-ttu-id="a5447-124">Заголовок Authorization используется для передачи учетных данных вызывающей стороны.</span><span class="sxs-lookup"><span data-stu-id="a5447-124">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="a5447-125">Bearer {Token}.</span><span class="sxs-lookup"><span data-stu-id="a5447-125">Bearer {token}.</span></span> <span data-ttu-id="a5447-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a5447-126">Required.</span></span> |
|<span data-ttu-id="a5447-127">X – УНС — ID</span><span class="sxs-lookup"><span data-stu-id="a5447-127">X-UNS-ID</span></span> | <span data-ttu-id="a5447-128">Усернотификатионсубскриптионид, возвращенный службой уведомлений Microsoft Graph после создания подписки, и используется для назначения определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5447-128">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription and is used to target the specific user.</span></span> <span data-ttu-id="a5447-129">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a5447-129">Required.</span></span> |
|<span data-ttu-id="a5447-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5447-130">Content-type</span></span> | <span data-ttu-id="a5447-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5447-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5447-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5447-133">Request body</span></span>
<span data-ttu-id="a5447-134">В тексте запроса добавьте представление объекта [уведомления](../resources/projectrome-notification.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5447-134">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a5447-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5447-135">Response</span></span>
<span data-ttu-id="a5447-136">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, указывающий, что уведомление было успешно создано и сохранено.</span><span class="sxs-lookup"><span data-stu-id="a5447-136">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="a5447-137">В дальнейшем уведомление будет развертывание которого выполняется на все указанные конечные точки с действующей подпиской.</span><span class="sxs-lookup"><span data-stu-id="a5447-137">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

<span data-ttu-id="a5447-138">В следующей таблице перечислены возможные коды ошибок и ответов, которые могут быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="a5447-138">The following table lists the possible error and response codes that can be returned.</span></span>

|<span data-ttu-id="a5447-139">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="a5447-139">Error code</span></span>             | <span data-ttu-id="a5447-140">дескритион</span><span class="sxs-lookup"><span data-stu-id="a5447-140">Descrition</span></span>                             |
|:-----------------------------------|:----------------------------------------------------------|
|<span data-ttu-id="a5447-141">HttpStatusCode. Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="a5447-141">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="a5447-142">Body является массивом (несколько уведомлений не поддерживаются).</span><span class="sxs-lookup"><span data-stu-id="a5447-142">Body is an array (multiple notifications is not supported).</span></span>|
|<span data-ttu-id="a5447-143">HttpStatusCode. Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="a5447-143">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="a5447-144">Текст не отвечает контракту для API.</span><span class="sxs-lookup"><span data-stu-id="a5447-144">Body doesn't match the contract for the API.</span></span>               |
|<span data-ttu-id="a5447-145">HttpStatusCode. запрещено</span><span class="sxs-lookup"><span data-stu-id="a5447-145">HttpStatusCode.Forbidden</span></span>            | <span data-ttu-id="a5447-146">Абонент находится в списке заблокированных.</span><span class="sxs-lookup"><span data-stu-id="a5447-146">Caller is on the blocked list.</span></span>                          |
|<span data-ttu-id="a5447-147">HttpStatusCode. Месодноталловед</span><span class="sxs-lookup"><span data-stu-id="a5447-147">HttpStatusCode.MethodNotAllowed</span></span>     | <span data-ttu-id="a5447-148">Используемый метод HTTP не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5447-148">The HTTP method used is not supported.</span></span>                     |
|<span data-ttu-id="a5447-149">HttpStatusCode. Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="a5447-149">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="a5447-150">В запросе присутствуют Неподдерживаемые заголовки.</span><span class="sxs-lookup"><span data-stu-id="a5447-150">Unsupported headers are present in the request.</span></span> <span data-ttu-id="a5447-151">Два заголовка не поддерживаются:</span><span class="sxs-lookup"><span data-stu-id="a5447-151">Two headers are not supported:</span></span><br/><br/><span data-ttu-id="a5447-152">If — Modified — с</span><span class="sxs-lookup"><span data-stu-id="a5447-152">If-Modified-Since</span></span><br/><span data-ttu-id="a5447-153">Если — Range</span><span class="sxs-lookup"><span data-stu-id="a5447-153">If-Range</span></span> |                    
|<span data-ttu-id="a5447-154">HttpStatusCode. Унсуппортедмедиатипе</span><span class="sxs-lookup"><span data-stu-id="a5447-154">HttpStatusCode.UnsupportedMediaType</span></span> | <span data-ttu-id="a5447-155">Заголовок Content-Encoding присутствует и имеет значения алгоритма сжатия, отличные от `Deflate` or `Gzip`.</span><span class="sxs-lookup"><span data-stu-id="a5447-155">The header Content-Encoding is present and has compression algorithm values other than `Deflate` or `Gzip`.</span></span>  |
|<span data-ttu-id="a5447-156">HttpStatusCode. Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="a5447-156">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="a5447-157">Недопустимые полезные данные.</span><span class="sxs-lookup"><span data-stu-id="a5447-157">Invalid payload.</span></span>                                           |
|<span data-ttu-id="a5447-158">HttpStatusCode. запрещено</span><span class="sxs-lookup"><span data-stu-id="a5447-158">HttpStatusCode.Forbidden</span></span>            | <span data-ttu-id="a5447-159">Абонент не имеет прав на действия от имени пользователя или отправлять уведомление пользователю.</span><span class="sxs-lookup"><span data-stu-id="a5447-159">Caller is not authorized to act on behalf of the user or send notification to the user.</span></span>                         |
|<span data-ttu-id="a5447-160">HttpStatusCode. несанкционированный</span><span class="sxs-lookup"><span data-stu-id="a5447-160">HttpStatusCode.Unauthorized</span></span>         |  <span data-ttu-id="a5447-161">Текст запроса содержит недопустимые типы данных о действиях.</span><span class="sxs-lookup"><span data-stu-id="a5447-161">Request body contains invalid activity data types.</span></span>        |
|<span data-ttu-id="a5447-162">HttpStatusCode. ОК</span><span class="sxs-lookup"><span data-stu-id="a5447-162">HttpStatusCode.OK</span></span>                   |  <span data-ttu-id="a5447-163">Действие успешно создано.</span><span class="sxs-lookup"><span data-stu-id="a5447-163">Activity successfully created.</span></span>                            |
|<span data-ttu-id="a5447-164">HttpStatusCode. Нотакцептабле</span><span class="sxs-lookup"><span data-stu-id="a5447-164">HttpStatusCode.NotAcceptable</span></span>        |  <span data-ttu-id="a5447-165">Запрос был отрегулирован или сервер занят.</span><span class="sxs-lookup"><span data-stu-id="a5447-165">Request has been throttled or the server is busy.</span></span>    |


## <a name="example"></a><span data-ttu-id="a5447-166">Пример</span><span class="sxs-lookup"><span data-stu-id="a5447-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5447-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5447-167">Request</span></span>
<span data-ttu-id="a5447-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5447-168">The following is an example of a request.</span></span>

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

### <a name="response"></a><span data-ttu-id="a5447-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5447-169">Response</span></span>
<span data-ttu-id="a5447-170">Ниже приведен пример соответствующего ответа.</span><span class="sxs-lookup"><span data-stu-id="a5447-170">The following is an example of the corresponding response.</span></span>

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

