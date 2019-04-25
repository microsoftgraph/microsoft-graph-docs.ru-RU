---
title: 'outlookTask: завершено'
description: 'Выполните задачу Outlook, которая устанавливает для свойства **комплетеддатетиме** текущую дату. '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: de3d47d59b89f8bbef42b8b17a9099ecf9e80c98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539907"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="bdd9f-103">outlookTask: завершено</span><span class="sxs-lookup"><span data-stu-id="bdd9f-103">outlookTask: complete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdd9f-104">Выполните задачу Outlook, которая устанавливает для свойства **комплетеддатетиме** текущую дату, а свойству **Status** — значение `completed`.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-104">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="bdd9f-105">Если вы завершаете задачу в повторяющейся серии, в ответе коллекция задач будет содержать завершенную задачу в ряду и следующую задачу в ряду.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-105">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="bdd9f-106">Свойство **комплетеддатетиме** представляет дату завершения задачи.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-106">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="bdd9f-107">По умолчанию для части времени **комплетеддатетиме** по умолчанию задается полночь UTC.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-107">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="bdd9f-108">По умолчанию эта операция (и операции задания POST, GET и PATCH) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-108">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="bdd9f-109">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdd9f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdd9f-110">Permissions</span></span>

<span data-ttu-id="bdd9f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdd9f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdd9f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdd9f-113">Permission type</span></span>      | <span data-ttu-id="bdd9f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdd9f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdd9f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdd9f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="bdd9f-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdd9f-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="bdd9f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdd9f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd9f-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdd9f-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="bdd9f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdd9f-119">Application</span></span> | <span data-ttu-id="bdd9f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdd9f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdd9f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="bdd9f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdd9f-122">Request headers</span></span>

| <span data-ttu-id="bdd9f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="bdd9f-123">Name</span></span>       | <span data-ttu-id="bdd9f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="bdd9f-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bdd9f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdd9f-125">Authorization</span></span>  | <span data-ttu-id="bdd9f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdd9f-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="bdd9f-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="bdd9f-129">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="bdd9f-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdd9f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdd9f-131">Request body</span></span>

<span data-ttu-id="bdd9f-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdd9f-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdd9f-133">Response</span></span>

<span data-ttu-id="bdd9f-134">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-134">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdd9f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bdd9f-135">Example</span></span>

<span data-ttu-id="bdd9f-136">В приведенном ниже примере указанная задача отмечается как завершенная.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-136">The following example marks the specified task as complete.</span></span> <span data-ttu-id="bdd9f-137">В нем задается тихоокеанское стандартное время (PST `Prefer: outlook.timezone` ) в заголовке.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-137">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="bdd9f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdd9f-138">Request</span></span>

<span data-ttu-id="bdd9f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="bdd9f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdd9f-140">Response</span></span>

<span data-ttu-id="bdd9f-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-141">Here is an example of the response.</span></span> <span data-ttu-id="bdd9f-142">Свойства **комплетеддатетиме** и другие связанные с датами свойства в отклике выражаются в PST-файле.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-142">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="bdd9f-143">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-143">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bdd9f-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdd9f-144">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-complete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
