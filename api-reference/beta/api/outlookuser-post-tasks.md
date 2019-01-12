---
title: Создание outlookTask
description: Создание задачи Outlook в группе задач по умолчанию (`My Tasks`) и папки задач по умолчанию (`Tasks`) в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 04cc91f9c6eee09f71783d0548470d167911ec91
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925597"
---
# <a name="create-outlooktask"></a><span data-ttu-id="36724-103">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="36724-103">Create outlookTask</span></span>

> <span data-ttu-id="36724-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="36724-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36724-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36724-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36724-106">Создание задачи Outlook в группе задач по умолчанию (`My Tasks`) и папки задач по умолчанию (`Tasks`) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="36724-106">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="36724-107">Метод POST всегда игнорирует времени часть **startDateTime** и **dueDateTime** в тексте запроса и предполагается времени, всегда полночь в указанном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="36724-107">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="36724-108">По умолчанию эта операция (и операции GET, ИСПРАВЛЕНИЙ и [выполнения](../api/outlooktask-complete.md) задачи) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="36724-108">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="36724-109">Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.</span><span class="sxs-lookup"><span data-stu-id="36724-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="36724-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36724-110">Permissions</span></span>
<span data-ttu-id="36724-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36724-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36724-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36724-113">Permission type</span></span>      | <span data-ttu-id="36724-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36724-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36724-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36724-115">Delegated (work or school account)</span></span> | <span data-ttu-id="36724-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36724-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="36724-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36724-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36724-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36724-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="36724-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36724-119">Application</span></span> | <span data-ttu-id="36724-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36724-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36724-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36724-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="36724-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36724-122">Request headers</span></span>
| <span data-ttu-id="36724-123">Имя</span><span class="sxs-lookup"><span data-stu-id="36724-123">Name</span></span>       | <span data-ttu-id="36724-124">Описание</span><span class="sxs-lookup"><span data-stu-id="36724-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="36724-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36724-125">Authorization</span></span>  | <span data-ttu-id="36724-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36724-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36724-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="36724-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="36724-129">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="36724-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="36724-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="36724-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36724-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36724-131">Request body</span></span>
<span data-ttu-id="36724-132">В тексте запроса укажите представление JSON объекта [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="36724-132">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="36724-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="36724-133">Response</span></span>

<span data-ttu-id="36724-134">Успешно завершена, этот метод возвращает `201 Created` объект [outlookTask](../resources/outlooktask.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="36724-134">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36724-135">Пример</span><span class="sxs-lookup"><span data-stu-id="36724-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36724-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="36724-136">Request</span></span>
<span data-ttu-id="36724-137">В следующем примере показано использование `Prefer: outlook.timezone` заголовка.</span><span class="sxs-lookup"><span data-stu-id="36724-137">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="36724-138">Создает задачу, выражает **startDateTime** и **dueDateTime** в Восточное время (ПРИБЛ) и включает в себя `Prefer` заголовка из Тихоокеанское время (PST).</span><span class="sxs-lookup"><span data-stu-id="36724-138">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
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
  "assignedTo": "Dana Swope",
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
<span data-ttu-id="36724-139">В тексте запроса укажите представление JSON объекта [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="36724-139">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="36724-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="36724-140">Response</span></span>
<span data-ttu-id="36724-141">Метод POST игнорирует времени часть **startDateTime** и **dueDateTime** в тексте запроса, а также предполагается времени, всегда полночь в указанном часовом поясе (ПРИБЛ).</span><span class="sxs-lookup"><span data-stu-id="36724-141">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="36724-142">Поскольку `Prefer` заголовок указывает PST-файлов, метод POST выражает все свойства зависящих от даты в ответ в PST-файлов.</span><span class="sxs-lookup"><span data-stu-id="36724-142">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="36724-143">В частности для свойства **startDateTime** и **dueDateTime** метода POST преобразует полночь в EST PST-файл и возвращает их в PST-файлов в ответе.</span><span class="sxs-lookup"><span data-stu-id="36724-143">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="36724-p108">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36724-p108">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "assignedTo": "Dana Swope",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
