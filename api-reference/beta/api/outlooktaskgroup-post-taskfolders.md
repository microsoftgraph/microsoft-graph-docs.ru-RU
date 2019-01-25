---
title: Создание outlookTaskFolder
description: Создайте папку задачи Outlook в указанном outlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 734be5578f6319307fabcac9c4e4b591b575858e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529959"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="c94f9-103">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="c94f9-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c94f9-104">Создайте папку задачи Outlook в указанном [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="c94f9-104">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c94f9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c94f9-105">Permissions</span></span>
<span data-ttu-id="c94f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c94f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c94f9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c94f9-108">Permission type</span></span>      | <span data-ttu-id="c94f9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c94f9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c94f9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c94f9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c94f9-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c94f9-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c94f9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c94f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c94f9-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c94f9-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c94f9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c94f9-114">Application</span></span> | <span data-ttu-id="c94f9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c94f9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c94f9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c94f9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="c94f9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c94f9-117">Request headers</span></span>
| <span data-ttu-id="c94f9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c94f9-118">Name</span></span>       | <span data-ttu-id="c94f9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c94f9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c94f9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c94f9-120">Authorization</span></span>  | <span data-ttu-id="c94f9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c94f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c94f9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c94f9-123">Request body</span></span>
<span data-ttu-id="c94f9-124">В тексте запроса укажите представление JSON объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="c94f9-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c94f9-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="c94f9-125">Response</span></span>

<span data-ttu-id="c94f9-126">Успешно завершена, этот метод возвращает `201 Created` объект [outlookTaskFolder](../resources/outlooktaskfolder.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c94f9-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c94f9-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c94f9-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c94f9-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c94f9-128">Request</span></span>
<span data-ttu-id="c94f9-129">В следующем примере создается задача папку с именем `Cooking` в группе указанной задачи.</span><span class="sxs-lookup"><span data-stu-id="c94f9-129">The following example creates a task folder called `Cooking` in the specified task group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskgroups('AAMkADIyAAAhrbe-AAA')/taskfolders 

Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```
<span data-ttu-id="c94f9-130">В тексте запроса укажите представление JSON объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="c94f9-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c94f9-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c94f9-131">Response</span></span>
<span data-ttu-id="c94f9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c94f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-post-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
