---
title: Обновление outlooktaskfolder
description: Обновим рукописные свойства папки Outlook задач.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 07bf8e50dae35458f6071f92cfc361b91e7e2f91
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055444"
---
# <a name="update-outlooktaskfolder-deprecated"></a><span data-ttu-id="a8d6b-103">Обновление outlooktaskfolder (износ)</span><span class="sxs-lookup"><span data-stu-id="a8d6b-103">Update outlooktaskfolder (deprecated)</span></span>

<span data-ttu-id="a8d6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8d6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="a8d6b-105">Обновим рукописные свойства папки Outlook задач.</span><span class="sxs-lookup"><span data-stu-id="a8d6b-105">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="a8d6b-106">Невозможно изменить значение **свойства имени** папки задач по умолчанию "Задачи".</span><span class="sxs-lookup"><span data-stu-id="a8d6b-106">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="a8d6b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8d6b-107">Permissions</span></span>
<span data-ttu-id="a8d6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8d6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8d6b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8d6b-110">Permission type</span></span>      | <span data-ttu-id="a8d6b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8d6b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8d6b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8d6b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a8d6b-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8d6b-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a8d6b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8d6b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8d6b-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8d6b-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a8d6b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8d6b-116">Application</span></span> | <span data-ttu-id="a8d6b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8d6b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8d6b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8d6b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a8d6b-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8d6b-119">Optional request headers</span></span>
| <span data-ttu-id="a8d6b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a8d6b-120">Name</span></span>       | <span data-ttu-id="a8d6b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a8d6b-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a8d6b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8d6b-122">Authorization</span></span>  | <span data-ttu-id="a8d6b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8d6b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8d6b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8d6b-125">Request body</span></span>
<span data-ttu-id="a8d6b-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a8d6b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a8d6b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8d6b-129">Property</span></span>     | <span data-ttu-id="a8d6b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a8d6b-130">Type</span></span>   |<span data-ttu-id="a8d6b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a8d6b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8d6b-132">name</span><span class="sxs-lookup"><span data-stu-id="a8d6b-132">name</span></span>|<span data-ttu-id="a8d6b-133">String</span><span class="sxs-lookup"><span data-stu-id="a8d6b-133">String</span></span>|<span data-ttu-id="a8d6b-134">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="a8d6b-134">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="a8d6b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8d6b-135">Response</span></span>

<span data-ttu-id="a8d6b-136">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект OutlookTaskFolder](../resources/outlooktaskfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a8d6b-136">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8d6b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a8d6b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8d6b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8d6b-138">Request</span></span>
<span data-ttu-id="a8d6b-139">В следующем примере имя указанной папки задач изменяется на `Charity work` .</span><span class="sxs-lookup"><span data-stu-id="a8d6b-139">The following example changes the name of the specified task folder to `Charity work`.</span></span>

# <a name="http"></a>[<span data-ttu-id="a8d6b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8d6b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=
Content-type: application/json
Content-length: 31

{
  "name": "Charity work"
}
```
# <a name="c"></a>[<span data-ttu-id="a8d6b-141">C#</span><span class="sxs-lookup"><span data-stu-id="a8d6b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8d6b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8d6b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8d6b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8d6b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8d6b-144">Java</span><span class="sxs-lookup"><span data-stu-id="a8d6b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktaskfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a8d6b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8d6b-145">Response</span></span>
<span data-ttu-id="a8d6b-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8d6b-146">Here is an example of the response.</span></span> <span data-ttu-id="a8d6b-147">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a8d6b-147">Note: The response object shown here might be shortened for readability.</span></span>
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
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAKfQ==",
  "isDefaultFolder": false,
  "name": "Charity work",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


