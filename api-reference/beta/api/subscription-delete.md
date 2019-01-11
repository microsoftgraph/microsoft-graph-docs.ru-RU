---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
ms.openlocfilehash: 1e2efb9835e5e625bdac0385b5011cfe5c8c64b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842051"
---
# <a name="delete-subscription"></a><span data-ttu-id="8a374-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="8a374-103">Delete subscription</span></span>

> <span data-ttu-id="8a374-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8a374-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a374-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a374-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a374-106">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="8a374-106">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a374-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a374-107">Permissions</span></span>

<span data-ttu-id="8a374-p102">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a374-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a374-110">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="8a374-110">Resource type / Item</span></span>        | <span data-ttu-id="8a374-111">Разрешение</span><span class="sxs-lookup"><span data-stu-id="8a374-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="8a374-112">Contacts</span><span class="sxs-lookup"><span data-stu-id="8a374-112">Contacts</span></span>                    | <span data-ttu-id="8a374-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8a374-113">Contacts.Read</span></span>       |
| <span data-ttu-id="8a374-114">Беседы</span><span class="sxs-lookup"><span data-stu-id="8a374-114">Conversations</span></span>               | <span data-ttu-id="8a374-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a374-115">Group.Read.All</span></span>      |
| <span data-ttu-id="8a374-116">События</span><span class="sxs-lookup"><span data-stu-id="8a374-116">Events</span></span>                      | <span data-ttu-id="8a374-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8a374-117">Calendars.Read</span></span>      |
| <span data-ttu-id="8a374-118">Сообщения</span><span class="sxs-lookup"><span data-stu-id="8a374-118">Messages</span></span>                    | <span data-ttu-id="8a374-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8a374-119">Mail.Read</span></span>           |
| <span data-ttu-id="8a374-120">Группы</span><span class="sxs-lookup"><span data-stu-id="8a374-120">Groups</span></span>                      | <span data-ttu-id="8a374-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a374-121">Group.Read.All</span></span>      |
| <span data-ttu-id="8a374-122">Пользователи</span><span class="sxs-lookup"><span data-stu-id="8a374-122">Users</span></span>                       | <span data-ttu-id="8a374-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a374-123">User.Read.All</span></span>       |
| <span data-ttu-id="8a374-124">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="8a374-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="8a374-125">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="8a374-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="8a374-126">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="8a374-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="8a374-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a374-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="8a374-128">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="8a374-128">Security alert</span></span>              | <span data-ttu-id="8a374-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a374-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="8a374-130">***Примечание:*** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8a374-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="8a374-131">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8a374-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="8a374-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a374-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8a374-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a374-133">Request headers</span></span>

| <span data-ttu-id="8a374-134">Имя</span><span class="sxs-lookup"><span data-stu-id="8a374-134">Name</span></span>       | <span data-ttu-id="8a374-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8a374-135">Type</span></span> | <span data-ttu-id="8a374-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8a374-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8a374-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a374-137">Authorization</span></span>  | <span data-ttu-id="8a374-138">string</span><span class="sxs-lookup"><span data-stu-id="8a374-138">string</span></span>  | <span data-ttu-id="8a374-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a374-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a374-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a374-141">Request body</span></span>

<span data-ttu-id="8a374-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a374-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a374-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a374-143">Response</span></span>

<span data-ttu-id="8a374-144">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8a374-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8a374-145">Пример</span><span class="sxs-lookup"><span data-stu-id="8a374-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8a374-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a374-146">Request</span></span>

<span data-ttu-id="8a374-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a374-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="8a374-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a374-148">Response</span></span>

<span data-ttu-id="8a374-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a374-149">Here is an example of the response.</span></span>
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
