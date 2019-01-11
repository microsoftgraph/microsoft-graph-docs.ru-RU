---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
ms.openlocfilehash: a5bd1998df3a7e3a8896fa770c0dbdd72cd59940
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805595"
---
# <a name="delete-subscription"></a><span data-ttu-id="8f5fc-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="8f5fc-103">Delete subscription</span></span>

<span data-ttu-id="8f5fc-104">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="8f5fc-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f5fc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f5fc-105">Permissions</span></span>

<span data-ttu-id="8f5fc-p101">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f5fc-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f5fc-108">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="8f5fc-108">Resource type / Item</span></span>        | <span data-ttu-id="8f5fc-109">Разрешение</span><span class="sxs-lookup"><span data-stu-id="8f5fc-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="8f5fc-110">Contacts</span><span class="sxs-lookup"><span data-stu-id="8f5fc-110">Contacts</span></span>                    | <span data-ttu-id="8f5fc-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8f5fc-111">Contacts.Read</span></span>       |
| <span data-ttu-id="8f5fc-112">Беседы</span><span class="sxs-lookup"><span data-stu-id="8f5fc-112">Conversations</span></span>               | <span data-ttu-id="8f5fc-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f5fc-113">Group.Read.All</span></span>      |
| <span data-ttu-id="8f5fc-114">События</span><span class="sxs-lookup"><span data-stu-id="8f5fc-114">Events</span></span>                      | <span data-ttu-id="8f5fc-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f5fc-115">Calendars.Read</span></span>      |
| <span data-ttu-id="8f5fc-116">Сообщения</span><span class="sxs-lookup"><span data-stu-id="8f5fc-116">Messages</span></span>                    | <span data-ttu-id="8f5fc-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8f5fc-117">Mail.Read</span></span>           |
| <span data-ttu-id="8f5fc-118">Группы</span><span class="sxs-lookup"><span data-stu-id="8f5fc-118">Groups</span></span>                      | <span data-ttu-id="8f5fc-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f5fc-119">Group.Read.All</span></span>      |
| <span data-ttu-id="8f5fc-120">Пользователи</span><span class="sxs-lookup"><span data-stu-id="8f5fc-120">Users</span></span>                       | <span data-ttu-id="8f5fc-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f5fc-121">User.Read.All</span></span>       |
| <span data-ttu-id="8f5fc-122">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="8f5fc-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="8f5fc-123">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="8f5fc-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="8f5fc-124">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="8f5fc-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="8f5fc-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f5fc-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="8f5fc-126">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="8f5fc-126">Security alert</span></span>| <span data-ttu-id="8f5fc-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f5fc-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f5fc-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f5fc-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8f5fc-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f5fc-129">Request headers</span></span>

| <span data-ttu-id="8f5fc-130">Имя</span><span class="sxs-lookup"><span data-stu-id="8f5fc-130">Name</span></span>       | <span data-ttu-id="8f5fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f5fc-131">Type</span></span> | <span data-ttu-id="8f5fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f5fc-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8f5fc-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f5fc-133">Authorization</span></span>  | <span data-ttu-id="8f5fc-134">string</span><span class="sxs-lookup"><span data-stu-id="8f5fc-134">string</span></span>  | <span data-ttu-id="8f5fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f5fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f5fc-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f5fc-137">Request body</span></span>

<span data-ttu-id="8f5fc-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f5fc-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f5fc-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f5fc-139">Response</span></span>

<span data-ttu-id="8f5fc-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8f5fc-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8f5fc-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8f5fc-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8f5fc-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f5fc-142">Request</span></span>

<span data-ttu-id="8f5fc-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f5fc-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="8f5fc-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f5fc-144">Response</span></span>

<span data-ttu-id="8f5fc-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f5fc-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
