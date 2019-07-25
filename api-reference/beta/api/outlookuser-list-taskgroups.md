---
title: Список taskGroups
description: Получение всех групп задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ce0110e166f4422a18332e85dc0f4cc0747e49b3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877428"
---
# <a name="list-taskgroups"></a><span data-ttu-id="3c736-103">Список taskGroups</span><span class="sxs-lookup"><span data-stu-id="3c736-103">List taskGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c736-104">Получение всех групп задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="3c736-104">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="3c736-105">Ответ всегда включает группу `My Tasks`задач по умолчанию и все остальные группы задач, созданные в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3c736-105">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c736-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c736-106">Permissions</span></span>
<span data-ttu-id="3c736-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c736-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c736-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c736-109">Permission type</span></span>      | <span data-ttu-id="3c736-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c736-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c736-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c736-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c736-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="3c736-112">Tasks.Read</span></span>    |
|<span data-ttu-id="3c736-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c736-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c736-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="3c736-114">Tasks.Read</span></span>    |
|<span data-ttu-id="3c736-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c736-115">Application</span></span> | <span data-ttu-id="3c736-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c736-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c736-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c736-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c736-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c736-118">Optional query parameters</span></span>
<span data-ttu-id="3c736-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3c736-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c736-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c736-120">Request headers</span></span>
| <span data-ttu-id="3c736-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3c736-121">Name</span></span>      |<span data-ttu-id="3c736-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3c736-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3c736-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c736-123">Authorization</span></span>  | <span data-ttu-id="3c736-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c736-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c736-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c736-126">Request body</span></span>
<span data-ttu-id="3c736-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c736-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c736-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c736-128">Response</span></span>

<span data-ttu-id="3c736-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c736-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c736-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3c736-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c736-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c736-131">Request</span></span>
<span data-ttu-id="3c736-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c736-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3c736-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c736-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c736-134">C#</span><span class="sxs-lookup"><span data-stu-id="3c736-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c736-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c736-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c736-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3c736-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3c736-137">Java</span><span class="sxs-lookup"><span data-stu-id="3c736-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c736-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c736-138">Response</span></span>
<span data-ttu-id="3c736-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c736-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
