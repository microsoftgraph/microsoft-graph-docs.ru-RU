---
title: Создание outlookTask
description: Создание задачи Outlook в папке указанной задачи.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 477ddf32b790da5b5d43560119d7a2529e773ad0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841421"
---
# <a name="create-outlooktask"></a><span data-ttu-id="29bd2-103">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="29bd2-103">Create outlookTask</span></span>

> <span data-ttu-id="29bd2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="29bd2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29bd2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29bd2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29bd2-106">Создание задачи Outlook в папке указанной задачи.</span><span class="sxs-lookup"><span data-stu-id="29bd2-106">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="29bd2-107">Метод POST всегда игнорирует времени часть **startDateTime** и **dueDateTime** в тексте запроса и предполагается времени, всегда полночь в указанном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="29bd2-107">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="29bd2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29bd2-108">Permissions</span></span>
<span data-ttu-id="29bd2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29bd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29bd2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29bd2-111">Permission type</span></span>      | <span data-ttu-id="29bd2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29bd2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29bd2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29bd2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="29bd2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29bd2-114">Not supported.</span></span>    |
|<span data-ttu-id="29bd2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29bd2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29bd2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29bd2-116">Not supported.</span></span>    |
|<span data-ttu-id="29bd2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29bd2-117">Application</span></span> | <span data-ttu-id="29bd2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29bd2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29bd2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29bd2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="29bd2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29bd2-120">Request headers</span></span>
| <span data-ttu-id="29bd2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="29bd2-121">Name</span></span>       | <span data-ttu-id="29bd2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="29bd2-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29bd2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29bd2-123">Authorization</span></span>  | <span data-ttu-id="29bd2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29bd2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29bd2-126">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="29bd2-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="29bd2-127">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="29bd2-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="29bd2-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="29bd2-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29bd2-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="29bd2-129">Request body</span></span>
<span data-ttu-id="29bd2-130">В тексте запроса укажите представление JSON объекта [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="29bd2-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="29bd2-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="29bd2-131">Response</span></span>

<span data-ttu-id="29bd2-132">Успешно завершена, этот метод возвращает `201 Created` объект [outlookTask](../resources/outlooktask.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="29bd2-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29bd2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="29bd2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29bd2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="29bd2-134">Request</span></span>
<span data-ttu-id="29bd2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29bd2-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlooktaskfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskfolders('AAMkADIyAAAhrbPXAAA=')/tasks
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
<span data-ttu-id="29bd2-136">В тексте запроса укажите представление JSON объекта [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="29bd2-136">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="29bd2-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="29bd2-137">Response</span></span>
<span data-ttu-id="29bd2-138">Метод POST игнорирует области времени в тексте запроса, а также предполагается времени, всегда полночь в указанном часовом поясе (PST).</span><span class="sxs-lookup"><span data-stu-id="29bd2-138">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="29bd2-139">Затем по умолчанию, метод POST преобразует и отображает все свойства зависящих от даты в формате UTC в ответе.</span><span class="sxs-lookup"><span data-stu-id="29bd2-139">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="29bd2-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29bd2-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
