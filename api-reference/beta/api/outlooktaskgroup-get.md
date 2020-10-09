---
title: Получение outlookTaskGroup
description: Получение свойств и связей указанной группы задач Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1f0c2cbd766e75f7f440d05a27a0b29d1851e7bc
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400916"
---
# <a name="get-outlooktaskgroup-deprecated"></a><span data-ttu-id="8639e-103">Получение outlookTaskGroup (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="8639e-103">Get outlookTaskGroup (deprecated)</span></span>

<span data-ttu-id="8639e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8639e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="8639e-105">Получение свойств и связей указанной группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="8639e-105">Get the properties and relationships of the specified Outlook task group.</span></span>
## <a name="permissions"></a><span data-ttu-id="8639e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8639e-106">Permissions</span></span>
<span data-ttu-id="8639e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8639e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8639e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8639e-109">Permission type</span></span>      | <span data-ttu-id="8639e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8639e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8639e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8639e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8639e-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8639e-112">Tasks.Read</span></span>    |
|<span data-ttu-id="8639e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8639e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8639e-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8639e-114">Tasks.Read</span></span>    |
|<span data-ttu-id="8639e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8639e-115">Application</span></span> | <span data-ttu-id="8639e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8639e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8639e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8639e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8639e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8639e-118">Optional query parameters</span></span>
<span data-ttu-id="8639e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8639e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8639e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8639e-120">Request headers</span></span>
| <span data-ttu-id="8639e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8639e-121">Name</span></span>      |<span data-ttu-id="8639e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8639e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8639e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8639e-123">Authorization</span></span>  | <span data-ttu-id="8639e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8639e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8639e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8639e-126">Request body</span></span>
<span data-ttu-id="8639e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8639e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8639e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8639e-128">Response</span></span>

<span data-ttu-id="8639e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8639e-129">If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8639e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8639e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8639e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8639e-131">Request</span></span>
<span data-ttu-id="8639e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8639e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8639e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8639e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="c"></a>[<span data-ttu-id="8639e-134">C#</span><span class="sxs-lookup"><span data-stu-id="8639e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8639e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8639e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8639e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8639e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8639e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8639e-137">Response</span></span>
<span data-ttu-id="8639e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8639e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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