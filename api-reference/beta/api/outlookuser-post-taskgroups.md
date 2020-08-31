---
title: Создание outlookTaskGroup
description: Создайте группу задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a352e301468713541cb6329df6932af10779597a
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312096"
---
# <a name="create-outlooktaskgroup-deprecated"></a><span data-ttu-id="2ddac-103">Создание outlookTaskGroup (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="2ddac-103">Create outlookTaskGroup (deprecated)</span></span>

<span data-ttu-id="2ddac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ddac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="2ddac-105">Создайте группу задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ddac-105">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ddac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ddac-106">Permissions</span></span>
<span data-ttu-id="2ddac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ddac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ddac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ddac-109">Permission type</span></span>      | <span data-ttu-id="2ddac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ddac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ddac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ddac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ddac-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ddac-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2ddac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ddac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ddac-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ddac-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2ddac-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ddac-115">Application</span></span> | <span data-ttu-id="2ddac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ddac-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ddac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ddac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="2ddac-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ddac-118">Request headers</span></span>
| <span data-ttu-id="2ddac-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2ddac-119">Name</span></span>       | <span data-ttu-id="2ddac-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2ddac-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ddac-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ddac-121">Authorization</span></span>  | <span data-ttu-id="2ddac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ddac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ddac-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ddac-124">Request body</span></span>
<span data-ttu-id="2ddac-125">В тексте запроса добавьте представление объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ddac-125">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2ddac-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ddac-126">Response</span></span>

<span data-ttu-id="2ddac-127">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ddac-127">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ddac-128">Пример</span><span class="sxs-lookup"><span data-stu-id="2ddac-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ddac-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ddac-129">Request</span></span>
<span data-ttu-id="2ddac-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ddac-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ddac-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ddac-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2ddac-132">C#</span><span class="sxs-lookup"><span data-stu-id="2ddac-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ddac-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ddac-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ddac-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ddac-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2ddac-135">В тексте запроса добавьте представление объекта [outlookTaskGroup](../resources/outlooktaskgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ddac-135">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2ddac-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ddac-136">Response</span></span>
<span data-ttu-id="2ddac-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ddac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
