---
title: Создание и отправление уведомления
description: 'Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph. Уведомление хранится в хранилище каналов уведомлений Microsoft Graph и отправляется всем клиентам приложений во всех конечных точках устройств, в которых пользователь вошел в систему.  '
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ''
ms.openlocfilehash: a5ed743e93a5cafcb7ee919acbbcee5f2734a5de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992649"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="ae45f-104">Создание и отправление уведомления</span><span class="sxs-lookup"><span data-stu-id="ae45f-104">Create and send a notification</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae45f-105">Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ae45f-105">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="ae45f-106">Уведомление хранится в хранилище каналов уведомлений Microsoft Graph и отправляется всем клиентам приложений во всех конечных точках устройств, в которых пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="ae45f-106">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="ae45f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae45f-107">Permissions</span></span>
<span data-ttu-id="ae45f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae45f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae45f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae45f-110">Permission type</span></span>      | <span data-ttu-id="ae45f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae45f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae45f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae45f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ae45f-113">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ae45f-113">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ae45f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae45f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae45f-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ae45f-115">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="ae45f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae45f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="ae45f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae45f-117">Request headers</span></span>
|<span data-ttu-id="ae45f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ae45f-118">Name</span></span> | <span data-ttu-id="ae45f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ae45f-119">Type</span></span> | <span data-ttu-id="ae45f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae45f-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="ae45f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae45f-121">Authorization</span></span> | <span data-ttu-id="ae45f-122">string</span><span class="sxs-lookup"><span data-stu-id="ae45f-122">string</span></span> |<span data-ttu-id="ae45f-123">Заголовок Authorization используется для передачи учетных данных вызывающей стороны.</span><span class="sxs-lookup"><span data-stu-id="ae45f-123">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="ae45f-124">Bearer {Token}.</span><span class="sxs-lookup"><span data-stu-id="ae45f-124">Bearer {token}.</span></span> <span data-ttu-id="ae45f-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ae45f-125">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="ae45f-126">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="ae45f-126">Request body</span></span>
<span data-ttu-id="ae45f-127">В тексте запроса добавьте представление объекта [уведомления](../resources/projectrome-notification.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae45f-127">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ae45f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae45f-128">Response</span></span>
<span data-ttu-id="ae45f-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, указывающий, что уведомление было успешно создано и сохранено.</span><span class="sxs-lookup"><span data-stu-id="ae45f-129">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="ae45f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ae45f-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ae45f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae45f-131">Request</span></span>
<span data-ttu-id="ae45f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae45f-132">The following is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2018-08-29T23:51:33.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
        "windows",
        "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "23"
}
```

#### <a name="response"></a><span data-ttu-id="ae45f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae45f-133">Response</span></span>
<span data-ttu-id="ae45f-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ae45f-134">The following is an example of the response.</span></span>

```http
HTTP/1.1 201
Content-Type: application/json
location: https://graph.microsoft.com/beta/me/notifications/518c4fb1-c565-4d67-95c4-bcc3eb8eda1b

{
    "@odata.context": "https://graph.microsoft.com/test872018/$metadata#users('graphNotificationsUser%40contoso.com')/notifications/$entity",
    "appNotificationId": "testDirectToastNotification",
    "displayTimeToLive": 23,
    "expirationDateTime": "2018-08-24T12:31:53.858Z",
    "groupName": "TestGroup",
    "id": "cd5c5e6a-99ce-470a-9982-c47635e73620",
    "priority": "1",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


