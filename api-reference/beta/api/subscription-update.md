---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 19355ff8acbcdade689b140abca63e8d9885e3fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512782"
---
# <a name="update-subscription"></a><span data-ttu-id="10373-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="10373-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10373-104">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="10373-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="10373-105">Срок действия подписок после продолжительность времени, зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="10373-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="10373-106">Во избежание отсутствует уведомлений, приложение следует обновлять его подписки еще до которых истек срок действия.</span><span class="sxs-lookup"><span data-stu-id="10373-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="10373-107">В разделе [подписки](../resources/subscription.md) для Максимальная длина подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="10373-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="10373-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10373-108">Permissions</span></span>

<span data-ttu-id="10373-p102">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10373-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10373-111">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="10373-111">Resource type / Item</span></span>        | <span data-ttu-id="10373-112">Разрешение</span><span class="sxs-lookup"><span data-stu-id="10373-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="10373-113">Contacts</span><span class="sxs-lookup"><span data-stu-id="10373-113">Contacts</span></span>                    | <span data-ttu-id="10373-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="10373-114">Contacts.Read</span></span>       |
| <span data-ttu-id="10373-115">Беседы</span><span class="sxs-lookup"><span data-stu-id="10373-115">Conversations</span></span>               | <span data-ttu-id="10373-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="10373-116">Group.Read.All</span></span>      |
| <span data-ttu-id="10373-117">События</span><span class="sxs-lookup"><span data-stu-id="10373-117">Events</span></span>                      | <span data-ttu-id="10373-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="10373-118">Calendars.Read</span></span>      |
| <span data-ttu-id="10373-119">Сообщения</span><span class="sxs-lookup"><span data-stu-id="10373-119">Messages</span></span>                    | <span data-ttu-id="10373-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="10373-120">Mail.Read</span></span>           |
| <span data-ttu-id="10373-121">Группы</span><span class="sxs-lookup"><span data-stu-id="10373-121">Groups</span></span>                      | <span data-ttu-id="10373-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="10373-122">Group.Read.All</span></span>      |
| <span data-ttu-id="10373-123">Пользователи</span><span class="sxs-lookup"><span data-stu-id="10373-123">Users</span></span>                       | <span data-ttu-id="10373-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="10373-124">User.Read.All</span></span>       |
| <span data-ttu-id="10373-125">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="10373-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="10373-126">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="10373-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="10373-127">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="10373-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="10373-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10373-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="10373-129">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="10373-129">Security alert</span></span>               | <span data-ttu-id="10373-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10373-130">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="10373-131">***Примечание:*** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="10373-131">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="10373-132">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="10373-132">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="10373-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10373-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="10373-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10373-134">Request headers</span></span>

| <span data-ttu-id="10373-135">Имя</span><span class="sxs-lookup"><span data-stu-id="10373-135">Name</span></span>       | <span data-ttu-id="10373-136">Тип</span><span class="sxs-lookup"><span data-stu-id="10373-136">Type</span></span> | <span data-ttu-id="10373-137">Описание</span><span class="sxs-lookup"><span data-stu-id="10373-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="10373-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="10373-138">Authorization</span></span>  | <span data-ttu-id="10373-139">string</span><span class="sxs-lookup"><span data-stu-id="10373-139">string</span></span>  | <span data-ttu-id="10373-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10373-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="10373-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="10373-142">Response</span></span>

<span data-ttu-id="10373-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10373-143">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10373-144">Пример</span><span class="sxs-lookup"><span data-stu-id="10373-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="10373-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="10373-145">Request</span></span>

<span data-ttu-id="10373-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10373-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="10373-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="10373-147">Response</span></span>

<span data-ttu-id="10373-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10373-148">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
