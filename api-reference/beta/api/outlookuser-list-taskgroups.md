---
title: Список taskGroups
description: Получение всех групп задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: eecffe794300ad682eeb24c69811e903679c41e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017440"
---
# <a name="list-taskgroups-deprecated"></a><span data-ttu-id="556ec-103">Список taskGroups (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="556ec-103">List taskGroups (deprecated)</span></span>

<span data-ttu-id="556ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="556ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="556ec-105">Получение всех групп задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="556ec-105">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="556ec-106">Ответ всегда включает группу задач по умолчанию `My Tasks` и все остальные группы задач, созданные в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="556ec-106">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="556ec-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="556ec-107">Permissions</span></span>
<span data-ttu-id="556ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="556ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="556ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="556ec-110">Permission type</span></span>      | <span data-ttu-id="556ec-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="556ec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="556ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="556ec-112">Delegated (work or school account)</span></span> | <span data-ttu-id="556ec-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="556ec-113">Tasks.Read</span></span>    |
|<span data-ttu-id="556ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="556ec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="556ec-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="556ec-115">Tasks.Read</span></span>    |
|<span data-ttu-id="556ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="556ec-116">Application</span></span> | <span data-ttu-id="556ec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="556ec-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="556ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="556ec-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="556ec-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="556ec-119">Optional query parameters</span></span>
<span data-ttu-id="556ec-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="556ec-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="556ec-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="556ec-121">Request headers</span></span>
| <span data-ttu-id="556ec-122">Имя</span><span class="sxs-lookup"><span data-stu-id="556ec-122">Name</span></span>      |<span data-ttu-id="556ec-123">Описание</span><span class="sxs-lookup"><span data-stu-id="556ec-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="556ec-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="556ec-124">Authorization</span></span>  | <span data-ttu-id="556ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="556ec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="556ec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="556ec-127">Request body</span></span>
<span data-ttu-id="556ec-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="556ec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="556ec-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="556ec-129">Response</span></span>

<span data-ttu-id="556ec-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="556ec-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="556ec-131">Пример</span><span class="sxs-lookup"><span data-stu-id="556ec-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="556ec-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="556ec-132">Request</span></span>
<span data-ttu-id="556ec-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="556ec-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="556ec-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="556ec-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
# <a name="c"></a>[<span data-ttu-id="556ec-135">C#</span><span class="sxs-lookup"><span data-stu-id="556ec-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="556ec-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="556ec-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="556ec-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="556ec-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="556ec-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="556ec-138">Response</span></span>
<span data-ttu-id="556ec-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="556ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


