---
title: Создание и отправление уведомления
description: Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 1828f72bfcedb701597ce4b0d55e274a25fcf834
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456686"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="1923a-103">Создание и отправление уведомления</span><span class="sxs-lookup"><span data-stu-id="1923a-103">Create and send a notification</span></span>

<span data-ttu-id="1923a-104">Пространство имен: Microsoft. Graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="1923a-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="1923a-105">Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1923a-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="1923a-106">Уведомление хранится в хранилище каналов уведомлений Microsoft Graph и отправляется всем клиентам приложений во всех конечных точках устройств, в которых пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="1923a-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="1923a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1923a-107">Permissions</span></span>
<span data-ttu-id="1923a-108">Служба приложения не требует дополнительных разрешений для отправки уведомлений целевому пользователю.</span><span class="sxs-lookup"><span data-stu-id="1923a-108">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="1923a-109">Если вы решите отправлять уведомления от имени пользователя через делегированные разрешения, то для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="1923a-109">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="1923a-110">Мы не рекомендуем использовать этот параметр для создания уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1923a-110">We don't recommend this option for creating notifications.</span></span> <span data-ttu-id="1923a-111">Если вы хотите узнать больше, в том числе как выбирать разрешения, ознакомьтесь с разделом [разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1923a-111">If you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1923a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1923a-112">Permission type</span></span>      | <span data-ttu-id="1923a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1923a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1923a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1923a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1923a-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1923a-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1923a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1923a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1923a-117">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1923a-117">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1923a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1923a-118">Application</span></span> | <span data-ttu-id="1923a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1923a-119">Not supported.</span></span>|



