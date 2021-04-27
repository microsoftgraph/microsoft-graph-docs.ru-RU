---
title: Список taskFolders
description: Получите все Outlook папки задач в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f863aa4edb26ef0d3ac1325404c07737ae0285af
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052980"
---
# <a name="list-taskfolders-deprecated"></a><span data-ttu-id="a5c33-103">List taskFolders (deprecated)</span><span class="sxs-lookup"><span data-stu-id="a5c33-103">List taskFolders (deprecated)</span></span>

<span data-ttu-id="a5c33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5c33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="a5c33-105">Получите все Outlook папки задач в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5c33-105">Get all the Outlook task folders in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="a5c33-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c33-106">Permissions</span></span>
<span data-ttu-id="a5c33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5c33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5c33-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c33-109">Permission type</span></span>      | <span data-ttu-id="a5c33-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5c33-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5c33-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5c33-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5c33-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a5c33-112">Tasks.Read</span></span>    |
|<span data-ttu-id="a5c33-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5c33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5c33-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a5c33-114">Tasks.Read</span></span>    |
|<span data-ttu-id="a5c33-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5c33-115">Application</span></span> | <span data-ttu-id="a5c33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5c33-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5c33-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5c33-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a5c33-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a5c33-118">Optional query parameters</span></span>
<span data-ttu-id="a5c33-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a5c33-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5c33-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5c33-120">Request headers</span></span>
| <span data-ttu-id="a5c33-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a5c33-121">Name</span></span>      |<span data-ttu-id="a5c33-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a5c33-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5c33-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5c33-123">Authorization</span></span>  | <span data-ttu-id="a5c33-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5c33-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5c33-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5c33-126">Request body</span></span>
<span data-ttu-id="a5c33-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5c33-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5c33-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c33-128">Response</span></span>

<span data-ttu-id="a5c33-129">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов OutlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a5c33-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5c33-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a5c33-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5c33-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5c33-131">Request</span></span>
<span data-ttu-id="a5c33-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5c33-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5c33-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5c33-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders
```
# <a name="c"></a>[<span data-ttu-id="a5c33-134">C#</span><span class="sxs-lookup"><span data-stu-id="a5c33-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5c33-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5c33-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5c33-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5c33-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5c33-137">Java</span><span class="sxs-lookup"><span data-stu-id="a5c33-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskfolders-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a5c33-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c33-138">Response</span></span>
<span data-ttu-id="a5c33-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5c33-139">Here is an example of the response.</span></span> <span data-ttu-id="a5c33-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5c33-140">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List TaskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
