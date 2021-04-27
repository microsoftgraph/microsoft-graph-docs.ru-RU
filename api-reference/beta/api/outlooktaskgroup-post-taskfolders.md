---
title: Создание outlookTaskFolder
description: Создайте папку Outlook задач в соответствии с указанным outlookTaskGroup.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e7fd36eae4980a533f4d3bc02223bab788f8e7a4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049221"
---
# <a name="create-outlooktaskfolder-deprecated"></a><span data-ttu-id="ddd9f-103">Создание outlookTaskFolder (амортизации)</span><span class="sxs-lookup"><span data-stu-id="ddd9f-103">Create outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="ddd9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddd9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="ddd9f-105">Создайте папку Outlook задач в указанном [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="ddd9f-105">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ddd9f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddd9f-106">Permissions</span></span>
<span data-ttu-id="ddd9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddd9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddd9f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddd9f-109">Permission type</span></span>      | <span data-ttu-id="ddd9f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddd9f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddd9f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddd9f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ddd9f-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddd9f-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ddd9f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddd9f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddd9f-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddd9f-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ddd9f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddd9f-115">Application</span></span> | <span data-ttu-id="ddd9f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddd9f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddd9f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddd9f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="ddd9f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddd9f-118">Request headers</span></span>
| <span data-ttu-id="ddd9f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ddd9f-119">Name</span></span>       | <span data-ttu-id="ddd9f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ddd9f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ddd9f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddd9f-121">Authorization</span></span>  | <span data-ttu-id="ddd9f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddd9f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddd9f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddd9f-124">Request body</span></span>
<span data-ttu-id="ddd9f-125">В теле запроса поставляем представление JSON объекта [OutlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="ddd9f-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ddd9f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddd9f-126">Response</span></span>

<span data-ttu-id="ddd9f-127">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект OutlookTaskFolder](../resources/outlooktaskfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ddd9f-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddd9f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ddd9f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddd9f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddd9f-129">Request</span></span>
<span data-ttu-id="ddd9f-130">В следующем примере создается папка задач, вызванная `Cooking` в указанной группе задач.</span><span class="sxs-lookup"><span data-stu-id="ddd9f-130">The following example creates a task folder called `Cooking` in the specified task group.</span></span>


# <a name="http"></a>[<span data-ttu-id="ddd9f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddd9f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=/taskfolders
Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```
# <a name="c"></a>[<span data-ttu-id="ddd9f-132">C#</span><span class="sxs-lookup"><span data-stu-id="ddd9f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddd9f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddd9f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddd9f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddd9f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddd9f-135">Java</span><span class="sxs-lookup"><span data-stu-id="ddd9f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskfolder-from-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ddd9f-136">В теле запроса поставляем представление JSON объекта [OutlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="ddd9f-136">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ddd9f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddd9f-137">Response</span></span>
<span data-ttu-id="ddd9f-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ddd9f-138">Here is an example of the response.</span></span> <span data-ttu-id="ddd9f-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ddd9f-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPXAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
  "isDefaultFolder": false,
  "name": "Cooking",
  "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


