---
title: Перечисление объектов taskGroups
description: Получение всех групп задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5dd844356b83005dd8df9d7e9b4ce52c8baa4e3
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849224"
---
# <a name="list-taskgroups"></a><span data-ttu-id="90c2f-103">Перечисление объектов taskGroups</span><span class="sxs-lookup"><span data-stu-id="90c2f-103">List taskGroups</span></span>

<span data-ttu-id="90c2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90c2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="90c2f-105">Получение всех групп задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="90c2f-105">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="90c2f-106">Отклик всегда включает в себя группу задач `My Tasks` по умолчанию и все другие группы задач, созданные в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="90c2f-106">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="90c2f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90c2f-107">Permissions</span></span>
<span data-ttu-id="90c2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90c2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90c2f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90c2f-110">Permission type</span></span>      | <span data-ttu-id="90c2f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90c2f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90c2f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90c2f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="90c2f-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="90c2f-113">Tasks.Read</span></span>    |
|<span data-ttu-id="90c2f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90c2f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90c2f-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="90c2f-115">Tasks.Read</span></span>    |
|<span data-ttu-id="90c2f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90c2f-116">Application</span></span> | <span data-ttu-id="90c2f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90c2f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90c2f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90c2f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="90c2f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="90c2f-119">Optional query parameters</span></span>
<span data-ttu-id="90c2f-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="90c2f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90c2f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90c2f-121">Request headers</span></span>
| <span data-ttu-id="90c2f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="90c2f-122">Name</span></span>      |<span data-ttu-id="90c2f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="90c2f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90c2f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90c2f-124">Authorization</span></span>  | <span data-ttu-id="90c2f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90c2f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90c2f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90c2f-127">Request body</span></span>
<span data-ttu-id="90c2f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90c2f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90c2f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c2f-129">Response</span></span>

<span data-ttu-id="90c2f-130">При успешном выполнении этот метод возвращает `200 OK` код ответа и коллекцию объектов [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90c2f-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="90c2f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="90c2f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90c2f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90c2f-132">Request</span></span>
<span data-ttu-id="90c2f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90c2f-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90c2f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="90c2f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
# <a name="c"></a>[<span data-ttu-id="90c2f-135">C#</span><span class="sxs-lookup"><span data-stu-id="90c2f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90c2f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90c2f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90c2f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90c2f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="90c2f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c2f-138">Response</span></span>
<span data-ttu-id="90c2f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90c2f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
