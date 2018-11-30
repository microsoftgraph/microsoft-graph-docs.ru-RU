---
title: Создание и отправка уведомления
description: 'Создание и отправка уведомления, предназначенные для пользователей через Microsoft Graph. Уведомление, сохраненных в Microsoft Graph уведомление, веб-канала хранилища и отправляется всем клиентам приложения на всех конечных точках устройства, которые пользователь входит в систему.  '
ms.openlocfilehash: 7855d8b369a2efc6dada33c66c12ae76384a2760
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080168"
---
# <a name="create-and-send-a-notification"></a><span data-ttu-id="bcb66-104">Создание и отправка уведомления</span><span class="sxs-lookup"><span data-stu-id="bcb66-104">Create and send a notification</span></span>
> <span data-ttu-id="bcb66-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bcb66-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcb66-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcb66-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bcb66-107">Создание и отправка уведомления, предназначенные для пользователей через Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bcb66-107">Create and send a notification targeting a user through Microsoft Graph.</span></span> <span data-ttu-id="bcb66-108">Уведомление, сохраненных в Microsoft Graph уведомление, веб-канала хранилища и отправляется всем клиентам приложения на всех конечных точках устройства, которые пользователь входит в систему.</span><span class="sxs-lookup"><span data-stu-id="bcb66-108">The notification is stored in the Microsoft Graph notification feed store, and is sent to all app clients on all device endpoints that the user is signed in to.</span></span>  
## <a name="permissions"></a><span data-ttu-id="bcb66-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcb66-109">Permissions</span></span>
<span data-ttu-id="bcb66-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcb66-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcb66-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcb66-112">Permission type</span></span>      | <span data-ttu-id="bcb66-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcb66-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcb66-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcb66-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bcb66-115">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="bcb66-115">Notifications.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="bcb66-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcb66-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcb66-117">Notifications.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="bcb66-117">Notifications.ReadWrite.CreatedByApp</span></span>    |

## <a name="http-request"></a><span data-ttu-id="bcb66-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcb66-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a><span data-ttu-id="bcb66-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcb66-119">Request headers</span></span>
|<span data-ttu-id="bcb66-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bcb66-120">Name</span></span> | <span data-ttu-id="bcb66-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bcb66-121">Type</span></span> | <span data-ttu-id="bcb66-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bcb66-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="bcb66-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcb66-123">Authorization</span></span> | <span data-ttu-id="bcb66-124">string</span><span class="sxs-lookup"><span data-stu-id="bcb66-124">string</span></span> |<span data-ttu-id="bcb66-125">Заголовок authorization используется для передачи учетных данных вызывающей стороны.</span><span class="sxs-lookup"><span data-stu-id="bcb66-125">The authorization header is used to pass the credentials of the calling party.</span></span> <span data-ttu-id="bcb66-126">Носителя {маркер}.</span><span class="sxs-lookup"><span data-stu-id="bcb66-126">Bearer {token}.</span></span> <span data-ttu-id="bcb66-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="bcb66-127">Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="bcb66-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcb66-128">Request body</span></span>
<span data-ttu-id="bcb66-129">В тексте запроса укажите представление JSON объекта [уведомлений](../resources/projectrome-notification.md) .</span><span class="sxs-lookup"><span data-stu-id="bcb66-129">In the request body, supply a JSON representation of a [notification](../resources/projectrome-notification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bcb66-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcb66-130">Response</span></span>
<span data-ttu-id="bcb66-131">Успешно завершена, этот метод возвращает `201 Created` код ответа, которое указывает, что уведомления было успешно создаются и сохраняются.</span><span class="sxs-lookup"><span data-stu-id="bcb66-131">If successful, this method returns the `201 Created` response code that indicates that the notification was successfully created and stored.</span></span> 
## <a name="example"></a><span data-ttu-id="bcb66-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bcb66-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bcb66-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcb66-133">Request</span></span>
<span data-ttu-id="bcb66-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcb66-134">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="bcb66-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcb66-135">Response</span></span>
<span data-ttu-id="bcb66-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bcb66-136">The following is an example of the response.</span></span>

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


