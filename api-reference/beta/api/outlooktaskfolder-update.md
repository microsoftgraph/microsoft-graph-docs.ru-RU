---
title: Обновление outlooktaskfolder
description: Обновление свойств, доступных для записи, папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8da97f756d449bf6494f13bd43b6228fa6a21c89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983708"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="15ba8-103">Обновление outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="15ba8-103">Update outlooktaskfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15ba8-104">Обновление свойств, доступных для записи, папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="15ba8-104">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="15ba8-105">Вы не можете изменить значение свойства **Name** папки задач по умолчанию, "задачи".</span><span class="sxs-lookup"><span data-stu-id="15ba8-105">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="15ba8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15ba8-106">Permissions</span></span>
<span data-ttu-id="15ba8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15ba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15ba8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15ba8-109">Permission type</span></span>      | <span data-ttu-id="15ba8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15ba8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15ba8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15ba8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="15ba8-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ba8-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="15ba8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15ba8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15ba8-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15ba8-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="15ba8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15ba8-115">Application</span></span> | <span data-ttu-id="15ba8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15ba8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15ba8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15ba8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="15ba8-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15ba8-118">Optional request headers</span></span>
| <span data-ttu-id="15ba8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="15ba8-119">Name</span></span>       | <span data-ttu-id="15ba8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="15ba8-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="15ba8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15ba8-121">Authorization</span></span>  | <span data-ttu-id="15ba8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15ba8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15ba8-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15ba8-124">Request body</span></span>
<span data-ttu-id="15ba8-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="15ba8-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="15ba8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="15ba8-128">Property</span></span>     | <span data-ttu-id="15ba8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="15ba8-129">Type</span></span>   |<span data-ttu-id="15ba8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="15ba8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15ba8-131">name</span><span class="sxs-lookup"><span data-stu-id="15ba8-131">name</span></span>|<span data-ttu-id="15ba8-132">String</span><span class="sxs-lookup"><span data-stu-id="15ba8-132">String</span></span>|<span data-ttu-id="15ba8-133">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="15ba8-133">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="15ba8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="15ba8-134">Response</span></span>

<span data-ttu-id="15ba8-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15ba8-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15ba8-136">Пример</span><span class="sxs-lookup"><span data-stu-id="15ba8-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15ba8-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="15ba8-137">Request</span></span>
<span data-ttu-id="15ba8-138">В следующем примере показано изменение имени указанной папки задач на `Charity work`.</span><span class="sxs-lookup"><span data-stu-id="15ba8-138">The following example changes the name of the specified task folder to `Charity work`.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="15ba8-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="15ba8-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="15ba8-140">C#</span><span class="sxs-lookup"><span data-stu-id="15ba8-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15ba8-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="15ba8-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15ba8-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="15ba8-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="15ba8-143">Java</span><span class="sxs-lookup"><span data-stu-id="15ba8-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktaskfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="15ba8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="15ba8-144">Response</span></span>
<span data-ttu-id="15ba8-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15ba8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
