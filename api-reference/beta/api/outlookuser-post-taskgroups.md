---
title: Создание outlookTaskGroup
description: Создайте группу задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9fbfcf6f9bbf14db0eb94b71de5ce6978a55a51f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349739"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="495f4-103">Создание outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="495f4-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="495f4-104">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="495f4-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="495f4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="495f4-105">Permissions</span></span>
<span data-ttu-id="495f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="495f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="495f4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="495f4-108">Permission type</span></span>      | <span data-ttu-id="495f4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="495f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="495f4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="495f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="495f4-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="495f4-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="495f4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="495f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="495f4-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="495f4-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="495f4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="495f4-114">Application</span></span> | <span data-ttu-id="495f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="495f4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="495f4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="495f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="495f4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="495f4-117">Request headers</span></span>
| <span data-ttu-id="495f4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="495f4-118">Name</span></span>       | <span data-ttu-id="495f4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="495f4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="495f4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="495f4-120">Authorization</span></span>  | <span data-ttu-id="495f4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="495f4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="495f4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="495f4-123">Request body</span></span>
<span data-ttu-id="495f4-124">В тексте запроса добавьте представление объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="495f4-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="495f4-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="495f4-125">Response</span></span>

<span data-ttu-id="495f4-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="495f4-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="495f4-127">Пример</span><span class="sxs-lookup"><span data-stu-id="495f4-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="495f4-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="495f4-128">Request</span></span>
<span data-ttu-id="495f4-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="495f4-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="495f4-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="495f4-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-type: application/json
Content-length: 40

{
  "name": "Leisure tasks"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="495f4-131">C#</span><span class="sxs-lookup"><span data-stu-id="495f4-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="495f4-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="495f4-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="495f4-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="495f4-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="495f4-134">Java</span><span class="sxs-lookup"><span data-stu-id="495f4-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskgroup-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="495f4-135">В тексте запроса добавьте представление объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="495f4-135">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="495f4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="495f4-136">Response</span></span>
<span data-ttu-id="495f4-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="495f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjg==",
  "isDefaultGroup": false,
  "name": "Leisure tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
