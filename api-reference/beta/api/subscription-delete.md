---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9ca4c772cb6d7de088550a16262275b4c43fb9c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509464"
---
# <a name="delete-subscription"></a><span data-ttu-id="8d63f-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="8d63f-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d63f-104">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="8d63f-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d63f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d63f-105">Permissions</span></span>

<span data-ttu-id="8d63f-p101">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d63f-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d63f-108">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="8d63f-108">Resource type / Item</span></span>        | <span data-ttu-id="8d63f-109">Разрешение</span><span class="sxs-lookup"><span data-stu-id="8d63f-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="8d63f-110">Contacts</span><span class="sxs-lookup"><span data-stu-id="8d63f-110">Contacts</span></span>                    | <span data-ttu-id="8d63f-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8d63f-111">Contacts.Read</span></span>       |
| <span data-ttu-id="8d63f-112">Беседы</span><span class="sxs-lookup"><span data-stu-id="8d63f-112">Conversations</span></span>               | <span data-ttu-id="8d63f-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d63f-113">Group.Read.All</span></span>      |
| <span data-ttu-id="8d63f-114">События</span><span class="sxs-lookup"><span data-stu-id="8d63f-114">Events</span></span>                      | <span data-ttu-id="8d63f-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8d63f-115">Calendars.Read</span></span>      |
| <span data-ttu-id="8d63f-116">Сообщения</span><span class="sxs-lookup"><span data-stu-id="8d63f-116">Messages</span></span>                    | <span data-ttu-id="8d63f-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8d63f-117">Mail.Read</span></span>           |
| <span data-ttu-id="8d63f-118">Группы</span><span class="sxs-lookup"><span data-stu-id="8d63f-118">Groups</span></span>                      | <span data-ttu-id="8d63f-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d63f-119">Group.Read.All</span></span>      |
| <span data-ttu-id="8d63f-120">Пользователи</span><span class="sxs-lookup"><span data-stu-id="8d63f-120">Users</span></span>                       | <span data-ttu-id="8d63f-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d63f-121">User.Read.All</span></span>       |
| <span data-ttu-id="8d63f-122">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="8d63f-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="8d63f-123">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="8d63f-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="8d63f-124">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="8d63f-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="8d63f-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d63f-125">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="8d63f-126">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="8d63f-126">Security alert</span></span>              | <span data-ttu-id="8d63f-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d63f-127">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="8d63f-128">***Примечание:*** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8d63f-128">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="8d63f-129">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8d63f-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="8d63f-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d63f-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8d63f-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d63f-131">Request headers</span></span>

| <span data-ttu-id="8d63f-132">Имя</span><span class="sxs-lookup"><span data-stu-id="8d63f-132">Name</span></span>       | <span data-ttu-id="8d63f-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8d63f-133">Type</span></span> | <span data-ttu-id="8d63f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8d63f-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8d63f-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d63f-135">Authorization</span></span>  | <span data-ttu-id="8d63f-136">string</span><span class="sxs-lookup"><span data-stu-id="8d63f-136">string</span></span>  | <span data-ttu-id="8d63f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d63f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d63f-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d63f-139">Request body</span></span>

<span data-ttu-id="8d63f-140">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d63f-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d63f-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d63f-141">Response</span></span>

<span data-ttu-id="8d63f-142">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8d63f-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8d63f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="8d63f-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8d63f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d63f-144">Request</span></span>

<span data-ttu-id="8d63f-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d63f-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="8d63f-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d63f-146">Response</span></span>

<span data-ttu-id="8d63f-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8d63f-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
