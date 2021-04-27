---
title: Обновление outlooktaskgroup
description: Обновим писаемые свойства группы Outlook задач.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 37bf87e8d52ac320d29fd7be1f6cdd3dae7165ea
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049207"
---
# <a name="update-outlooktaskgroup-deprecated"></a><span data-ttu-id="d8cd2-103">Обновление outlooktaskgroup (неподготовленное)</span><span class="sxs-lookup"><span data-stu-id="d8cd2-103">Update outlooktaskgroup (deprecated)</span></span>

<span data-ttu-id="d8cd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8cd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="d8cd2-105">Обновим писаемые свойства группы Outlook задач.</span><span class="sxs-lookup"><span data-stu-id="d8cd2-105">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="d8cd2-106">Обратите внимание, что нельзя изменить имя группы задач по умолчанию "Мои задачи".</span><span class="sxs-lookup"><span data-stu-id="d8cd2-106">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="d8cd2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8cd2-107">Permissions</span></span>
<span data-ttu-id="d8cd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8cd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8cd2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8cd2-110">Permission type</span></span>      | <span data-ttu-id="d8cd2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8cd2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8cd2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8cd2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8cd2-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8cd2-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d8cd2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8cd2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8cd2-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8cd2-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d8cd2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8cd2-116">Application</span></span> | <span data-ttu-id="d8cd2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8cd2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8cd2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8cd2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskGroups/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d8cd2-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8cd2-119">Optional request headers</span></span>
| <span data-ttu-id="d8cd2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d8cd2-120">Name</span></span>       | <span data-ttu-id="d8cd2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d8cd2-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d8cd2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8cd2-122">Authorization</span></span>  | <span data-ttu-id="d8cd2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8cd2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8cd2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8cd2-125">Request body</span></span>
<span data-ttu-id="d8cd2-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d8cd2-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d8cd2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8cd2-129">Property</span></span>     | <span data-ttu-id="d8cd2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d8cd2-130">Type</span></span>   |<span data-ttu-id="d8cd2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d8cd2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8cd2-132">name</span><span class="sxs-lookup"><span data-stu-id="d8cd2-132">name</span></span>|<span data-ttu-id="d8cd2-133">String</span><span class="sxs-lookup"><span data-stu-id="d8cd2-133">String</span></span>|<span data-ttu-id="d8cd2-134">Имя группы задач.</span><span class="sxs-lookup"><span data-stu-id="d8cd2-134">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="d8cd2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8cd2-135">Response</span></span>

<span data-ttu-id="d8cd2-136">В случае успешной работы этот метод возвращает код ответа и `200 OK` обновленный [объект OutlookTaskGroup](../resources/outlooktaskgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d8cd2-136">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8cd2-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d8cd2-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8cd2-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8cd2-138">Request</span></span>
<span data-ttu-id="d8cd2-139">В следующем примере изменяется имя группы задач на "Личные задачи".</span><span class="sxs-lookup"><span data-stu-id="d8cd2-139">The following example changes the name of a task group to "Personal Tasks".</span></span> 

# <a name="http"></a>[<span data-ttu-id="d8cd2-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8cd2-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d8cd2-141">C#</span><span class="sxs-lookup"><span data-stu-id="d8cd2-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8cd2-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8cd2-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8cd2-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8cd2-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8cd2-144">Java</span><span class="sxs-lookup"><span data-stu-id="d8cd2-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d8cd2-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8cd2-145">Response</span></span>
<span data-ttu-id="d8cd2-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8cd2-146">Here is an example of the response.</span></span> <span data-ttu-id="d8cd2-147">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d8cd2-147">Note: The response object shown here might be shortened for readability.</span></span>
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


