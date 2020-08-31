---
title: Обновление outlooktaskfolder
description: Обновление свойств, доступных для записи, папки задач Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 99c3ca379760812ad3312395b3f03d2bdaf3d2a8
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311958"
---
# <a name="update-outlooktaskfolder-deprecated"></a><span data-ttu-id="3a13e-103">Обновление outlooktaskfolder (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="3a13e-103">Update outlooktaskfolder (deprecated)</span></span>

<span data-ttu-id="3a13e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a13e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="3a13e-105">Обновление свойств, доступных для записи, папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="3a13e-105">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="3a13e-106">Вы не можете изменить значение свойства **Name** папки задач по умолчанию, "задачи".</span><span class="sxs-lookup"><span data-stu-id="3a13e-106">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="3a13e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a13e-107">Permissions</span></span>
<span data-ttu-id="3a13e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a13e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a13e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a13e-110">Permission type</span></span>      | <span data-ttu-id="3a13e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a13e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a13e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a13e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a13e-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a13e-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3a13e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a13e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a13e-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a13e-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="3a13e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a13e-116">Application</span></span> | <span data-ttu-id="3a13e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a13e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a13e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a13e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3a13e-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a13e-119">Optional request headers</span></span>
| <span data-ttu-id="3a13e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3a13e-120">Name</span></span>       | <span data-ttu-id="3a13e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3a13e-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3a13e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a13e-122">Authorization</span></span>  | <span data-ttu-id="3a13e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a13e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a13e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a13e-125">Request body</span></span>
<span data-ttu-id="3a13e-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3a13e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3a13e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a13e-129">Property</span></span>     | <span data-ttu-id="3a13e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3a13e-130">Type</span></span>   |<span data-ttu-id="3a13e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3a13e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a13e-132">name</span><span class="sxs-lookup"><span data-stu-id="3a13e-132">name</span></span>|<span data-ttu-id="3a13e-133">String</span><span class="sxs-lookup"><span data-stu-id="3a13e-133">String</span></span>|<span data-ttu-id="3a13e-134">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="3a13e-134">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="3a13e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a13e-135">Response</span></span>

<span data-ttu-id="3a13e-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a13e-136">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a13e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="3a13e-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a13e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a13e-138">Request</span></span>
<span data-ttu-id="3a13e-139">В следующем примере показано изменение имени указанной папки задач на `Charity work` .</span><span class="sxs-lookup"><span data-stu-id="3a13e-139">The following example changes the name of the specified task folder to `Charity work`.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a13e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a13e-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3a13e-141">C#</span><span class="sxs-lookup"><span data-stu-id="3a13e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a13e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a13e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a13e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a13e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3a13e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a13e-144">Response</span></span>
<span data-ttu-id="3a13e-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a13e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
