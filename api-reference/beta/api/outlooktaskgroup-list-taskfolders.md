---
title: Список Таскфолдерс
description: Получение папок задач Outlook в определенном outlookTaskGroup.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 541788d964623b4bf99a6619c5af166db11ecbbf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978053"
---
# <a name="list-taskfolders-deprecated"></a><span data-ttu-id="52d3c-103">Список Таскфолдерс (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="52d3c-103">List taskFolders (deprecated)</span></span>

<span data-ttu-id="52d3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52d3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="52d3c-105">Получение папок задач Outlook в определенном [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="52d3c-105">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="52d3c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52d3c-106">Permissions</span></span>
<span data-ttu-id="52d3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52d3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52d3c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52d3c-109">Permission type</span></span>      | <span data-ttu-id="52d3c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52d3c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52d3c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52d3c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="52d3c-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="52d3c-112">Tasks.Read</span></span>    |
|<span data-ttu-id="52d3c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52d3c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52d3c-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="52d3c-114">Tasks.Read</span></span>    |
|<span data-ttu-id="52d3c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52d3c-115">Application</span></span> | <span data-ttu-id="52d3c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52d3c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52d3c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52d3c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52d3c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="52d3c-118">Optional query parameters</span></span>
<span data-ttu-id="52d3c-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="52d3c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52d3c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52d3c-120">Request headers</span></span>
| <span data-ttu-id="52d3c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="52d3c-121">Name</span></span>      |<span data-ttu-id="52d3c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="52d3c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52d3c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52d3c-123">Authorization</span></span>  | <span data-ttu-id="52d3c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52d3c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52d3c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52d3c-126">Request body</span></span>
<span data-ttu-id="52d3c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52d3c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52d3c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="52d3c-128">Response</span></span>

<span data-ttu-id="52d3c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52d3c-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52d3c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="52d3c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52d3c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="52d3c-131">Request</span></span>
<span data-ttu-id="52d3c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52d3c-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52d3c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="52d3c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders
```
# <a name="c"></a>[<span data-ttu-id="52d3c-134">C#</span><span class="sxs-lookup"><span data-stu-id="52d3c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52d3c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52d3c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52d3c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52d3c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52d3c-137">Java</span><span class="sxs-lookup"><span data-stu-id="52d3c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="52d3c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="52d3c-138">Response</span></span>
<span data-ttu-id="52d3c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52d3c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "AAMkADIyAAAhrbPXAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
      "isDefaultFolder": false,
      "name": "Cooking",
      "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
