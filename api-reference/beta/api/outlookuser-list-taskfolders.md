---
title: Список taskFolders
description: Получите все папки задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
ms.openlocfilehash: 71cacaf2cc666376dc696a1df124847b6a2a45eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837585"
---
# <a name="list-taskfolders"></a><span data-ttu-id="b2379-103">Список taskFolders</span><span class="sxs-lookup"><span data-stu-id="b2379-103">List taskFolders</span></span>

> <span data-ttu-id="b2379-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2379-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2379-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2379-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2379-106">Получите все папки задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="b2379-106">Get all the Outlook task folders in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="b2379-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2379-107">Permissions</span></span>
<span data-ttu-id="b2379-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2379-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2379-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2379-110">Permission type</span></span>      | <span data-ttu-id="b2379-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2379-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2379-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2379-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b2379-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="b2379-113">Tasks.Read</span></span>    |
|<span data-ttu-id="b2379-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2379-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2379-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="b2379-115">Tasks.Read</span></span>    |
|<span data-ttu-id="b2379-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2379-116">Application</span></span> | <span data-ttu-id="b2379-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2379-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2379-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2379-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b2379-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b2379-119">Optional query parameters</span></span>
<span data-ttu-id="b2379-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b2379-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2379-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2379-121">Request headers</span></span>
| <span data-ttu-id="b2379-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b2379-122">Name</span></span>      |<span data-ttu-id="b2379-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b2379-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b2379-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2379-124">Authorization</span></span>  | <span data-ttu-id="b2379-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2379-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2379-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b2379-127">Request body</span></span>
<span data-ttu-id="b2379-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2379-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2379-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2379-129">Response</span></span>

<span data-ttu-id="b2379-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [outlookTaskFolder](../resources/outlooktaskfolder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b2379-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b2379-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b2379-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2379-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2379-132">Request</span></span>
<span data-ttu-id="b2379-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2379-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders
```
##### <a name="response"></a><span data-ttu-id="b2379-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2379-134">Response</span></span>
<span data-ttu-id="b2379-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b2379-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "value": [
   {
      "id": "AAMkADIyAAAAABrJAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
      "isDefaultFolder": false,
      "name": "Monthly tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAAAAESAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAAPA==",
      "isDefaultFolder": true,
      "name": "Tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TaskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
