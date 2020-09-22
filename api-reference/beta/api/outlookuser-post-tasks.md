---
title: Создание объекта outlookTask
description: Создайте задачу Outlook в группе задач по умолчанию ( `My Tasks` ) и папке задач по умолчанию ( `Tasks` ) в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5adb1afed482c7080cb06ecb70a2612ac37758ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074267"
---
# <a name="create-outlooktask-deprecated"></a><span data-ttu-id="ceb71-103">Создание outlookTask (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="ceb71-103">Create outlookTask (deprecated)</span></span>

<span data-ttu-id="ceb71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceb71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="ceb71-105">Создайте задачу Outlook в группе задач по умолчанию ( `My Tasks` ) и папке задач по умолчанию ( `Tasks` ) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="ceb71-105">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="ceb71-106">Метод POST всегда игнорирует часть времени **startDateTime** и **дуедатетиме** в теле запроса и предполагает, что время будет всегда в полночь в заданном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="ceb71-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="ceb71-107">По умолчанию эта операция (а также операции GET, PATCH и [Complete](../api/outlooktask-complete.md) ) Возвращает свойства, связанные с датами, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ceb71-107">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="ceb71-108">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="ceb71-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="ceb71-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ceb71-109">Permissions</span></span>
<span data-ttu-id="ceb71-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceb71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceb71-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ceb71-112">Permission type</span></span>      | <span data-ttu-id="ceb71-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ceb71-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ceb71-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ceb71-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ceb71-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceb71-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ceb71-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ceb71-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceb71-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceb71-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ceb71-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ceb71-118">Application</span></span> | <span data-ttu-id="ceb71-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceb71-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ceb71-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ceb71-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="ceb71-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ceb71-121">Request headers</span></span>
| <span data-ttu-id="ceb71-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ceb71-122">Name</span></span>       | <span data-ttu-id="ceb71-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ceb71-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ceb71-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ceb71-124">Authorization</span></span>  | <span data-ttu-id="ceb71-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ceb71-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ceb71-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ceb71-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="ceb71-128">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="ceb71-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="ceb71-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="ceb71-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceb71-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ceb71-130">Request body</span></span>
<span data-ttu-id="ceb71-131">В тексте запроса добавьте представление объекта [outlookTask](../resources/outlooktask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ceb71-131">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ceb71-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ceb71-132">Response</span></span>

<span data-ttu-id="ceb71-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ceb71-133">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceb71-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ceb71-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ceb71-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ceb71-135">Request</span></span>
<span data-ttu-id="ceb71-136">В приведенном ниже примере показано использование `Prefer: outlook.timezone` заголовка.</span><span class="sxs-lookup"><span data-stu-id="ceb71-136">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="ceb71-137">Он создает задачу, выражает **startDateTime** и **Дуедатетиме** в восточное стандартное время (EST) и включает `Prefer` заголовку тихоокеанского стандартного времени (PST).</span><span class="sxs-lookup"><span data-stu-id="ceb71-137">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
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
# <a name="c"></a>[<span data-ttu-id="ceb71-138">C#</span><span class="sxs-lookup"><span data-stu-id="ceb71-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktask-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ceb71-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ceb71-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktask-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ceb71-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ceb71-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktask-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ceb71-141">В тексте запроса добавьте представление объекта [outlookTask](../resources/outlooktask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ceb71-141">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ceb71-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ceb71-142">Response</span></span>
<span data-ttu-id="ceb71-143">Метод POST игнорирует часть времени **startDateTime** и **дуедатетиме** в теле запроса и предполагает, что время будет всегда в полночь в заданном часовом поясе (EST).</span><span class="sxs-lookup"><span data-stu-id="ceb71-143">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="ceb71-144">Так как `Prefer` Заголовок указывает PST-файл, метод POST выражает все свойства, связанные с датами, в ответе в PST-файле.</span><span class="sxs-lookup"><span data-stu-id="ceb71-144">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="ceb71-145">В частности, для свойств **startDateTime** и **дуедатетиме** метод POST преобразовывает полночь в СРЕДСТВе EST в PST-файл и возвращает их в PST-файле в ответе.</span><span class="sxs-lookup"><span data-stu-id="ceb71-145">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="ceb71-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ceb71-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "assignedTo": null,
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
  ]
}
-->


