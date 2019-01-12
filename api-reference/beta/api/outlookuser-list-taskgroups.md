---
title: Список taskGroups
description: Получение всех групп задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 3e0146a40698f8f150f39064b38aa562756b64ae
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913711"
---
# <a name="list-taskgroups"></a><span data-ttu-id="96065-103">Список taskGroups</span><span class="sxs-lookup"><span data-stu-id="96065-103">List taskGroups</span></span>

> <span data-ttu-id="96065-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="96065-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96065-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96065-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96065-106">Получение всех групп задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="96065-106">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="96065-107">Ответ всегда включает в себя группу задач по умолчанию `My Tasks`и других групп задач, которые были созданы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="96065-107">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="96065-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96065-108">Permissions</span></span>
<span data-ttu-id="96065-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96065-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96065-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96065-111">Permission type</span></span>      | <span data-ttu-id="96065-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96065-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96065-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96065-113">Delegated (work or school account)</span></span> | <span data-ttu-id="96065-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="96065-114">Tasks.Read</span></span>    |
|<span data-ttu-id="96065-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96065-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96065-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="96065-116">Tasks.Read</span></span>    |
|<span data-ttu-id="96065-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96065-117">Application</span></span> | <span data-ttu-id="96065-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96065-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96065-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96065-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96065-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="96065-120">Optional query parameters</span></span>
<span data-ttu-id="96065-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="96065-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96065-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96065-122">Request headers</span></span>
| <span data-ttu-id="96065-123">Имя</span><span class="sxs-lookup"><span data-stu-id="96065-123">Name</span></span>      |<span data-ttu-id="96065-124">Описание</span><span class="sxs-lookup"><span data-stu-id="96065-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96065-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96065-125">Authorization</span></span>  | <span data-ttu-id="96065-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96065-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96065-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96065-128">Request body</span></span>
<span data-ttu-id="96065-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96065-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96065-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="96065-130">Response</span></span>

<span data-ttu-id="96065-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [outlookTaskGroup](../resources/outlooktaskgroup.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="96065-131">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96065-132">Пример</span><span class="sxs-lookup"><span data-stu-id="96065-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96065-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="96065-133">Request</span></span>
<span data-ttu-id="96065-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96065-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="96065-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="96065-135">Response</span></span>
<span data-ttu-id="96065-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="96065-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "id": "AAMkADIyAAADJ5pYAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxLA==",
      "isDefaultGroup": true,
      "name": "My Tasks",
      "groupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAhrbe-AAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
      "isDefaultGroup": false,
      "name": "Leisure Tasks",
      "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
