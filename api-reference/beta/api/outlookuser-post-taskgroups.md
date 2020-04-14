---
title: Создание outlookTaskGroup
description: Создайте группу задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ed70266ccd093128fa3d3f48c8999f7b615a759c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456187"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="27991-103">Создание outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="27991-103">Create outlookTaskGroup</span></span>

<span data-ttu-id="27991-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27991-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27991-105">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="27991-105">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="27991-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27991-106">Permissions</span></span>
<span data-ttu-id="27991-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27991-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27991-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27991-109">Permission type</span></span>      | <span data-ttu-id="27991-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27991-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27991-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27991-111">Delegated (work or school account)</span></span> | <span data-ttu-id="27991-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27991-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="27991-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27991-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27991-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27991-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="27991-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27991-115">Application</span></span> | <span data-ttu-id="27991-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27991-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27991-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27991-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="27991-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27991-118">Request headers</span></span>
| <span data-ttu-id="27991-119">Имя</span><span class="sxs-lookup"><span data-stu-id="27991-119">Name</span></span>       | <span data-ttu-id="27991-120">Описание</span><span class="sxs-lookup"><span data-stu-id="27991-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="27991-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27991-121">Authorization</span></span>  | <span data-ttu-id="27991-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27991-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27991-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="27991-124">Request body</span></span>
<span data-ttu-id="27991-125">В тексте запроса добавьте представление объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27991-125">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="27991-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="27991-126">Response</span></span>

<span data-ttu-id="27991-127">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27991-127">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27991-128">Пример</span><span class="sxs-lookup"><span data-stu-id="27991-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27991-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="27991-129">Request</span></span>
<span data-ttu-id="27991-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27991-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27991-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="27991-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="27991-132">C#</span><span class="sxs-lookup"><span data-stu-id="27991-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27991-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27991-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27991-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27991-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="27991-135">В тексте запроса добавьте представление объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27991-135">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="27991-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="27991-136">Response</span></span>
<span data-ttu-id="27991-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27991-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
