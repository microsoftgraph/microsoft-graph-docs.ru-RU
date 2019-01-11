---
title: 'outlookTask: завершена'
description: 'Завершить задачу Outlook, в котором задается свойство **completedDateTime** текущей дате '
localization_priority: Normal
ms.openlocfilehash: 6a033624a1fafbc30b200550acc466f7fdb432d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891919"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="0598f-103">outlookTask: завершена</span><span class="sxs-lookup"><span data-stu-id="0598f-103">outlookTask: complete</span></span>

> <span data-ttu-id="0598f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0598f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0598f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0598f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0598f-106">Завершить задачу Outlook, в котором задается свойство **completedDateTime** текущей дате и свойство **состояние** для `completed`.</span><span class="sxs-lookup"><span data-stu-id="0598f-106">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="0598f-107">При завершении задачи в ряде повторяющихся в ответ, коллекция задач будет содержать выполненной задачи в серии и следующую задачу из серии.</span><span class="sxs-lookup"><span data-stu-id="0598f-107">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="0598f-108">Свойство **completedDateTime** представляет дату окончания задачи.</span><span class="sxs-lookup"><span data-stu-id="0598f-108">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="0598f-109">Часть времени **completedDateTime** по умолчанию имеет значение полуночи в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0598f-109">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="0598f-110">По умолчанию эта операция (и операции задачи POST, GET и ИСПРАВЛЕНИЯ) возвращает свойства, связанные с даты в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0598f-110">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="0598f-111">Можно использовать `Prefer: outlook.timezone` заголовок, чтобы все свойства, связанный с данными в ответ, представленного в часовом поясе, отличного от UTC.</span><span class="sxs-lookup"><span data-stu-id="0598f-111">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="0598f-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0598f-112">Permissions</span></span>

<span data-ttu-id="0598f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0598f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0598f-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0598f-115">Permission type</span></span>      | <span data-ttu-id="0598f-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0598f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0598f-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0598f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0598f-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0598f-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="0598f-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0598f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0598f-120">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0598f-120">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="0598f-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0598f-121">Application</span></span> | <span data-ttu-id="0598f-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0598f-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0598f-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0598f-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="0598f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0598f-124">Request headers</span></span>

| <span data-ttu-id="0598f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="0598f-125">Name</span></span>       | <span data-ttu-id="0598f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0598f-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0598f-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0598f-127">Authorization</span></span>  | <span data-ttu-id="0598f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0598f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0598f-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="0598f-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="0598f-131">Указывает часовой пояс для свойств времени в ответ, который может быть в формате UTC, если не указан этот заголовок.</span><span class="sxs-lookup"><span data-stu-id="0598f-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="0598f-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="0598f-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0598f-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0598f-133">Request body</span></span>

<span data-ttu-id="0598f-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0598f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0598f-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="0598f-135">Response</span></span>

<span data-ttu-id="0598f-136">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [outlookTask](../resources/outlooktask.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0598f-136">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0598f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="0598f-137">Example</span></span>

<span data-ttu-id="0598f-138">В следующем примере указывается указанной задачи как завершенные.</span><span class="sxs-lookup"><span data-stu-id="0598f-138">The following example marks the specified task as complete.</span></span> <span data-ttu-id="0598f-139">Указывает Тихоокеанское время (PST) в `Prefer: outlook.timezone` заголовка.</span><span class="sxs-lookup"><span data-stu-id="0598f-139">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="0598f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0598f-140">Request</span></span>

<span data-ttu-id="0598f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0598f-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="0598f-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="0598f-142">Response</span></span>

<span data-ttu-id="0598f-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0598f-143">Here is an example of the response.</span></span> <span data-ttu-id="0598f-144">**CompletedDateTime** и другие свойства, связанные с даты в ответе выражаются в PST-файлов.</span><span class="sxs-lookup"><span data-stu-id="0598f-144">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="0598f-145">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0598f-145">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0598f-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0598f-146">All of the properties will be returned from an actual call.</span></span>
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
