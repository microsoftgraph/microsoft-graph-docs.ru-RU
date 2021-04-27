---
title: 'outlookTask: полный'
description: 'Выполните задачу Outlook, которая задает **свойство completedDateTime** к текущей дате, '
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 35ff88db1fb8cde5c84a6010fc6e33b81661c387
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055486"
---
# <a name="outlooktask-complete-deprecated"></a><span data-ttu-id="db4de-103">outlookTask: полный (неподготовленный)</span><span class="sxs-lookup"><span data-stu-id="db4de-103">outlookTask: complete (deprecated)</span></span>

<span data-ttu-id="db4de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db4de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="db4de-105">Выполните задачу Outlook, которая задает свойство **completedDateTime** к текущей дате, а свойство **состояния** `completed` — .</span><span class="sxs-lookup"><span data-stu-id="db4de-105">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="db4de-106">Если вы завершаете задачу в повторяющейся серии, в ответе коллекция задач будет содержать завершенную задачу в серии и следующую задачу в серии.</span><span class="sxs-lookup"><span data-stu-id="db4de-106">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="db4de-107">Свойство **completedDateTime** представляет дату завершения задачи.</span><span class="sxs-lookup"><span data-stu-id="db4de-107">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="db4de-108">Временная часть **completedDateTime** по умолчанию задана до полуночи UTC.</span><span class="sxs-lookup"><span data-stu-id="db4de-108">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="db4de-109">По умолчанию эта операция (и задачи POST, GET и PATCH) возвращает свойства, связанные с датами в UTC.</span><span class="sxs-lookup"><span data-stu-id="db4de-109">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="db4de-110">Можно использовать заголовок `Prefer: outlook.timezone`, чтобы все свойства, связанные с датами, были представлены в часовом поясе, отличном от UTC.</span><span class="sxs-lookup"><span data-stu-id="db4de-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="db4de-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db4de-111">Permissions</span></span>

<span data-ttu-id="db4de-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db4de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db4de-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db4de-114">Permission type</span></span>      | <span data-ttu-id="db4de-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db4de-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db4de-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db4de-116">Delegated (work or school account)</span></span> | <span data-ttu-id="db4de-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db4de-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="db4de-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db4de-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db4de-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db4de-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="db4de-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db4de-120">Application</span></span> | <span data-ttu-id="db4de-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db4de-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db4de-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db4de-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="db4de-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db4de-123">Request headers</span></span>

| <span data-ttu-id="db4de-124">Имя</span><span class="sxs-lookup"><span data-stu-id="db4de-124">Name</span></span>       | <span data-ttu-id="db4de-125">Описание</span><span class="sxs-lookup"><span data-stu-id="db4de-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db4de-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db4de-126">Authorization</span></span>  | <span data-ttu-id="db4de-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db4de-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db4de-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="db4de-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="db4de-130">Указывает часовой пояс для свойств времени в ответе, который будет в UTC, если этот заглавный не указан.</span><span class="sxs-lookup"><span data-stu-id="db4de-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="db4de-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="db4de-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db4de-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db4de-132">Request body</span></span>

<span data-ttu-id="db4de-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db4de-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db4de-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="db4de-134">Response</span></span>

<span data-ttu-id="db4de-135">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект OutlookTask](../resources/outlooktask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="db4de-135">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db4de-136">Пример</span><span class="sxs-lookup"><span data-stu-id="db4de-136">Example</span></span>

<span data-ttu-id="db4de-137">В следующем примере указанная задача будет завершена.</span><span class="sxs-lookup"><span data-stu-id="db4de-137">The following example marks the specified task as complete.</span></span> <span data-ttu-id="db4de-138">Он указывает тихоокеанское стандартное время (PST) в `Prefer: outlook.timezone` заговорке.</span><span class="sxs-lookup"><span data-stu-id="db4de-138">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="db4de-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="db4de-139">Request</span></span>

<span data-ttu-id="db4de-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db4de-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db4de-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="db4de-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="db4de-142">C#</span><span class="sxs-lookup"><span data-stu-id="db4de-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlooktask-complete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db4de-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db4de-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlooktask-complete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db4de-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db4de-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlooktask-complete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db4de-145">Java</span><span class="sxs-lookup"><span data-stu-id="db4de-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/outlooktask-complete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db4de-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="db4de-146">Response</span></span>

<span data-ttu-id="db4de-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db4de-147">Here is an example of the response.</span></span> <span data-ttu-id="db4de-148">Свойства **completedDateTime** и другие свойства, связанные с датами в ответе, выражены в PST.</span><span class="sxs-lookup"><span data-stu-id="db4de-148">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="db4de-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="db4de-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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


