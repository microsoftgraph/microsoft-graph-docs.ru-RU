---
title: Создание outlookTaskGroup
description: Создайте группу задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2ccb22e1838fd3e8ba73df4133121250927f9218
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35452272"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="9f65d-103">Создание outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="9f65d-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f65d-104">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f65d-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f65d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f65d-105">Permissions</span></span>
<span data-ttu-id="9f65d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f65d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f65d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f65d-108">Permission type</span></span>      | <span data-ttu-id="9f65d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f65d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f65d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f65d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f65d-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f65d-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9f65d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f65d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f65d-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f65d-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9f65d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f65d-114">Application</span></span> | <span data-ttu-id="9f65d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f65d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f65d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f65d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="9f65d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f65d-117">Request headers</span></span>
| <span data-ttu-id="9f65d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9f65d-118">Name</span></span>       | <span data-ttu-id="9f65d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9f65d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9f65d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f65d-120">Authorization</span></span>  | <span data-ttu-id="9f65d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f65d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f65d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f65d-123">Request body</span></span>
<span data-ttu-id="9f65d-124">В тексте запроса добавьте представление объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f65d-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9f65d-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f65d-125">Response</span></span>

<span data-ttu-id="9f65d-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f65d-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f65d-127">Пример</span><span class="sxs-lookup"><span data-stu-id="9f65d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f65d-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f65d-128">Request</span></span>
<span data-ttu-id="9f65d-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f65d-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9f65d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f65d-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9f65d-131">C#</span><span class="sxs-lookup"><span data-stu-id="9f65d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f65d-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="9f65d-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9f65d-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9f65d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9f65d-134">В тексте запроса добавьте представление объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f65d-134">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9f65d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f65d-135">Response</span></span>
<span data-ttu-id="9f65d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f65d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
