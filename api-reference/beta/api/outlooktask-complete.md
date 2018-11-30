---
title: 'outlookTask: завершена'
description: 'Завершить задачу Outlook, в котором задается свойство **completedDateTime** текущей дате '
ms.openlocfilehash: 732da0f3eb03f6a4674e1254586ae21b5f3334bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081040"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="6add0-103">outlookTask: завершена</span><span class="sxs-lookup"><span data-stu-id="6add0-103">outlookTask: complete</span></span>

> <span data-ttu-id="6add0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6add0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6add0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6add0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6add0-106">Завершить задачу Outlook, в котором задается свойство **completedDateTime** текущей дате и свойство **состояние** для `completed`.</span><span class="sxs-lookup"><span data-stu-id="6add0-106">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="6add0-107">При завершении задачи в ряде повторяющихся в ответ, коллекция задач будет содержать выполненной задачи в серии и следующую задачу из серии.</span><span class="sxs-lookup"><span data-stu-id="6add0-107">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="6add0-108">Свойство **completedDateTime** представляет дату окончания задачи.</span><span class="sxs-lookup"><span data-stu-id="6add0-108">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="6add0-109">Часть времени **completedDateTime** по умолчанию имеет значение полуночи в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6add0-109">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span> 

<span data-ttu-id="6add0-110">По умолчанию эта операция (и операции задачи POST, GET и ИСПРАВЛЕНИЯ) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6add0-110">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="6add0-111">Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.</span><span class="sxs-lookup"><span data-stu-id="6add0-111">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="6add0-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6add0-112">Permissions</span></span>
<span data-ttu-id="6add0-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6add0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6add0-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6add0-115">Permission type</span></span>      | <span data-ttu-id="6add0-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6add0-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6add0-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6add0-117">Delegated (work or school account)</span></span> | <span data-ttu-id="6add0-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6add0-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="6add0-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6add0-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6add0-120">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6add0-120">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="6add0-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6add0-121">Application</span></span> | <span data-ttu-id="6add0-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6add0-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6add0-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6add0-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}/complete

```
## <a name="request-headers"></a><span data-ttu-id="6add0-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6add0-124">Request headers</span></span>
| <span data-ttu-id="6add0-125">Имя</span><span class="sxs-lookup"><span data-stu-id="6add0-125">Name</span></span>       | <span data-ttu-id="6add0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6add0-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6add0-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6add0-127">Authorization</span></span>  | <span data-ttu-id="6add0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6add0-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6add0-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="6add0-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="6add0-131">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="6add0-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="6add0-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6add0-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6add0-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6add0-133">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6add0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6add0-134">Response</span></span>

<span data-ttu-id="6add0-135">Успешно завершена, этот метод возвращает `200 OK` кода и [outlookTask](../resources/outlooktask.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6add0-135">If successful, this method returns `200 OK` response code and [outlookTask](../resources/outlooktask.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6add0-136">Пример</span><span class="sxs-lookup"><span data-stu-id="6add0-136">Example</span></span>
<span data-ttu-id="6add0-137">В следующем примере указывается указанной задачи как завершенные.</span><span class="sxs-lookup"><span data-stu-id="6add0-137">The following example marks the specified task as complete.</span></span> <span data-ttu-id="6add0-138">Указывает Тихоокеанское время (PST) в `Prefer: outlook.timezone` заголовка.</span><span class="sxs-lookup"><span data-stu-id="6add0-138">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>
##### <a name="request"></a><span data-ttu-id="6add0-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6add0-139">Request</span></span>
<span data-ttu-id="6add0-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6add0-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->
```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response"></a><span data-ttu-id="6add0-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="6add0-141">Response</span></span>
<span data-ttu-id="6add0-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6add0-142">Here is an example of the response.</span></span> <span data-ttu-id="6add0-143">**CompletedDateTime** и другие свойства, связанные с даты в ответе выражаются в PST-файлов.</span><span class="sxs-lookup"><span data-stu-id="6add0-143">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span> 

<span data-ttu-id="6add0-p109">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6add0-p109">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 465

{
  "value": [
    {
      "id": "AAMkADA1MT15rfAAA=",
      "createdDateTime": "2016-04-21T22:44:01.2012012-07:00",
      "lastModifiedDateTime": "2016-04-22T19:28:38.5300447-07:00",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XYQ==",
      "categories": [
      ],
      "assignedTo": null,
      "body": {
          "contentType": "text",
          "content": ""
      },
      "completedDateTime": {
          "dateTime": "2016-04-22T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "dueDateTime": {
          "dateTime": "2016-04-25T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTIBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
          "dateTime": "2016-04-21T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "status": "completed",
      "subject": "Shop for dinner"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->