---
title: 'outlookTask: завершено'
description: 'Выполните задачу Outlook, которая устанавливает для свойства **комплетеддатетиме** текущую дату. '
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 83fd7935e03791e3695454ff99eac7d5397817d9
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311578"
---
# <a name="outlooktask-complete-deprecated"></a><span data-ttu-id="c880f-103">outlookTask: Complete (устарело)</span><span class="sxs-lookup"><span data-stu-id="c880f-103">outlookTask: complete (deprecated)</span></span>

<span data-ttu-id="c880f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c880f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="c880f-105">Выполните задачу Outlook, которая устанавливает для свойства **комплетеддатетиме** текущую дату, а свойству **Status** — значение `completed` .</span><span class="sxs-lookup"><span data-stu-id="c880f-105">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="c880f-106">Если вы завершаете задачу в повторяющейся серии, в ответе коллекция задач будет содержать завершенную задачу в ряду и следующую задачу в ряду.</span><span class="sxs-lookup"><span data-stu-id="c880f-106">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="c880f-107">Свойство **комплетеддатетиме** представляет дату завершения задачи.</span><span class="sxs-lookup"><span data-stu-id="c880f-107">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="c880f-108">По умолчанию для части времени **комплетеддатетиме** по умолчанию задается полночь UTC.</span><span class="sxs-lookup"><span data-stu-id="c880f-108">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="c880f-109">По умолчанию эта операция (и операции задания POST, GET и PATCH) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c880f-109">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="c880f-110">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="c880f-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="c880f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c880f-111">Permissions</span></span>

<span data-ttu-id="c880f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c880f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c880f-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c880f-114">Permission type</span></span>      | <span data-ttu-id="c880f-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c880f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c880f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c880f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c880f-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c880f-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c880f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c880f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c880f-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c880f-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c880f-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c880f-120">Application</span></span> | <span data-ttu-id="c880f-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c880f-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c880f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c880f-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="c880f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c880f-123">Request headers</span></span>

| <span data-ttu-id="c880f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c880f-124">Name</span></span>       | <span data-ttu-id="c880f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c880f-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c880f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c880f-126">Authorization</span></span>  | <span data-ttu-id="c880f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c880f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c880f-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c880f-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="c880f-130">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="c880f-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="c880f-131">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c880f-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c880f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c880f-132">Request body</span></span>

<span data-ttu-id="c880f-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c880f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c880f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c880f-134">Response</span></span>

<span data-ttu-id="c880f-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c880f-135">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c880f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c880f-136">Example</span></span>

<span data-ttu-id="c880f-137">В приведенном ниже примере указанная задача отмечается как завершенная.</span><span class="sxs-lookup"><span data-stu-id="c880f-137">The following example marks the specified task as complete.</span></span> <span data-ttu-id="c880f-138">В нем задается тихоокеанское стандартное время (PST) в `Prefer: outlook.timezone` заголовке.</span><span class="sxs-lookup"><span data-stu-id="c880f-138">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="c880f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c880f-139">Request</span></span>

<span data-ttu-id="c880f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c880f-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="c880f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c880f-141">Response</span></span>

<span data-ttu-id="c880f-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c880f-142">Here is an example of the response.</span></span> <span data-ttu-id="c880f-143">Свойства **комплетеддатетиме** и другие связанные с датами свойства в отклике выражаются в PST-файле.</span><span class="sxs-lookup"><span data-stu-id="c880f-143">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="c880f-144">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c880f-144">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c880f-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c880f-145">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
