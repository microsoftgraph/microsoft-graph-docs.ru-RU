---
title: Создание outlookTaskGroup
description: Создайте группу задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7fadfbb0ff448b74d02460d6437a92d5cee327d3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265662"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="12c6c-103">Создание outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="12c6c-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12c6c-104">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="12c6c-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="12c6c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12c6c-105">Permissions</span></span>
<span data-ttu-id="12c6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12c6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12c6c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12c6c-108">Permission type</span></span>      | <span data-ttu-id="12c6c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12c6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12c6c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12c6c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="12c6c-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12c6c-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="12c6c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12c6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12c6c-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12c6c-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="12c6c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12c6c-114">Application</span></span> | <span data-ttu-id="12c6c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12c6c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12c6c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12c6c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="12c6c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12c6c-117">Request headers</span></span>
| <span data-ttu-id="12c6c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="12c6c-118">Name</span></span>       | <span data-ttu-id="12c6c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="12c6c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12c6c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12c6c-120">Authorization</span></span>  | <span data-ttu-id="12c6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12c6c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12c6c-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12c6c-123">Request body</span></span>
<span data-ttu-id="12c6c-124">В тексте запроса добавьте представление объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12c6c-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="12c6c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="12c6c-125">Response</span></span>

<span data-ttu-id="12c6c-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12c6c-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c6c-127">Пример</span><span class="sxs-lookup"><span data-stu-id="12c6c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12c6c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="12c6c-128">Request</span></span>
<span data-ttu-id="12c6c-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12c6c-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="12c6c-130">В тексте запроса добавьте представление объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12c6c-130">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="12c6c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="12c6c-131">Response</span></span>
<span data-ttu-id="12c6c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12c6c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="12c6c-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="12c6c-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="12c6c-136">C#</span><span class="sxs-lookup"><span data-stu-id="12c6c-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_outlooktaskgroup_from_outlookuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12c6c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="12c6c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_outlooktaskgroup_from_outlookuser-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="12c6c-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="12c6c-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_outlooktaskgroup_from_outlookuser-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlookuser-post-taskgroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-post-taskgroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-post-taskgroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
