---
title: Создание и отправление уведомления
description: Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: c30df0bf19aeab48fab7655fd134dbc1cfe13195
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938164"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="ccccb-103">Создание и отправление уведомления</span><span class="sxs-lookup"><span data-stu-id="ccccb-103">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccccb-104">Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ccccb-104">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="ccccb-105">Уведомление хранится в хранилище каналов уведомлений Microsoft Graph и отправляется всем клиентам приложений во всех конечных точках устройств, в которых пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="ccccb-105">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  

## <a name="permissions"></a><span data-ttu-id="ccccb-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ccccb-106">Permissions</span></span>
<span data-ttu-id="ccccb-107">Служба приложения не требует дополнительных разрешений для отправки уведомлений целевому пользователю.</span><span class="sxs-lookup"><span data-stu-id="ccccb-107">Your application service does not require any additional permissions to post notifications to your targeted user.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="ccccb-108">Если вы решите отправлять уведомления от имени пользователя через делегированные разрешения, то для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="ccccb-108">If you choose to post notifications on behalf of a user via delegated permissions instead, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="ccccb-109">Мы не рекомендуем использовать этот параметр для отправки уведомлений, но если вы хотите узнать больше, в том числе как выбирать разрешения, ознакомьтесь с разделом [разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccccb-109">We don't recommend this option for posting notifications but if you'd like to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccccb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccccb-110">Permission type</span></span>      | <span data-ttu-id="ccccb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccccb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccccb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccccb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ccccb-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ccccb-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ccccb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccccb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccccb-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ccccb-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
| <span data-ttu-id="ccccb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccccb-116">Application</span></span>                           | <span data-ttu-id="ccccb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccccb-117">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="ccccb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccccb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="ccccb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccccb-119">Request headers</span></span>
|<span data-ttu-id="ccccb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ccccb-120">Name</span></span> | <span data-ttu-id="ccccb-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ccccb-121">Type</span></span> | <span data-ttu-id="ccccb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ccccb-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="ccccb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccccb-123">Authorization</span></span> | <span data-ttu-id="ccccb-124">string</span><span class="sxs-lookup"><span data-stu-id="ccccb-124">string</span></span> |<span data-ttu-id="ccccb-125">Заголовок Authorization используется для передачи учетных данных вызывающей стороны.</span><span class="sxs-lookup"><span data-stu-id="ccccb-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="ccccb-126">Bearer {Token}.</span><span class="sxs-lookup"><span data-stu-id="ccccb-126">Bearer {token}.</span></span> <span data-ttu-id="ccccb-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="ccccb-127">Required.</span></span> |
|<span data-ttu-id="ccccb-128">X – УНС — ID</span><span class="sxs-lookup"><span data-stu-id="ccccb-128">X-UNS-ID</span></span> | <span data-ttu-id="ccccb-129">string</span><span class="sxs-lookup"><span data-stu-id="ccccb-129">string</span></span> |<span data-ttu-id="ccccb-130">Усернотификатионсубскриптионид, возвращенный службой уведомлений Microsoft Graph после создания подписки на стороне клиента, и используется для назначения определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ccccb-130">The UserNotificationSubscriptionId that is returned by the Microsoft Graph notification service after creating a subscription on the client-side, and is used to target the specific user.</span></span> <span data-ttu-id="ccccb-131">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ccccb-131">Required.</span></span> |
|<span data-ttu-id="ccccb-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ccccb-132">Content-type</span></span>| <span data-ttu-id="ccccb-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccccb-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccccb-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccccb-135">Request body</span></span>
<span data-ttu-id="ccccb-136">В тексте запроса добавьте представление объекта [уведомления](../resources/projectrome-notification.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccccb-136">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ccccb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccccb-137">Response</span></span>
<span data-ttu-id="ccccb-138">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, указывающий, что уведомление было успешно создано и сохранено.</span><span class="sxs-lookup"><span data-stu-id="ccccb-138">If successful, this method returns a `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> <span data-ttu-id="ccccb-139">В дальнейшем уведомление будет развертывание которого выполняется на все указанные конечные точки с действующей подпиской.</span><span class="sxs-lookup"><span data-stu-id="ccccb-139">The notification will be subsequently fanned-out to all specified endpoints with a valid subscription.</span></span> 

## <a name="example"></a><span data-ttu-id="ccccb-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ccccb-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="ccccb-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccccb-141">Request</span></span>
<span data-ttu-id="ccccb-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccccb-142">The following is an example of a request.</span></span>

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

### <a name="response"></a><span data-ttu-id="ccccb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccccb-143">Response</span></span>
<span data-ttu-id="ccccb-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ccccb-144">The following is an example of the response.</span></span>

> <span data-ttu-id="ccccb-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccccb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