## <a name="http-request"></a><span data-ttu-id="1923a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1923a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="1923a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1923a-121">Request headers</span></span>
|<span data-ttu-id="1923a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1923a-122">Name</span></span> | <span data-ttu-id="1923a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1923a-123">Description</span></span>|
|:----|:-----------|
|<span data-ttu-id="1923a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1923a-124">Authorization</span></span> | <span data-ttu-id="1923a-125">Заголовок Authorization используется для передачи учетных данных вызывающей стороны.</span><span class="sxs-lookup"><span data-stu-id="1923a-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="1923a-126">Bearer {Token}.</span><span class="sxs-lookup"><span data-stu-id="1923a-126">Bearer {token}.</span></span> <span data-ttu-id="1923a-127">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="1923a-127">Required.</span></span> |
|<span data-ttu-id="1923a-128">X – УНС — ID</span><span class="sxs-lookup"><span data-stu-id="1923a-128">X-UNS-ID</span></span> | <span data-ttu-id="1923a-129">Усернотификатионсубскриптионид, возвращенный службой уведомлений Microsoft Graph после создания подписки, и используется для назначения определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1923a-129">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription and is used to target the specific user.</span></span> <span data-ttu-id="1923a-130">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1923a-130">Required.</span></span> |
|<span data-ttu-id="1923a-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1923a-131">Content-type</span></span> | <span data-ttu-id="1923a-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1923a-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1923a-134">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="1923a-134">Request body</span></span>
<span data-ttu-id="1923a-135">В тексте запроса добавьте представление объекта [уведомления](../resources/projectrome-notification.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1923a-135">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1923a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1923a-136">Response</span></span>
<span data-ttu-id="1923a-137">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, указывающий, что уведомление было успешно создано и сохранено.</span><span class="sxs-lookup"><span data-stu-id="1923a-137">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="1923a-138">В дальнейшем уведомление будет развертывание которого выполняется на все указанные конечные точки с действующей подпиской.</span><span class="sxs-lookup"><span data-stu-id="1923a-138">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

<span data-ttu-id="1923a-139">В следующей таблице перечислены возможные коды ошибок и ответов, которые могут быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="1923a-139">The following table lists the possible error and response codes that can be returned.</span></span>

|<span data-ttu-id="1923a-140">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="1923a-140">Error code</span></span>             | <span data-ttu-id="1923a-141">дескритион</span><span class="sxs-lookup"><span data-stu-id="1923a-141">Descrition</span></span>                             |
|:-----------------------------------|:----------------------------------------------------------|
|<span data-ttu-id="1923a-142">HttpStatusCode. Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="1923a-142">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="1923a-143">Body является массивом (несколько уведомлений не поддерживаются).</span><span class="sxs-lookup"><span data-stu-id="1923a-143">Body is an array (multiple notifications is not supported).</span></span>|
|<span data-ttu-id="1923a-144">HttpStatusCode. Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="1923a-144">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="1923a-145">Текст не отвечает контракту для API.</span><span class="sxs-lookup"><span data-stu-id="1923a-145">Body doesn't match the contract for the API.</span></span>               |
|<span data-ttu-id="1923a-146">HttpStatusCode. запрещено</span><span class="sxs-lookup"><span data-stu-id="1923a-146">HttpStatusCode.Forbidden</span></span>            | <span data-ttu-id="1923a-147">Абонент находится в списке заблокированных.</span><span class="sxs-lookup"><span data-stu-id="1923a-147">Caller is on the blocked list.</span></span>                          |
|<span data-ttu-id="1923a-148">HttpStatusCode. Месодноталловед</span><span class="sxs-lookup"><span data-stu-id="1923a-148">HttpStatusCode.MethodNotAllowed</span></span>     | <span data-ttu-id="1923a-149">Используемый метод HTTP не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1923a-149">The HTTP method used is not supported.</span></span>                     |
|<span data-ttu-id="1923a-150">HttpStatusCode. Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="1923a-150">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="1923a-151">В запросе присутствуют Неподдерживаемые заголовки.</span><span class="sxs-lookup"><span data-stu-id="1923a-151">Unsupported headers are present in the request.</span></span> <span data-ttu-id="1923a-152">Два заголовка не поддерживаются:</span><span class="sxs-lookup"><span data-stu-id="1923a-152">Two headers are not supported:</span></span><br/><br/><span data-ttu-id="1923a-153">If — Modified — с</span><span class="sxs-lookup"><span data-stu-id="1923a-153">If-Modified-Since</span></span><br/><span data-ttu-id="1923a-154">Если — Range</span><span class="sxs-lookup"><span data-stu-id="1923a-154">If-Range</span></span> |                    
|<span data-ttu-id="1923a-155">HttpStatusCode. Унсуппортедмедиатипе</span><span class="sxs-lookup"><span data-stu-id="1923a-155">HttpStatusCode.UnsupportedMediaType</span></span> | <span data-ttu-id="1923a-156">Заголовок Content-Encoding присутствует и имеет значения алгоритма сжатия, отличные от `Deflate` or `Gzip`.</span><span class="sxs-lookup"><span data-stu-id="1923a-156">The header Content-Encoding is present and has compression algorithm values other than `Deflate` or `Gzip`.</span></span>  |
|<span data-ttu-id="1923a-157">HttpStatusCode. Бадрекуест</span><span class="sxs-lookup"><span data-stu-id="1923a-157">HttpStatusCode.BadRequest</span></span>           | <span data-ttu-id="1923a-158">Недопустимые полезные данные.</span><span class="sxs-lookup"><span data-stu-id="1923a-158">Invalid payload.</span></span>                                           |
|<span data-ttu-id="1923a-159">HttpStatusCode. запрещено</span><span class="sxs-lookup"><span data-stu-id="1923a-159">HttpStatusCode.Forbidden</span></span>            | <span data-ttu-id="1923a-160">Абонент не имеет прав на действия от имени пользователя или отправлять уведомление пользователю.</span><span class="sxs-lookup"><span data-stu-id="1923a-160">Caller is not authorized to act on behalf of the user or send notification to the user.</span></span>                         |
|<span data-ttu-id="1923a-161">HttpStatusCode. несанкционированный</span><span class="sxs-lookup"><span data-stu-id="1923a-161">HttpStatusCode.Unauthorized</span></span>         |  <span data-ttu-id="1923a-162">Текст запроса содержит недопустимые типы данных о действиях.</span><span class="sxs-lookup"><span data-stu-id="1923a-162">Request body contains invalid activity data types.</span></span>        |
|<span data-ttu-id="1923a-163">HttpStatusCode. ОК</span><span class="sxs-lookup"><span data-stu-id="1923a-163">HttpStatusCode.OK</span></span>                   |  <span data-ttu-id="1923a-164">Действие успешно создано.</span><span class="sxs-lookup"><span data-stu-id="1923a-164">Activity successfully created.</span></span>                            |
|<span data-ttu-id="1923a-165">HttpStatusCode. Нотакцептабле</span><span class="sxs-lookup"><span data-stu-id="1923a-165">HttpStatusCode.NotAcceptable</span></span>        |  <span data-ttu-id="1923a-166">Запрос был отрегулирован или сервер занят.</span><span class="sxs-lookup"><span data-stu-id="1923a-166">Request has been throttled or the server is busy.</span></span>    |


## <a name="example"></a><span data-ttu-id="1923a-167">Пример</span><span class="sxs-lookup"><span data-stu-id="1923a-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="1923a-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="1923a-168">Request</span></span>
<span data-ttu-id="1923a-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1923a-169">The following is an example of a request.</span></span>

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

### <a name="response"></a><span data-ttu-id="1923a-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="1923a-170">Response</span></span>
<span data-ttu-id="1923a-171">Ниже приведен пример соответствующего ответа.</span><span class="sxs-lookup"><span data-stu-id="1923a-171">The following is an example of the corresponding response.</span></span>

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

