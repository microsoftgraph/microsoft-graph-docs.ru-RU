---
title: Создание outlookTask
description: Создание задачи Outlook в группе задач по умолчанию (`My Tasks`) и папки задач по умолчанию (`Tasks`) в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 935732e14f7e467e3094d4a5a2f82d2922020569
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520993"
---
# <a name="create-outlooktask"></a><span data-ttu-id="fd7b5-103">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="fd7b5-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd7b5-104">Создание задачи Outlook в группе задач по умолчанию (`My Tasks`) и папки задач по умолчанию (`Tasks`) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-104">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="fd7b5-105">Метод POST всегда игнорирует времени часть **startDateTime** и **dueDateTime** в тексте запроса и предполагается времени, всегда полночь в указанном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="fd7b5-106">По умолчанию эта операция (и операции GET, ИСПРАВЛЕНИЙ и [выполнения](../api/outlooktask-complete.md) задачи) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-106">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="fd7b5-107">Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd7b5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd7b5-108">Permissions</span></span>
<span data-ttu-id="fd7b5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd7b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd7b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd7b5-111">Permission type</span></span>      | <span data-ttu-id="fd7b5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd7b5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd7b5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd7b5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fd7b5-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd7b5-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="fd7b5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd7b5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd7b5-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd7b5-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="fd7b5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd7b5-117">Application</span></span> | <span data-ttu-id="fd7b5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd7b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd7b5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="fd7b5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd7b5-120">Request headers</span></span>
| <span data-ttu-id="fd7b5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fd7b5-121">Name</span></span>       | <span data-ttu-id="fd7b5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fd7b5-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fd7b5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd7b5-123">Authorization</span></span>  | <span data-ttu-id="fd7b5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd7b5-126">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="fd7b5-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="fd7b5-127">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="fd7b5-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd7b5-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd7b5-129">Request body</span></span>
<span data-ttu-id="fd7b5-130">В тексте запроса укажите представление JSON объекта [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="fd7b5-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fd7b5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd7b5-131">Response</span></span>

<span data-ttu-id="fd7b5-132">Успешно завершена, этот метод возвращает `201 Created` объект [outlookTask](../resources/outlooktask.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd7b5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fd7b5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd7b5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd7b5-134">Request</span></span>
<span data-ttu-id="fd7b5-135">В следующем примере показано использование `Prefer: outlook.timezone` заголовка.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-135">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="fd7b5-136">Создает задачу, выражает **startDateTime** и **dueDateTime** в Восточное время (ПРИБЛ) и включает в себя `Prefer` заголовка из Тихоокеанское время (PST).</span><span class="sxs-lookup"><span data-stu-id="fd7b5-136">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
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
<span data-ttu-id="fd7b5-137">В тексте запроса укажите представление JSON объекта [outlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="fd7b5-137">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fd7b5-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd7b5-138">Response</span></span>
<span data-ttu-id="fd7b5-139">Метод POST игнорирует времени часть **startDateTime** и **dueDateTime** в тексте запроса, а также предполагается времени, всегда полночь в указанном часовом поясе (ПРИБЛ).</span><span class="sxs-lookup"><span data-stu-id="fd7b5-139">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="fd7b5-140">Поскольку `Prefer` заголовок указывает PST-файлов, метод POST выражает все свойства зависящих от даты в ответ в PST-файлов.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-140">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="fd7b5-141">В частности для свойства **startDateTime** и **dueDateTime** метода POST преобразует полночь в EST PST-файл и возвращает их в PST-файлов в ответе.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-141">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="fd7b5-p107">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd7b5-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
