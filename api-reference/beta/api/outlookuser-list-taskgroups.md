---
title: Список taskGroups
description: Получение всех групп задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b3ebf2896ff8805280c23680915e54f9a094a7c8
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869360"
---
# <a name="list-taskgroups"></a><span data-ttu-id="43e1b-103">Список taskGroups</span><span class="sxs-lookup"><span data-stu-id="43e1b-103">List taskGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43e1b-104">Получение всех групп задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="43e1b-104">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="43e1b-105">Ответ всегда включает группу `My Tasks`задач по умолчанию и все остальные группы задач, созданные в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="43e1b-105">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="43e1b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43e1b-106">Permissions</span></span>
<span data-ttu-id="43e1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43e1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43e1b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43e1b-109">Permission type</span></span>      | <span data-ttu-id="43e1b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43e1b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43e1b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43e1b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="43e1b-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="43e1b-112">Tasks.Read</span></span>    |
|<span data-ttu-id="43e1b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43e1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43e1b-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="43e1b-114">Tasks.Read</span></span>    |
|<span data-ttu-id="43e1b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43e1b-115">Application</span></span> | <span data-ttu-id="43e1b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43e1b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="43e1b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43e1b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="43e1b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43e1b-118">Optional query parameters</span></span>
<span data-ttu-id="43e1b-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="43e1b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43e1b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43e1b-120">Request headers</span></span>
| <span data-ttu-id="43e1b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="43e1b-121">Name</span></span>      |<span data-ttu-id="43e1b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="43e1b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="43e1b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43e1b-123">Authorization</span></span>  | <span data-ttu-id="43e1b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43e1b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43e1b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43e1b-126">Request body</span></span>
<span data-ttu-id="43e1b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43e1b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43e1b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="43e1b-128">Response</span></span>

<span data-ttu-id="43e1b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43e1b-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="43e1b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="43e1b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43e1b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="43e1b-131">Request</span></span>
<span data-ttu-id="43e1b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43e1b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="43e1b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="43e1b-133">Response</span></span>
<span data-ttu-id="43e1b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43e1b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-list-taskgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
