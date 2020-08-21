---
title: Создание объекта outlookTaskGroup
description: Создание группы задач Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 12160cf04ac2fbb0a5ed8dabfcc5870765b30511
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849284"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="78498-103">Создание объекта outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="78498-103">Create outlookTaskGroup</span></span>

<span data-ttu-id="78498-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78498-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="78498-105">Создание группы задач Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="78498-105">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="78498-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78498-106">Permissions</span></span>
<span data-ttu-id="78498-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78498-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78498-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78498-109">Permission type</span></span>      | <span data-ttu-id="78498-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78498-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78498-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78498-111">Delegated (work or school account)</span></span> | <span data-ttu-id="78498-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78498-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="78498-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78498-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78498-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78498-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="78498-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78498-115">Application</span></span> | <span data-ttu-id="78498-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78498-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78498-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78498-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="78498-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78498-118">Request headers</span></span>
| <span data-ttu-id="78498-119">Имя</span><span class="sxs-lookup"><span data-stu-id="78498-119">Name</span></span>       | <span data-ttu-id="78498-120">Описание</span><span class="sxs-lookup"><span data-stu-id="78498-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="78498-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78498-121">Authorization</span></span>  | <span data-ttu-id="78498-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78498-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78498-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78498-124">Request body</span></span>
<span data-ttu-id="78498-125">Представьте в тексте запроса описание объекта [outlookTaskGroup в формате](../resources/outlooktaskgroup.md) JSON.</span><span class="sxs-lookup"><span data-stu-id="78498-125">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="78498-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="78498-126">Response</span></span>

<span data-ttu-id="78498-127">При успешном выполнении этот метод возвращает `201 Created` код ответа [и объект outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="78498-127">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78498-128">Пример</span><span class="sxs-lookup"><span data-stu-id="78498-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78498-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="78498-129">Request</span></span>
<span data-ttu-id="78498-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78498-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="78498-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="78498-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="78498-132">C#</span><span class="sxs-lookup"><span data-stu-id="78498-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskgroup-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78498-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78498-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskgroup-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78498-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78498-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskgroup-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="78498-135">Представьте в тексте запроса описание объекта [outlookTaskGroup в формате](../resources/outlooktaskgroup.md) JSON.</span><span class="sxs-lookup"><span data-stu-id="78498-135">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="78498-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="78498-136">Response</span></span>
<span data-ttu-id="78498-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78498-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
