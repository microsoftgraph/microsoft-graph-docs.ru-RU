---
title: Получение outlookTaskGroup
description: Получение свойств и связей указанной группы задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8d3d5b164d3bdcfee98f9f664afd187b91d9f016
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456123"
---
# <a name="get-outlooktaskgroup"></a><span data-ttu-id="f9284-103">Получение outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f9284-103">Get outlookTaskGroup</span></span>

<span data-ttu-id="f9284-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f9284-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9284-105">Получение свойств и связей указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="f9284-105">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9284-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9284-106">Permissions</span></span>
<span data-ttu-id="f9284-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9284-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9284-109">Permission type</span></span>      | <span data-ttu-id="f9284-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9284-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9284-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9284-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f9284-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f9284-112">Tasks.Read</span></span>    |
|<span data-ttu-id="f9284-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9284-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9284-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f9284-114">Tasks.Read</span></span>    |
|<span data-ttu-id="f9284-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9284-115">Application</span></span> | <span data-ttu-id="f9284-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9284-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9284-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9284-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9284-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9284-118">Optional query parameters</span></span>
<span data-ttu-id="f9284-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f9284-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9284-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9284-120">Request headers</span></span>
| <span data-ttu-id="f9284-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f9284-121">Name</span></span>      |<span data-ttu-id="f9284-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f9284-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9284-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9284-123">Authorization</span></span>  | <span data-ttu-id="f9284-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9284-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9284-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9284-126">Request body</span></span>
<span data-ttu-id="f9284-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9284-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9284-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9284-128">Response</span></span>

<span data-ttu-id="f9284-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9284-129">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9284-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f9284-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9284-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9284-131">Request</span></span>
<span data-ttu-id="f9284-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9284-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9284-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9284-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="c"></a>[<span data-ttu-id="f9284-134">C#</span><span class="sxs-lookup"><span data-stu-id="f9284-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9284-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9284-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9284-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9284-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f9284-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9284-137">Response</span></span>
<span data-ttu-id="f9284-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9284-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
