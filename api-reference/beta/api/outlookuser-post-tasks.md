---
title: Создание объекта outlookTask
description: Создайте Outlook задачу в группе задач по умолчанию () и папку задач по умолчанию () в `My Tasks` `Tasks` почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a327acde8db0928b1ade7e5fcf660f86d6cdae96
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037958"
---
# <a name="create-outlooktask-deprecated"></a><span data-ttu-id="f1801-103">Создание объекта outlookTask (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="f1801-103">Create outlookTask (deprecated)</span></span>

<span data-ttu-id="f1801-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1801-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="f1801-105">Создайте Outlook задачу в группе задач по умолчанию () и папку задач по умолчанию () в `My Tasks` `Tasks` почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1801-105">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="f1801-106">Метод POST всегда игнорирует временную часть **startDateTime** и **dueDateTime** в теле запроса и предполагает время, когда всегда будет полночь в указанном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="f1801-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="f1801-107">По умолчанию эта операция (и GET, [](../api/outlooktask-complete.md) PATCH и полные операции задач) возвращает свойства, связанные с датами в UTC.</span><span class="sxs-lookup"><span data-stu-id="f1801-107">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="f1801-108">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="f1801-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1801-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1801-109">Permissions</span></span>
<span data-ttu-id="f1801-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1801-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1801-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1801-112">Permission type</span></span>      | <span data-ttu-id="f1801-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1801-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1801-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1801-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f1801-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1801-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f1801-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1801-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1801-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1801-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f1801-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1801-118">Application</span></span> | <span data-ttu-id="f1801-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1801-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1801-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1801-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="f1801-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1801-121">Request headers</span></span>
| <span data-ttu-id="f1801-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f1801-122">Name</span></span>       | <span data-ttu-id="f1801-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f1801-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f1801-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1801-124">Authorization</span></span>  | <span data-ttu-id="f1801-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1801-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1801-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f1801-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="f1801-128">Указывает часовой пояс для свойств времени в ответе, который будет в UTC, если этот заглавный не указан.</span><span class="sxs-lookup"><span data-stu-id="f1801-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="f1801-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="f1801-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1801-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1801-130">Request body</span></span>
<span data-ttu-id="f1801-131">В теле запроса поставляем представление JSON [объекта OutlookTask.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="f1801-131">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f1801-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1801-132">Response</span></span>

<span data-ttu-id="f1801-133">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект OutlookTask](../resources/outlooktask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f1801-133">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1801-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f1801-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1801-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1801-135">Request</span></span>
<span data-ttu-id="f1801-136">В следующем примере показано использование `Prefer: outlook.timezone` загона.</span><span class="sxs-lookup"><span data-stu-id="f1801-136">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="f1801-137">Он создает задачу, выражает **startDateTime** и **dueDateTime** в восточном стандартном времени (EST) и включает в себя загон тихоокеанского стандартного времени `Prefer` (PST).</span><span class="sxs-lookup"><span data-stu-id="f1801-137">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/tasks
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 276

{
  "subject": "Shop for children's weekend",
  "startDateTime": {
      "dateTime": "2016-05-03T09:00:00",
      "timeZone": "Eastern Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-05-05T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="f1801-138">C#</span><span class="sxs-lookup"><span data-stu-id="f1801-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktask-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1801-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1801-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktask-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1801-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1801-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktask-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1801-141">Java</span><span class="sxs-lookup"><span data-stu-id="f1801-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktask-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f1801-142">В теле запроса поставляем представление JSON [объекта OutlookTask.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="f1801-142">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f1801-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1801-143">Response</span></span>
<span data-ttu-id="f1801-144">Метод POST игнорирует временную часть **startDateTime** и **dueDateTime** в теле запроса и предполагает время, когда всегда будет полночь в указанном часовом поясе (EST).</span><span class="sxs-lookup"><span data-stu-id="f1801-144">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="f1801-145">Так как в заговорке указан PST, метод POST выражает все свойства, связанные с датой, в ответе `Prefer` в PST.</span><span class="sxs-lookup"><span data-stu-id="f1801-145">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="f1801-146">В частности, для свойств **startDateTime** и **dueDateTime** метод POST преобразует полночь в EST в PST и возвращает их в PST в ответе.</span><span class="sxs-lookup"><span data-stu-id="f1801-146">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="f1801-147">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f1801-147">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 576

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [ ],
  "assignedTo": null,
  "body": {
    "contentType": "Text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments":false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "Normal",
  "startDateTime": {
    "dateTime": "2016-05-02T21:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "status": "notStarted",
  "subject": "Shop for children's weekend"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


