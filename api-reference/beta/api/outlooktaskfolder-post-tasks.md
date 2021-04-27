---
title: Создание объекта outlookTask
description: Создайте Outlook задачу в указанной папке задач.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 233e93529c2b4644a69643fd8bf1f49562765127
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055437"
---
# <a name="create-outlooktask-deprecated"></a><span data-ttu-id="7f2ca-103">Создание объекта outlookTask (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="7f2ca-103">Create outlookTask (deprecated)</span></span>

<span data-ttu-id="7f2ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f2ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="7f2ca-105">Создайте Outlook задачу в указанной папке задач.</span><span class="sxs-lookup"><span data-stu-id="7f2ca-105">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="7f2ca-106">Метод POST всегда игнорирует временную часть **startDateTime** и **dueDateTime** в теле запроса и предполагает время, когда всегда будет полночь в указанном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="7f2ca-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f2ca-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f2ca-107">Permissions</span></span>
<span data-ttu-id="7f2ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f2ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f2ca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f2ca-110">Permission type</span></span>      | <span data-ttu-id="7f2ca-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f2ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f2ca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f2ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f2ca-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f2ca-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7f2ca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f2ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f2ca-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f2ca-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7f2ca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f2ca-116">Application</span></span> | <span data-ttu-id="7f2ca-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f2ca-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f2ca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f2ca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="7f2ca-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f2ca-119">Request headers</span></span>
| <span data-ttu-id="7f2ca-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7f2ca-120">Name</span></span>       | <span data-ttu-id="7f2ca-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7f2ca-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7f2ca-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f2ca-122">Authorization</span></span>  | <span data-ttu-id="7f2ca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f2ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f2ca-125">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7f2ca-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="7f2ca-126">Указывает часовой пояс для свойств времени в ответе, который будет в UTC, если этот заглавный не указан.</span><span class="sxs-lookup"><span data-stu-id="7f2ca-126">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="7f2ca-127">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7f2ca-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f2ca-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f2ca-128">Request body</span></span>
<span data-ttu-id="7f2ca-129">В теле запроса поставляем представление JSON [объекта OutlookTask.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="7f2ca-129">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7f2ca-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f2ca-130">Response</span></span>

<span data-ttu-id="7f2ca-131">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект OutlookTask](../resources/outlooktask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7f2ca-131">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f2ca-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7f2ca-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f2ca-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f2ca-133">Request</span></span>
<span data-ttu-id="7f2ca-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f2ca-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f2ca-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f2ca-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlooktaskfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders('AAMkADIyAAAhrbPXAAA=')/tasks
Content-type: application/json
Content-length: 376

{
  "subject": "Shop for dinner",
  "startDateTime": {
      "dateTime": "2016-04-23T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-04-25T13:00:00",
      "timeZone": "Pacific Standard Time"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="7f2ca-136">C#</span><span class="sxs-lookup"><span data-stu-id="7f2ca-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktask-from-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f2ca-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f2ca-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktask-from-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f2ca-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f2ca-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktask-from-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f2ca-139">Java</span><span class="sxs-lookup"><span data-stu-id="7f2ca-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktask-from-outlooktaskfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7f2ca-140">В теле запроса поставляем представление JSON [объекта OutlookTask.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="7f2ca-140">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7f2ca-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f2ca-141">Response</span></span>
<span data-ttu-id="7f2ca-142">Метод POST игнорирует время в теле запроса и предполагает время, когда всегда будет полночь в указанном часовом поясе (PST).</span><span class="sxs-lookup"><span data-stu-id="7f2ca-142">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="7f2ca-143">Затем метод POST по умолчанию преобразует и отображает все связанные с датой свойства в UTC в ответе.</span><span class="sxs-lookup"><span data-stu-id="7f2ca-143">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="7f2ca-144">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7f2ca-144">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 376

{
  "createdDateTime": "2016-04-22T05:44:01.2012012Z",
  "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
  "categories": [ ],
  "assignedTo": "null",
  "body": {
    "contentType": "Text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-04-25T07:00:00.0000000",
    "timeZone": "UTC"
  },
  "hasAttachments":false,
  "importance": "Normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTkAAAAIBEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "Normal",
  "startDateTime": {
    "dateTime": "2016-04-23T07:00:00.0000000",
    "timeZone": "UTC"
  },
  "status": "NotStarted",
  "subject": "Shop for dinner"
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
  "suppressions": []
}
-->


