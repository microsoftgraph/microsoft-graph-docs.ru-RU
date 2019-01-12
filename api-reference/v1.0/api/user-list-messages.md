---
title: Список сообщений
description: Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5bc831c952f13dbf67b4e7d3de6ccfd5aa28f0b1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976025"
---
# <a name="list-messages"></a><span data-ttu-id="91d9d-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="91d9d-103">List messages</span></span>

<span data-ttu-id="91d9d-104">Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные").</span><span class="sxs-lookup"><span data-stu-id="91d9d-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="91d9d-105">В настоящее время эта операция возвращает текст сообщения только в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="91d9d-105">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="91d9d-106">Существует два сценария, где приложения можно получить сообщения в почтовой папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="91d9d-106">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="91d9d-107">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="91d9d-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="91d9d-108">Если приложение имеет соответствующий делегированных [разрешений](#permissions) от одного пользователя и другой пользователь доступ к папке почты с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="91d9d-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="91d9d-109">В разделе [сведения и примеры](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="91d9d-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="91d9d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91d9d-110">Permissions</span></span>
<span data-ttu-id="91d9d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91d9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91d9d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91d9d-113">Permission type</span></span>      | <span data-ttu-id="91d9d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91d9d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91d9d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91d9d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="91d9d-116">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91d9d-116">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="91d9d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91d9d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91d9d-118">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91d9d-118">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="91d9d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91d9d-119">Application</span></span> | <span data-ttu-id="91d9d-120">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91d9d-120">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="91d9d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91d9d-121">HTTP request</span></span>

<span data-ttu-id="91d9d-122">Для получения всех сообщений в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="91d9d-122">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="91d9d-123">Для получения сообщений из определенной папки в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="91d9d-123">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91d9d-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91d9d-124">Optional query parameters</span></span>
<span data-ttu-id="91d9d-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="91d9d-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="91d9d-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91d9d-126">Request headers</span></span>
| <span data-ttu-id="91d9d-127">Имя</span><span class="sxs-lookup"><span data-stu-id="91d9d-127">Name</span></span>       | <span data-ttu-id="91d9d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="91d9d-128">Type</span></span> | <span data-ttu-id="91d9d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="91d9d-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="91d9d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="91d9d-130">Authorization</span></span>  | <span data-ttu-id="91d9d-131">строка</span><span class="sxs-lookup"><span data-stu-id="91d9d-131">string</span></span>  | <span data-ttu-id="91d9d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91d9d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91d9d-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="91d9d-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="91d9d-135">строка</span><span class="sxs-lookup"><span data-stu-id="91d9d-135">string</span></span> | <span data-ttu-id="91d9d-136">Формат возвращаемых свойств **body** и **uniqueBody**.</span><span class="sxs-lookup"><span data-stu-id="91d9d-136">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="91d9d-137">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="91d9d-137">Values can be "text" or "html".</span></span> <span data-ttu-id="91d9d-138">Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="91d9d-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="91d9d-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="91d9d-139">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="91d9d-140">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91d9d-140">Request body</span></span>
<span data-ttu-id="91d9d-141">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91d9d-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91d9d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="91d9d-142">Response</span></span>

<span data-ttu-id="91d9d-143">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91d9d-143">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="91d9d-144">Размер страницы по умолчанию для этого запроса предусматривает отображение 10 сообщений.</span><span class="sxs-lookup"><span data-stu-id="91d9d-144">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="91d9d-145">Пример</span><span class="sxs-lookup"><span data-stu-id="91d9d-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91d9d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="91d9d-146">Request</span></span>
<span data-ttu-id="91d9d-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91d9d-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="91d9d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="91d9d-148">Response</span></span>
<span data-ttu-id="91d9d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="91d9d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
