---
title: Создание объекта outlookTask
description: Создайте задачу Outlook в указанной папке задач.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7278347dce74138b6eb38281f32dc7b968a9aacb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472456"
---
# <a name="create-outlooktask-deprecated"></a><span data-ttu-id="aaebc-103">Создание объекта outlookTask (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="aaebc-103">Create outlookTask (deprecated)</span></span>

<span data-ttu-id="aaebc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaebc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="aaebc-105">Создайте задачу Outlook в указанной папке задач.</span><span class="sxs-lookup"><span data-stu-id="aaebc-105">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="aaebc-106">Метод POST всегда игнорирует временную часть **startDateTime** и **dueDateTime** в теле запроса и предполагает время, когда всегда будет полночь в указанном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="aaebc-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaebc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aaebc-107">Permissions</span></span>
<span data-ttu-id="aaebc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaebc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaebc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaebc-110">Permission type</span></span>      | <span data-ttu-id="aaebc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaebc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaebc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaebc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aaebc-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaebc-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="aaebc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaebc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaebc-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaebc-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="aaebc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaebc-116">Application</span></span> | <span data-ttu-id="aaebc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaebc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaebc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaebc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="aaebc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaebc-119">Request headers</span></span>
| <span data-ttu-id="aaebc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="aaebc-120">Name</span></span>       | <span data-ttu-id="aaebc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="aaebc-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aaebc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aaebc-122">Authorization</span></span>  | <span data-ttu-id="aaebc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aaebc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aaebc-125">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="aaebc-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="aaebc-126">Указывает часовой пояс для свойств времени в ответе, который будет в UTC, если этот заглавный не указан.</span><span class="sxs-lookup"><span data-stu-id="aaebc-126">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="aaebc-127">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="aaebc-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaebc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aaebc-128">Request body</span></span>
<span data-ttu-id="aaebc-129">В теле запроса поставляем представление JSON [объекта OutlookTask.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="aaebc-129">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aaebc-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaebc-130">Response</span></span>

<span data-ttu-id="aaebc-131">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект OutlookTask](../resources/outlooktask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aaebc-131">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaebc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="aaebc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aaebc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaebc-133">Request</span></span>
<span data-ttu-id="aaebc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaebc-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="aaebc-135">В теле запроса поставляем представление JSON [объекта OutlookTask.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="aaebc-135">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="aaebc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaebc-136">Response</span></span>
<span data-ttu-id="aaebc-137">Метод POST игнорирует время в теле запроса и предполагает время, когда всегда будет полночь в указанном часовом поясе (PST).</span><span class="sxs-lookup"><span data-stu-id="aaebc-137">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="aaebc-138">Затем метод POST по умолчанию преобразует и отображает все связанные с датой свойства в UTC в ответе.</span><span class="sxs-lookup"><span data-stu-id="aaebc-138">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="aaebc-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aaebc-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


