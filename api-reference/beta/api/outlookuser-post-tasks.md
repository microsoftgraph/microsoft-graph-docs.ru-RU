---
title: Создание outlookTask
description: Создайте задачу Outlook в группе задач по умолчанию (`My Tasks`) и папке задач по умолчанию (`Tasks`) в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f508aa05ad70246584ebc33bfaabc9317205011d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596100"
---
# <a name="create-outlooktask"></a><span data-ttu-id="f29cc-103">Создание outlookTask</span><span class="sxs-lookup"><span data-stu-id="f29cc-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f29cc-104">Создайте задачу Outlook в группе задач по умолчанию (`My Tasks`) и папке задач по умолчанию (`Tasks`) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="f29cc-104">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="f29cc-105">Метод POST всегда игнорирует часть времени **startDateTime** и **дуедатетиме** в теле запроса и предполагает, что время будет всегда в полночь в заданном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="f29cc-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="f29cc-106">По умолчанию эта операция (а также операции GET, PATCH и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f29cc-106">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="f29cc-107">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="f29cc-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="f29cc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f29cc-108">Permissions</span></span>
<span data-ttu-id="f29cc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f29cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f29cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f29cc-111">Permission type</span></span>      | <span data-ttu-id="f29cc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f29cc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f29cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f29cc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f29cc-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f29cc-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f29cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f29cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f29cc-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f29cc-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f29cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f29cc-117">Application</span></span> | <span data-ttu-id="f29cc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f29cc-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f29cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f29cc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="f29cc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f29cc-120">Request headers</span></span>
| <span data-ttu-id="f29cc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f29cc-121">Name</span></span>       | <span data-ttu-id="f29cc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f29cc-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f29cc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f29cc-123">Authorization</span></span>  | <span data-ttu-id="f29cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f29cc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f29cc-126">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f29cc-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="f29cc-127">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="f29cc-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="f29cc-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="f29cc-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f29cc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f29cc-129">Request body</span></span>
<span data-ttu-id="f29cc-130">В тексте запроса добавьте представление объекта [OutlookTask](../resources/outlooktask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f29cc-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f29cc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f29cc-131">Response</span></span>

<span data-ttu-id="f29cc-132">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f29cc-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f29cc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f29cc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f29cc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f29cc-134">Request</span></span>
<span data-ttu-id="f29cc-135">В приведенном ниже примере показано использование `Prefer: outlook.timezone` заголовка.</span><span class="sxs-lookup"><span data-stu-id="f29cc-135">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="f29cc-136">Он создает задачу, выражает **startDateTime** и **Дуедатетиме** в восточное стандартное время (EST) и включает `Prefer` заголовку тихоокеанского стандартного времени (PST).</span><span class="sxs-lookup"><span data-stu-id="f29cc-136">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
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
<span data-ttu-id="f29cc-137">В тексте запроса добавьте представление объекта [OutlookTask](../resources/outlooktask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f29cc-137">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f29cc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f29cc-138">Response</span></span>
<span data-ttu-id="f29cc-139">Метод POST игнорирует часть времени **startDateTime** и **дуедатетиме** в теле запроса и предполагает, что время будет всегда в полночь в заданном часовом поясе (EST).</span><span class="sxs-lookup"><span data-stu-id="f29cc-139">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="f29cc-140">Так как `Prefer` заголовок указывает PST-файл, метод POST выражает все свойства, связанные с датами, в ответе в PST-файле.</span><span class="sxs-lookup"><span data-stu-id="f29cc-140">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="f29cc-141">В частности, для свойств **startDateTime** и **дуедатетиме** метод POST преобразовывает полночь в СРЕДСТВе EST в PST-файл и возвращает их в PST-файле в ответе.</span><span class="sxs-lookup"><span data-stu-id="f29cc-141">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="f29cc-142">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f29cc-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f29cc-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f29cc-143">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f29cc-144">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="f29cc-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f29cc-145">Языках</span><span class="sxs-lookup"><span data-stu-id="f29cc-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_outlooktask_from_outlookuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f29cc-146">Язык</span><span class="sxs-lookup"><span data-stu-id="f29cc-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_outlooktask_from_outlookuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
