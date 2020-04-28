---
title: Создание outlookTaskFolder
description: Создайте папку задач Outlook в заданном outlookTaskGroup.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 05a0c3052114bcc1817a43f8476b4214da05ee67
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468101"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="f4b72-103">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="f4b72-103">Create outlookTaskFolder</span></span>

<span data-ttu-id="f4b72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4b72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4b72-105">Создайте папку задач Outlook в заданном [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="f4b72-105">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f4b72-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4b72-106">Permissions</span></span>
<span data-ttu-id="f4b72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4b72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4b72-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4b72-109">Permission type</span></span>      | <span data-ttu-id="f4b72-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4b72-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4b72-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4b72-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4b72-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4b72-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f4b72-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4b72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4b72-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4b72-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f4b72-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4b72-115">Application</span></span> | <span data-ttu-id="f4b72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4b72-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4b72-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4b72-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="f4b72-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4b72-118">Request headers</span></span>
| <span data-ttu-id="f4b72-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f4b72-119">Name</span></span>       | <span data-ttu-id="f4b72-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f4b72-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f4b72-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4b72-121">Authorization</span></span>  | <span data-ttu-id="f4b72-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4b72-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4b72-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4b72-124">Request body</span></span>
<span data-ttu-id="f4b72-125">В тексте запроса добавьте представление объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4b72-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f4b72-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4b72-126">Response</span></span>

<span data-ttu-id="f4b72-127">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4b72-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4b72-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f4b72-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4b72-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4b72-129">Request</span></span>
<span data-ttu-id="f4b72-130">В следующем примере создается папка задач, вызываемая `Cooking` из указанной группы задач.</span><span class="sxs-lookup"><span data-stu-id="f4b72-130">The following example creates a task folder called `Cooking` in the specified task group.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4b72-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4b72-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskgroups/AAMkADIyAAAhrbe-AAA'/taskfolders
Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```
# <a name="javascript"></a>[<span data-ttu-id="f4b72-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4b72-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f4b72-133">В тексте запроса добавьте представление объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4b72-133">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f4b72-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4b72-134">Response</span></span>
<span data-ttu-id="f4b72-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4b72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPXAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
  "isDefaultFolder": false,
  "name": "Cooking",
  "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
