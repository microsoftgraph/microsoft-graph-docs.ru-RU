---
title: Get outlookTaskGroup
description: Получите свойства и связи указанной Outlook группы задач.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6abb0d4103cf63fc0ff48a8070cc81c32469f139
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049214"
---
# <a name="get-outlooktaskgroup-deprecated"></a><span data-ttu-id="30718-103">Получить outlookTaskGroup (обесценилось)</span><span class="sxs-lookup"><span data-stu-id="30718-103">Get outlookTaskGroup (deprecated)</span></span>

<span data-ttu-id="30718-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30718-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="30718-105">Получите свойства и связи указанной Outlook группы задач.</span><span class="sxs-lookup"><span data-stu-id="30718-105">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="30718-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30718-106">Permissions</span></span>
<span data-ttu-id="30718-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30718-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30718-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30718-109">Permission type</span></span>      | <span data-ttu-id="30718-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30718-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30718-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30718-111">Delegated (work or school account)</span></span> | <span data-ttu-id="30718-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="30718-112">Tasks.Read</span></span>    |
|<span data-ttu-id="30718-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30718-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30718-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="30718-114">Tasks.Read</span></span>    |
|<span data-ttu-id="30718-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30718-115">Application</span></span> | <span data-ttu-id="30718-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30718-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30718-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30718-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30718-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30718-118">Optional query parameters</span></span>
<span data-ttu-id="30718-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="30718-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30718-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30718-120">Request headers</span></span>
| <span data-ttu-id="30718-121">Имя</span><span class="sxs-lookup"><span data-stu-id="30718-121">Name</span></span>      |<span data-ttu-id="30718-122">Описание</span><span class="sxs-lookup"><span data-stu-id="30718-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="30718-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30718-123">Authorization</span></span>  | <span data-ttu-id="30718-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30718-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30718-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30718-126">Request body</span></span>
<span data-ttu-id="30718-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30718-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30718-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="30718-128">Response</span></span>

<span data-ttu-id="30718-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект OutlookTaskGroup](../resources/outlooktaskgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="30718-129">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30718-130">Пример</span><span class="sxs-lookup"><span data-stu-id="30718-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30718-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="30718-131">Request</span></span>
<span data-ttu-id="30718-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30718-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="30718-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="30718-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="c"></a>[<span data-ttu-id="30718-134">C#</span><span class="sxs-lookup"><span data-stu-id="30718-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30718-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30718-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30718-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30718-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30718-137">Java</span><span class="sxs-lookup"><span data-stu-id="30718-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="30718-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="30718-138">Response</span></span>
<span data-ttu-id="30718-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30718-139">Here is an example of the response.</span></span> <span data-ttu-id="30718-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30718-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
    "id": "AAMkADIyAAAhrbe-AAA=",
    "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
    "isDefaultGroup": false,
    "name": "Leisure Tasks",
    "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
