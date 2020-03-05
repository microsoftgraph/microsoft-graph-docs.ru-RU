---
title: Создание объекта outlookTask
description: Создание задачи Outlook в указанной папке задач.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d9054dbc262c9350bb3efcc17193d66f27ae5904
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456147"
---
# <a name="create-outlooktask"></a><span data-ttu-id="61d23-103">Создание объекта outlookTask</span><span class="sxs-lookup"><span data-stu-id="61d23-103">Create outlookTask</span></span>

<span data-ttu-id="61d23-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="61d23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61d23-105">Создание задачи Outlook в указанной папке задач.</span><span class="sxs-lookup"><span data-stu-id="61d23-105">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="61d23-106">Метод POST всегда игнорирует часть времени **startDateTime** и **дуедатетиме** в теле запроса и предполагает, что время будет всегда в полночь в заданном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="61d23-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="61d23-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61d23-107">Permissions</span></span>
<span data-ttu-id="61d23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61d23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61d23-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61d23-110">Permission type</span></span>      | <span data-ttu-id="61d23-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61d23-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61d23-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61d23-112">Delegated (work or school account)</span></span> | <span data-ttu-id="61d23-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61d23-113">Not supported.</span></span>    |
|<span data-ttu-id="61d23-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61d23-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61d23-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61d23-115">Not supported.</span></span>    |
|<span data-ttu-id="61d23-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61d23-116">Application</span></span> | <span data-ttu-id="61d23-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61d23-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61d23-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61d23-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="61d23-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61d23-119">Request headers</span></span>
| <span data-ttu-id="61d23-120">Имя</span><span class="sxs-lookup"><span data-stu-id="61d23-120">Name</span></span>       | <span data-ttu-id="61d23-121">Описание</span><span class="sxs-lookup"><span data-stu-id="61d23-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="61d23-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61d23-122">Authorization</span></span>  | <span data-ttu-id="61d23-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61d23-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="61d23-125">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="61d23-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="61d23-126">Задает часовой пояс для свойств времени в отклике в формате UTC, если заголовок не указан.</span><span class="sxs-lookup"><span data-stu-id="61d23-126">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="61d23-127">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="61d23-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61d23-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61d23-128">Request body</span></span>
<span data-ttu-id="61d23-129">В тексте запроса добавьте представление объекта [outlookTask](../resources/outlooktask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61d23-129">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="61d23-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="61d23-130">Response</span></span>

<span data-ttu-id="61d23-131">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTask](../resources/outlooktask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="61d23-131">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61d23-132">Пример</span><span class="sxs-lookup"><span data-stu-id="61d23-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61d23-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="61d23-133">Request</span></span>
<span data-ttu-id="61d23-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61d23-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="61d23-135">В тексте запроса добавьте представление объекта [outlookTask](../resources/outlooktask.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61d23-135">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="61d23-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="61d23-136">Response</span></span>
<span data-ttu-id="61d23-137">Метод POST игнорирует часть времени в теле запроса и принимает время в полночь всегда в заданном часовом поясе (PST).</span><span class="sxs-lookup"><span data-stu-id="61d23-137">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="61d23-138">Затем по умолчанию метод POST преобразует и отображает все свойства, связанные с датой, в формате UTC в ответе.</span><span class="sxs-lookup"><span data-stu-id="61d23-138">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="61d23-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61d23-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
