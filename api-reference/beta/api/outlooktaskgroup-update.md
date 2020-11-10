---
title: Обновление outlooktaskgroup
description: Обновление свойств, доступных для записи, для группы задач Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8b0dbeffd373e702bdd0ac8560f659436e24dee6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978032"
---
# <a name="update-outlooktaskgroup-deprecated"></a><span data-ttu-id="8681f-103">Обновление outlooktaskgroup (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="8681f-103">Update outlooktaskgroup (deprecated)</span></span>

<span data-ttu-id="8681f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8681f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="8681f-105">Обновление свойств, доступных для записи, для группы задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="8681f-105">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="8681f-106">Обратите внимание, что нельзя изменить имя группы задач по умолчанию "Мои задачи".</span><span class="sxs-lookup"><span data-stu-id="8681f-106">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="8681f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8681f-107">Permissions</span></span>
<span data-ttu-id="8681f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8681f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8681f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8681f-110">Permission type</span></span>      | <span data-ttu-id="8681f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8681f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8681f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8681f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8681f-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8681f-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8681f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8681f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8681f-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8681f-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8681f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8681f-116">Application</span></span> | <span data-ttu-id="8681f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8681f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8681f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8681f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskGroups/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="8681f-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8681f-119">Optional request headers</span></span>
| <span data-ttu-id="8681f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8681f-120">Name</span></span>       | <span data-ttu-id="8681f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8681f-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8681f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8681f-122">Authorization</span></span>  | <span data-ttu-id="8681f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8681f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8681f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8681f-125">Request body</span></span>
<span data-ttu-id="8681f-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8681f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8681f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8681f-129">Property</span></span>     | <span data-ttu-id="8681f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8681f-130">Type</span></span>   |<span data-ttu-id="8681f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8681f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8681f-132">name</span><span class="sxs-lookup"><span data-stu-id="8681f-132">name</span></span>|<span data-ttu-id="8681f-133">String</span><span class="sxs-lookup"><span data-stu-id="8681f-133">String</span></span>|<span data-ttu-id="8681f-134">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="8681f-134">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="8681f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8681f-135">Response</span></span>

<span data-ttu-id="8681f-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [outlookTaskGroup](../resources/outlooktaskgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8681f-136">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8681f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="8681f-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8681f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="8681f-138">Request</span></span>
<span data-ttu-id="8681f-139">В следующем примере имя группы задач изменяется на "личные задачи".</span><span class="sxs-lookup"><span data-stu-id="8681f-139">The following example changes the name of a task group to "Personal Tasks".</span></span> 

# <a name="http"></a>[<span data-ttu-id="8681f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="8681f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
Content-type: application/json
Content-length: 28

{
  "name": "Personal Tasks",
}
```
# <a name="c"></a>[<span data-ttu-id="8681f-141">C#</span><span class="sxs-lookup"><span data-stu-id="8681f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8681f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8681f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8681f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8681f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8681f-144">Java</span><span class="sxs-lookup"><span data-stu-id="8681f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8681f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8681f-145">Response</span></span>
<span data-ttu-id="8681f-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8681f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjw==",
  "isDefaultGroup": false,
  "name": "Personal Tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


