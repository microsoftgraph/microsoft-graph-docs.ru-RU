---
title: Получение outlookTaskFolder
description: Получение свойств и связей указанной папки задач Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 918692269cc7af11ba8a9f1bbb0881f41d112bdb
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402690"
---
# <a name="get-outlooktaskfolder-deprecated"></a><span data-ttu-id="2e134-103">Получение outlookTaskFolder (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="2e134-103">Get outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="2e134-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e134-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="2e134-105">Получение свойств и связей указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="2e134-105">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e134-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e134-106">Permissions</span></span>
<span data-ttu-id="2e134-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e134-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e134-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e134-109">Permission type</span></span>      | <span data-ttu-id="2e134-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e134-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e134-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e134-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2e134-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2e134-112">Tasks.Read</span></span>    |
|<span data-ttu-id="2e134-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e134-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e134-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2e134-114">Tasks.Read</span></span>    |
|<span data-ttu-id="2e134-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e134-115">Application</span></span> | <span data-ttu-id="2e134-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e134-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e134-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e134-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}
GET /me/outlook/taskGroups/{id}/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e134-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e134-118">Optional query parameters</span></span>
<span data-ttu-id="2e134-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2e134-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e134-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e134-120">Request headers</span></span>
| <span data-ttu-id="2e134-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2e134-121">Name</span></span>      |<span data-ttu-id="2e134-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2e134-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e134-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e134-123">Authorization</span></span>  | <span data-ttu-id="2e134-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e134-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e134-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e134-126">Request body</span></span>
<span data-ttu-id="2e134-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e134-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e134-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e134-128">Response</span></span>

<span data-ttu-id="2e134-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e134-129">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e134-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2e134-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e134-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e134-131">Request</span></span>
<span data-ttu-id="2e134-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e134-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e134-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e134-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=
```
# <a name="c"></a>[<span data-ttu-id="2e134-134">C#</span><span class="sxs-lookup"><span data-stu-id="2e134-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e134-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e134-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e134-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e134-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e134-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e134-137">Response</span></span>
<span data-ttu-id="2e134-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e134-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->